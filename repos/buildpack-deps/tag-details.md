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
$ docker pull buildpack-deps@sha256:ed8a3a685f4b0b8e377d4f8c8e1baa7963aea31ba5d2e97294fadaf63def04f0
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
$ docker pull buildpack-deps@sha256:29635a7ce106a6fb76fb04fb862890d50647ad6eccd38ba33456cf9d81c79522
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.0 MB (209962270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:902f82b2116fd21d8e7a7eab834541cd4467bc9f4b2531ff4b257dcf8717a3d8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:48:22 GMT
ADD file:3c6dc937cb7b4c81b42126f377d23320ec1d0a8ca34d38e7c45871f1d08dac43 in / 
# Sat, 16 Oct 2021 01:48:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 16 Oct 2021 01:48:23 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:48:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 16 Oct 2021 01:48:25 GMT
CMD ["/bin/bash"]
# Sat, 16 Oct 2021 03:11:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:11:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 03:11:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:12:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:828b35a09f0b2f3d1dead43aa2468ff5eba6c463423b3fff7ee6d150f6fd1b6b`  
		Last Modified: Thu, 05 Aug 2021 00:25:09 GMT  
		Size: 41.2 MB (41239253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238e9b8fdf46981043813ae269c4420735959dd01d4d15c420b66448523e9adc`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5b1b49195905e9415adfe3583301316ef591d794fcfd12b5cd29103fa7ee6b`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269a6c6175ba12a0fd708883c2625167711f111f24ce2bb79221fda132487e57`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77011f0e629af6f1792d3ccf59b89e6c06bb7f9a0f9ff78fee1d59ca55eda175`  
		Last Modified: Sat, 16 Oct 2021 03:24:02 GMT  
		Size: 6.8 MB (6837244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef3e23489d0258d8ea0afeec7d0eac6009020741bdee47ed1cae3fd5a9004fb`  
		Last Modified: Sat, 16 Oct 2021 03:24:19 GMT  
		Size: 39.8 MB (39815288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0884afca89907fa2ac7f34ac68afcbba8e0be0626d1bb3927c23cbd7cdd9c24`  
		Last Modified: Sat, 16 Oct 2021 03:24:47 GMT  
		Size: 122.1 MB (122068992 bytes)  
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
$ docker pull buildpack-deps@sha256:ea5020e4cda81416f5265e6ff8fb336e1a3b70637de0b68241217f64483b2cef
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
$ docker pull buildpack-deps@sha256:d7f4fe08183763a004061ab5bb9663ab2f51bf303b9be25d3a37d46e9bc4c744
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48077990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27605cc34c887f769b55b6bbaf4811f39a6448d2c48146d5c0ff53270d2a50f5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:48:22 GMT
ADD file:3c6dc937cb7b4c81b42126f377d23320ec1d0a8ca34d38e7c45871f1d08dac43 in / 
# Sat, 16 Oct 2021 01:48:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 16 Oct 2021 01:48:23 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:48:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 16 Oct 2021 01:48:25 GMT
CMD ["/bin/bash"]
# Sat, 16 Oct 2021 03:11:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:11:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:828b35a09f0b2f3d1dead43aa2468ff5eba6c463423b3fff7ee6d150f6fd1b6b`  
		Last Modified: Thu, 05 Aug 2021 00:25:09 GMT  
		Size: 41.2 MB (41239253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238e9b8fdf46981043813ae269c4420735959dd01d4d15c420b66448523e9adc`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5b1b49195905e9415adfe3583301316ef591d794fcfd12b5cd29103fa7ee6b`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269a6c6175ba12a0fd708883c2625167711f111f24ce2bb79221fda132487e57`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77011f0e629af6f1792d3ccf59b89e6c06bb7f9a0f9ff78fee1d59ca55eda175`  
		Last Modified: Sat, 16 Oct 2021 03:24:02 GMT  
		Size: 6.8 MB (6837244 bytes)  
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
$ docker pull buildpack-deps@sha256:7eb08b3466cf0830b1b16429f7a16f428f8441163debd766b8ffabcd3cfffac7
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
$ docker pull buildpack-deps@sha256:676194f83bf0884b02998c5e5783ba66882579a02a3da41de3a8180280f8f5d6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.9 MB (87893278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a849f28400387145666eead1018792c030ac71ad4445140201f4e6395aee9178`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:48:22 GMT
ADD file:3c6dc937cb7b4c81b42126f377d23320ec1d0a8ca34d38e7c45871f1d08dac43 in / 
# Sat, 16 Oct 2021 01:48:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 16 Oct 2021 01:48:23 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:48:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 16 Oct 2021 01:48:25 GMT
CMD ["/bin/bash"]
# Sat, 16 Oct 2021 03:11:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:11:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 03:11:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:828b35a09f0b2f3d1dead43aa2468ff5eba6c463423b3fff7ee6d150f6fd1b6b`  
		Last Modified: Thu, 05 Aug 2021 00:25:09 GMT  
		Size: 41.2 MB (41239253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238e9b8fdf46981043813ae269c4420735959dd01d4d15c420b66448523e9adc`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5b1b49195905e9415adfe3583301316ef591d794fcfd12b5cd29103fa7ee6b`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269a6c6175ba12a0fd708883c2625167711f111f24ce2bb79221fda132487e57`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77011f0e629af6f1792d3ccf59b89e6c06bb7f9a0f9ff78fee1d59ca55eda175`  
		Last Modified: Sat, 16 Oct 2021 03:24:02 GMT  
		Size: 6.8 MB (6837244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef3e23489d0258d8ea0afeec7d0eac6009020741bdee47ed1cae3fd5a9004fb`  
		Last Modified: Sat, 16 Oct 2021 03:24:19 GMT  
		Size: 39.8 MB (39815288 bytes)  
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
$ docker pull buildpack-deps@sha256:b2b2faaae9b30af6432903f81f858e6362cede40078ad6b8fc7456e0045c9993
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
$ docker pull buildpack-deps@sha256:19c0527602ef9047ea9af278bd2e7c739b4639471a44a2e9462b14f8b619cec7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.4 MB (205381635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c0fc413befe38312de14b98f4ecb6c76ea42726f0169b3d760775a153ca9434`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:38 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Sat, 16 Oct 2021 01:47:38 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:04:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:04:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 03:05:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:06:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a555366df07c0f7aae069a38b120e5b8e6e95f359b898d0032574413b8b2c1`  
		Last Modified: Sat, 16 Oct 2021 03:19:21 GMT  
		Size: 6.1 MB (6084243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233462b381c92a25d3bf01a6a656557732c43fb811b0b5173d611ac8fd767a94`  
		Last Modified: Sat, 16 Oct 2021 03:19:20 GMT  
		Size: 2.6 MB (2570190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237b11e5d0bf83fb3fb6bdb6b3cfd1967ea6e80fd7bf3b2f3f6167b48ba59cbd`  
		Last Modified: Sat, 16 Oct 2021 03:19:39 GMT  
		Size: 43.3 MB (43277011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f134b5b86813b51223749bd3bdbe427289e06813ec214b870337081a650822`  
		Last Modified: Sat, 16 Oct 2021 03:20:09 GMT  
		Size: 129.7 MB (129722715 bytes)  
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
$ docker pull buildpack-deps@sha256:8fd11f4c0036db05fb68618db00da04b0c79c13f44859c75bb7208f2e1dd64fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.2 MB (246225436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:098c5a0af01f04f9df9faef2c21612259a54295d1e4ac9ab63471dde03939d4c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Oct 2021 11:07:29 GMT
ADD file:fd96554dfb72307c3cf9292c343050a8b9f0848735b7555820f0068914ebd758 in / 
# Tue, 05 Oct 2021 11:07:35 GMT
CMD ["bash"]
# Tue, 05 Oct 2021 14:41:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Oct 2021 14:42:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 05 Oct 2021 14:46:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 05 Oct 2021 14:57:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:db28fc1e594e5598e665c54ac1b7fd602d86dddaf8bb237a72303cec22a9185c`  
		Last Modified: Tue, 05 Oct 2021 11:10:31 GMT  
		Size: 30.4 MB (30432921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb1c3498d7cd3adcb6d716b98adcea053880272423eb1a9939a7426d428cfd8`  
		Last Modified: Tue, 05 Oct 2021 15:46:03 GMT  
		Size: 7.1 MB (7058539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:494fb7e48f3a6cbd76b9eaab065228a859bdd7e6f41a24d6aa2cf74d77d31e73`  
		Last Modified: Tue, 05 Oct 2021 15:45:58 GMT  
		Size: 3.7 MB (3719778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961571b34653877509a0b15ed874ac56391305c5a20707a48fdf723b3becd986`  
		Last Modified: Tue, 05 Oct 2021 15:46:51 GMT  
		Size: 53.7 MB (53722746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e23c150699147a85f182ea8b9a515a5693a4957bd9f3d7a86057372d8888d231`  
		Last Modified: Tue, 05 Oct 2021 15:48:34 GMT  
		Size: 151.3 MB (151291452 bytes)  
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
$ docker pull buildpack-deps@sha256:d910ddef17dc4c1e788ed6f495c671dc76199b485090f1114409077b13ef7d2d
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
$ docker pull buildpack-deps@sha256:b3aa99deddad631d348b89d6c671ec7bd6d1fd898210f07ed15f38b9527174d0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.4 MB (32381909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc96931ce78d81afa20b59e979221712e50c103543abd31b3f45a8d2d4ed29ec`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:38 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Sat, 16 Oct 2021 01:47:38 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:04:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:04:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a555366df07c0f7aae069a38b120e5b8e6e95f359b898d0032574413b8b2c1`  
		Last Modified: Sat, 16 Oct 2021 03:19:21 GMT  
		Size: 6.1 MB (6084243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233462b381c92a25d3bf01a6a656557732c43fb811b0b5173d611ac8fd767a94`  
		Last Modified: Sat, 16 Oct 2021 03:19:20 GMT  
		Size: 2.6 MB (2570190 bytes)  
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
$ docker pull buildpack-deps@sha256:83e8be4ead24277419d0cd40f98276cfb93f497d55128a5c2db9eac556213a4c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41211238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c4951cd140e5db022882ab2a533d8ee9c6728be12eaa2480606c112538681a7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Oct 2021 11:07:29 GMT
ADD file:fd96554dfb72307c3cf9292c343050a8b9f0848735b7555820f0068914ebd758 in / 
# Tue, 05 Oct 2021 11:07:35 GMT
CMD ["bash"]
# Tue, 05 Oct 2021 14:41:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Oct 2021 14:42:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:db28fc1e594e5598e665c54ac1b7fd602d86dddaf8bb237a72303cec22a9185c`  
		Last Modified: Tue, 05 Oct 2021 11:10:31 GMT  
		Size: 30.4 MB (30432921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb1c3498d7cd3adcb6d716b98adcea053880272423eb1a9939a7426d428cfd8`  
		Last Modified: Tue, 05 Oct 2021 15:46:03 GMT  
		Size: 7.1 MB (7058539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:494fb7e48f3a6cbd76b9eaab065228a859bdd7e6f41a24d6aa2cf74d77d31e73`  
		Last Modified: Tue, 05 Oct 2021 15:45:58 GMT  
		Size: 3.7 MB (3719778 bytes)  
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
$ docker pull buildpack-deps@sha256:a161d52291bf8c954c5c827dca5ef294681a85fc96aa37eec6b14d4d093a26dc
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
$ docker pull buildpack-deps@sha256:4cd7d49c2897395988195e6981f71613db7fe5968de61afdf95af231ada24c78
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75658920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5408604964ea4bbf7712a3f19081f5d0aeb3813f010484bb8d592e9dd6603469`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:38 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Sat, 16 Oct 2021 01:47:38 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:04:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:04:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 03:05:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a555366df07c0f7aae069a38b120e5b8e6e95f359b898d0032574413b8b2c1`  
		Last Modified: Sat, 16 Oct 2021 03:19:21 GMT  
		Size: 6.1 MB (6084243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233462b381c92a25d3bf01a6a656557732c43fb811b0b5173d611ac8fd767a94`  
		Last Modified: Sat, 16 Oct 2021 03:19:20 GMT  
		Size: 2.6 MB (2570190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237b11e5d0bf83fb3fb6bdb6b3cfd1967ea6e80fd7bf3b2f3f6167b48ba59cbd`  
		Last Modified: Sat, 16 Oct 2021 03:19:39 GMT  
		Size: 43.3 MB (43277011 bytes)  
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
$ docker pull buildpack-deps@sha256:d4a4d531a63f36ca9d9b778f021e88bedc03615312d12bc138ae8829798e9d40
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.9 MB (94933984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55b74a920f641c6acbe8e3557e6b0420efaa1a94b372cdffb52a99991e04d210`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Oct 2021 11:07:29 GMT
ADD file:fd96554dfb72307c3cf9292c343050a8b9f0848735b7555820f0068914ebd758 in / 
# Tue, 05 Oct 2021 11:07:35 GMT
CMD ["bash"]
# Tue, 05 Oct 2021 14:41:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Oct 2021 14:42:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 05 Oct 2021 14:46:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:db28fc1e594e5598e665c54ac1b7fd602d86dddaf8bb237a72303cec22a9185c`  
		Last Modified: Tue, 05 Oct 2021 11:10:31 GMT  
		Size: 30.4 MB (30432921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb1c3498d7cd3adcb6d716b98adcea053880272423eb1a9939a7426d428cfd8`  
		Last Modified: Tue, 05 Oct 2021 15:46:03 GMT  
		Size: 7.1 MB (7058539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:494fb7e48f3a6cbd76b9eaab065228a859bdd7e6f41a24d6aa2cf74d77d31e73`  
		Last Modified: Tue, 05 Oct 2021 15:45:58 GMT  
		Size: 3.7 MB (3719778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961571b34653877509a0b15ed874ac56391305c5a20707a48fdf723b3becd986`  
		Last Modified: Tue, 05 Oct 2021 15:46:51 GMT  
		Size: 53.7 MB (53722746 bytes)  
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
$ docker pull buildpack-deps@sha256:8046d17468dec05d82ec79681bf1c5e0f43ada1c2efd4222dd9d90023a226bc7
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
$ docker pull buildpack-deps@sha256:704e4e9e47293f392f16e1f74eb96784ee4ec426c416d006295e71856e550a9d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.8 MB (241796219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:701bdfc5b1f5072d2996e2f7a86ffd244192c9c42231d090abb7b8c44734cb03`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:43:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:43:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 01:44:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:47:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d2365e1e08bb86c1668a76475087cb6db5b42ba70cff99e936b0dda67d9215`  
		Last Modified: Sat, 16 Oct 2021 01:54:19 GMT  
		Size: 7.8 MB (7774998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577c425bc29205ed0c522c9332f7199d4e5805576b76cfa97ff9e345cdb268a5`  
		Last Modified: Sat, 16 Oct 2021 01:54:18 GMT  
		Size: 3.6 MB (3624513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fcda6c22ed5cb34aaea71f2bd9622535b40c91c4f8cc26f304720b510f9a6f`  
		Last Modified: Sat, 16 Oct 2021 01:54:38 GMT  
		Size: 60.7 MB (60722104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91046370e281131f8cd808e9fd0ec37c4f175001570c9196d54443154f9eaaa5`  
		Last Modified: Sat, 16 Oct 2021 01:55:07 GMT  
		Size: 141.1 MB (141107503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:4215ea236dbf14f9f94442857a9d9345f2fff063927f027cb9c724e78f76e6d5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.2 MB (207220779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78ce8d17eb298ae091fe14706ba52064dee049eb0d9a6f40dc060768396b945f`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:12:00 GMT
ADD file:625e3906181f4bd86e59a0e9748f67fcb1391a2e65e36c729e71353381a49757 in / 
# Sat, 16 Oct 2021 01:12:00 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:52:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:52:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 02:53:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:55:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8795d4da4abd6abcafe7285749aa85d3a164999e84720a3845f764e56e306771`  
		Last Modified: Sat, 16 Oct 2021 01:15:01 GMT  
		Size: 24.1 MB (24064451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a23aff9df2cf391d11feae54be8e82799a837823112a6dac845d32dc72eca02`  
		Last Modified: Sat, 16 Oct 2021 03:04:40 GMT  
		Size: 6.8 MB (6770106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce73020529e5c4c05a06cf469c45636d454253e819779803de574708312ec61`  
		Last Modified: Sat, 16 Oct 2021 03:04:37 GMT  
		Size: 3.1 MB (3104081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9998d3d2297827b1708a84f36e166391af9aecaafd91bf2d67b2dff8b1ad8a`  
		Last Modified: Sat, 16 Oct 2021 03:05:32 GMT  
		Size: 55.5 MB (55453746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fee38c0bd1ce11408a904c46f60d7de2595b0cda7b99bcbf74c2b5994bb1fad`  
		Last Modified: Sat, 16 Oct 2021 03:06:56 GMT  
		Size: 117.8 MB (117828395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a1b289eb033907eb4c99d514e204e8144577faee1302fed2fd86915bd0fa0c70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.5 MB (231499713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13278dccc5e41ca5c8bb7391753d4dd6554de1ad70743b7ca632257ea042f26f`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:06:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:06:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 03:06:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:07:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d32ba945c264e68ad0217898b4deb849a7b2b26d5877601d63d4545e29806e8`  
		Last Modified: Sat, 16 Oct 2021 03:20:27 GMT  
		Size: 7.6 MB (7639827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8491af4d3a3f4c7eace39c71ad3060a1909e99874d90b33647db45e9ce4482fa`  
		Last Modified: Sat, 16 Oct 2021 03:20:21 GMT  
		Size: 3.4 MB (3386522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cfb326f9da9ecc7f75c6f18d8aad46bf48677fba9bfb90d7d598271ee287959`  
		Last Modified: Sat, 16 Oct 2021 03:20:47 GMT  
		Size: 60.8 MB (60775123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dcedfdcd571b25c3f063cf324a265be0fbcf93e8208e31ccacb40a358cd4e11`  
		Last Modified: Sat, 16 Oct 2021 03:21:18 GMT  
		Size: 132.5 MB (132527341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:982eea1c9873499f87ffadcd10757d03ad62c3da04c72580d5ccff88fdfdfbca
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.4 MB (265361410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9424c0457501b56ce0517f9c6cca49b325fa99cc3f8c8d59fed4db28749bfba`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:36:38 GMT
ADD file:9246bf887411af1b286de95d779c11581dcef3c0d5a29e434162f0c085a7ce85 in / 
# Sat, 16 Oct 2021 00:36:44 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:08:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:09:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 01:11:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:17:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:77ba7971d651af68e20e7cbb6603a3f7acd8ef2893066767a93db104723556f2`  
		Last Modified: Sat, 16 Oct 2021 00:38:38 GMT  
		Size: 33.3 MB (33287238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b70bd5d2bc58b580d50736dbb70b528bdcd2910275584c8774c52efd29b8838`  
		Last Modified: Sat, 16 Oct 2021 01:29:38 GMT  
		Size: 8.7 MB (8728083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5e49a7fcde36f5b4cd0c87bace3ad307d0709d6942ff3ec27c5090922c1c7c`  
		Last Modified: Sat, 16 Oct 2021 01:29:16 GMT  
		Size: 4.5 MB (4456437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9332a33dc6df6ad95548ba3915b3a1235486dee9aacc7d13206604539866d440`  
		Last Modified: Sat, 16 Oct 2021 01:30:25 GMT  
		Size: 69.4 MB (69387759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b303db83d7ca2e64579e38fcb0676cf4f073f2f7a2f91e3088057f0b1a20a7`  
		Last Modified: Sat, 16 Oct 2021 01:31:04 GMT  
		Size: 149.5 MB (149501893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:451b83fcf3e41a5ee8bb7eabced23808496c11485d512282551948f7fa4f73b1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.6 MB (222629035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4bd65308571622b527359b75449d6e2a2a52e1563b6b374998b2462690dee78`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:41:46 GMT
ADD file:cf3b6f9c395392eaf2c629969f59c48cde60ae1c74c3dbb13886481999a7a4d5 in / 
# Sat, 16 Oct 2021 00:41:48 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:09:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:09:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 01:10:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:10:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1f0267805ccac7499fadaabf65e52d4564add2bc20ed25bcf77df24d8debb103`  
		Last Modified: Sat, 16 Oct 2021 00:42:57 GMT  
		Size: 27.1 MB (27120856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe453f45d32c58639c70b42127d12e8467533bc152ff663c5ffc8d0b5407293`  
		Last Modified: Sat, 16 Oct 2021 01:15:04 GMT  
		Size: 7.4 MB (7428503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df987c93c7f716b8ea845b480a00ccf4e4d962df89ed9f8cbefecdb1d9a96cf2`  
		Last Modified: Sat, 16 Oct 2021 01:15:03 GMT  
		Size: 3.5 MB (3542069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb4bb9db0d64c1d22f8065532581f6cdd28f20b4360950d6c5c3741db428c4f`  
		Last Modified: Sat, 16 Oct 2021 01:15:19 GMT  
		Size: 60.0 MB (60019955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07117226d68472223964833e6e866764854828a538fdf2ceb27bb6a66fd9fca5`  
		Last Modified: Sat, 16 Oct 2021 01:15:41 GMT  
		Size: 124.5 MB (124517652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:20.04-curl`

```console
$ docker pull buildpack-deps@sha256:47084e6d055f10f777634a540c0ec891300768a8fc014ee86e38ad8a961bafa2
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
$ docker pull buildpack-deps@sha256:b1bb273927172a3307daf2e435ad3eaedac707b52aed1a80a6559b5045aa918b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.0 MB (39966612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:699ca4594065556769c48f4df863439f7854e2dc3d247de1ca0ef27c44f306fd`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:43:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:43:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d2365e1e08bb86c1668a76475087cb6db5b42ba70cff99e936b0dda67d9215`  
		Last Modified: Sat, 16 Oct 2021 01:54:19 GMT  
		Size: 7.8 MB (7774998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577c425bc29205ed0c522c9332f7199d4e5805576b76cfa97ff9e345cdb268a5`  
		Last Modified: Sat, 16 Oct 2021 01:54:18 GMT  
		Size: 3.6 MB (3624513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:5ac106cdf6e5b13b0618a85b4eed39d1b3ddee354c7bf1ba5da0f0554c9a9b9b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33938638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4e7f6efd6008f76b37ff18082e23ab310aac81c1e795dec85a64e7fe4f5f7cf`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:12:00 GMT
ADD file:625e3906181f4bd86e59a0e9748f67fcb1391a2e65e36c729e71353381a49757 in / 
# Sat, 16 Oct 2021 01:12:00 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:52:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:52:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8795d4da4abd6abcafe7285749aa85d3a164999e84720a3845f764e56e306771`  
		Last Modified: Sat, 16 Oct 2021 01:15:01 GMT  
		Size: 24.1 MB (24064451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a23aff9df2cf391d11feae54be8e82799a837823112a6dac845d32dc72eca02`  
		Last Modified: Sat, 16 Oct 2021 03:04:40 GMT  
		Size: 6.8 MB (6770106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce73020529e5c4c05a06cf469c45636d454253e819779803de574708312ec61`  
		Last Modified: Sat, 16 Oct 2021 03:04:37 GMT  
		Size: 3.1 MB (3104081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:5ab6253594e45232ef897f4704055eea3babf20a475e9747ce10766d44c4fdc6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38197249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:369dd1ca9197a48ea1f1e4db32de5c2bebef7886c4477c290b342f8f85be72d8`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:06:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:06:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d32ba945c264e68ad0217898b4deb849a7b2b26d5877601d63d4545e29806e8`  
		Last Modified: Sat, 16 Oct 2021 03:20:27 GMT  
		Size: 7.6 MB (7639827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8491af4d3a3f4c7eace39c71ad3060a1909e99874d90b33647db45e9ce4482fa`  
		Last Modified: Sat, 16 Oct 2021 03:20:21 GMT  
		Size: 3.4 MB (3386522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:eef3c0a41f6cfc83f7c300350cc0da51c3d3185a17d758edbcdc8b4e2b6c3ccf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46471758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44c8645449e8182a2157126f6b3219cb1ec8436d8919a30c6ef1e8eff0cf511c`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:36:38 GMT
ADD file:9246bf887411af1b286de95d779c11581dcef3c0d5a29e434162f0c085a7ce85 in / 
# Sat, 16 Oct 2021 00:36:44 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:08:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:09:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:77ba7971d651af68e20e7cbb6603a3f7acd8ef2893066767a93db104723556f2`  
		Last Modified: Sat, 16 Oct 2021 00:38:38 GMT  
		Size: 33.3 MB (33287238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b70bd5d2bc58b580d50736dbb70b528bdcd2910275584c8774c52efd29b8838`  
		Last Modified: Sat, 16 Oct 2021 01:29:38 GMT  
		Size: 8.7 MB (8728083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5e49a7fcde36f5b4cd0c87bace3ad307d0709d6942ff3ec27c5090922c1c7c`  
		Last Modified: Sat, 16 Oct 2021 01:29:16 GMT  
		Size: 4.5 MB (4456437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:8102a47411513107d38819cf1c50c53a59b006b8758ef1760d08cf6ef9189d53
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34121525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81fb5dedcf54f0770eebdd37611586bf30053249c901ae7232aa30b16ab13d82`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:14:21 GMT
ADD file:9e85e474b240689ee9bae50d5101df1d6128c335d61a8010cd69202f778a773f in / 
# Sat, 16 Oct 2021 00:14:22 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 00:55:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 00:56:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:828cfd0a7a30e2a8cf76cca67b8314a0738943c0ea83f167ea5b8bd084c19324`  
		Last Modified: Sat, 16 Oct 2021 00:27:58 GMT  
		Size: 24.2 MB (24226165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0acf80d7193afc4761abdd46a164fd3130cfdb676ff3801645cb819e88404dad`  
		Last Modified: Sat, 16 Oct 2021 01:28:59 GMT  
		Size: 6.8 MB (6750726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab037bb968a07aace1a589724d7eb8ec30de3a596a4227fa9fc39de318067cb`  
		Last Modified: Sat, 16 Oct 2021 01:28:54 GMT  
		Size: 3.1 MB (3144634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:df2267e8f1ad540996bba096ece6a0ac191843ccd329f8acea0b78f977e3433f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.1 MB (38091428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f3fe3fc44fce5558d3d6596b6c1c62d958ff8a740b249bcb858c65f15c905f7`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:41:46 GMT
ADD file:cf3b6f9c395392eaf2c629969f59c48cde60ae1c74c3dbb13886481999a7a4d5 in / 
# Sat, 16 Oct 2021 00:41:48 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:09:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:09:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1f0267805ccac7499fadaabf65e52d4564add2bc20ed25bcf77df24d8debb103`  
		Last Modified: Sat, 16 Oct 2021 00:42:57 GMT  
		Size: 27.1 MB (27120856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe453f45d32c58639c70b42127d12e8467533bc152ff663c5ffc8d0b5407293`  
		Last Modified: Sat, 16 Oct 2021 01:15:04 GMT  
		Size: 7.4 MB (7428503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df987c93c7f716b8ea845b480a00ccf4e4d962df89ed9f8cbefecdb1d9a96cf2`  
		Last Modified: Sat, 16 Oct 2021 01:15:03 GMT  
		Size: 3.5 MB (3542069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:20.04-scm`

```console
$ docker pull buildpack-deps@sha256:222ddf4dba302cca6ac700a276e8bb278ce853044531129cb2fccec37d3f622d
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
$ docker pull buildpack-deps@sha256:db28fe2833804601492020af431060420b8ff94b84c08e332edff1754ca43cc7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.7 MB (100688716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfe4a06be9ec9a6f2ed84a88ec5a2efd03025dfebdadaa46558c9a8ae2086f1f`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:43:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:43:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 01:44:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d2365e1e08bb86c1668a76475087cb6db5b42ba70cff99e936b0dda67d9215`  
		Last Modified: Sat, 16 Oct 2021 01:54:19 GMT  
		Size: 7.8 MB (7774998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577c425bc29205ed0c522c9332f7199d4e5805576b76cfa97ff9e345cdb268a5`  
		Last Modified: Sat, 16 Oct 2021 01:54:18 GMT  
		Size: 3.6 MB (3624513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fcda6c22ed5cb34aaea71f2bd9622535b40c91c4f8cc26f304720b510f9a6f`  
		Last Modified: Sat, 16 Oct 2021 01:54:38 GMT  
		Size: 60.7 MB (60722104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:c9f054bee4df38a6541850b189dbf384ed8fbaa5db4819a2ebc183f1f8e40d48
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.4 MB (89392384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8f483864653a58be09108cba02450a5d4f63047b5b1a94b83f052739ad0dbb2`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:12:00 GMT
ADD file:625e3906181f4bd86e59a0e9748f67fcb1391a2e65e36c729e71353381a49757 in / 
# Sat, 16 Oct 2021 01:12:00 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:52:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:52:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 02:53:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8795d4da4abd6abcafe7285749aa85d3a164999e84720a3845f764e56e306771`  
		Last Modified: Sat, 16 Oct 2021 01:15:01 GMT  
		Size: 24.1 MB (24064451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a23aff9df2cf391d11feae54be8e82799a837823112a6dac845d32dc72eca02`  
		Last Modified: Sat, 16 Oct 2021 03:04:40 GMT  
		Size: 6.8 MB (6770106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce73020529e5c4c05a06cf469c45636d454253e819779803de574708312ec61`  
		Last Modified: Sat, 16 Oct 2021 03:04:37 GMT  
		Size: 3.1 MB (3104081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9998d3d2297827b1708a84f36e166391af9aecaafd91bf2d67b2dff8b1ad8a`  
		Last Modified: Sat, 16 Oct 2021 03:05:32 GMT  
		Size: 55.5 MB (55453746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f2c785f3366e906ddfb3628fc19d27edf4085e718b958ee51da3f053cc4fb963
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.0 MB (98972372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28368350ce887feb38c7efd949a238df59747b3b785649046168c4a048339e0e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:06:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:06:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 03:06:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d32ba945c264e68ad0217898b4deb849a7b2b26d5877601d63d4545e29806e8`  
		Last Modified: Sat, 16 Oct 2021 03:20:27 GMT  
		Size: 7.6 MB (7639827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8491af4d3a3f4c7eace39c71ad3060a1909e99874d90b33647db45e9ce4482fa`  
		Last Modified: Sat, 16 Oct 2021 03:20:21 GMT  
		Size: 3.4 MB (3386522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cfb326f9da9ecc7f75c6f18d8aad46bf48677fba9bfb90d7d598271ee287959`  
		Last Modified: Sat, 16 Oct 2021 03:20:47 GMT  
		Size: 60.8 MB (60775123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:326e4176f66a5c4be1ac29828e60f739348b5ba008dc4e2361c427756faa6b02
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115859517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0326065a3f294abcae80a83eedf20dd7b4d76df25a85d8bea0e01f32bc0a25f`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:36:38 GMT
ADD file:9246bf887411af1b286de95d779c11581dcef3c0d5a29e434162f0c085a7ce85 in / 
# Sat, 16 Oct 2021 00:36:44 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:08:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:09:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 01:11:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:77ba7971d651af68e20e7cbb6603a3f7acd8ef2893066767a93db104723556f2`  
		Last Modified: Sat, 16 Oct 2021 00:38:38 GMT  
		Size: 33.3 MB (33287238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b70bd5d2bc58b580d50736dbb70b528bdcd2910275584c8774c52efd29b8838`  
		Last Modified: Sat, 16 Oct 2021 01:29:38 GMT  
		Size: 8.7 MB (8728083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5e49a7fcde36f5b4cd0c87bace3ad307d0709d6942ff3ec27c5090922c1c7c`  
		Last Modified: Sat, 16 Oct 2021 01:29:16 GMT  
		Size: 4.5 MB (4456437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9332a33dc6df6ad95548ba3915b3a1235486dee9aacc7d13206604539866d440`  
		Last Modified: Sat, 16 Oct 2021 01:30:25 GMT  
		Size: 69.4 MB (69387759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:32c03e9661aebe7ea0b551909060f7933d21dd26b8cff2f9bba539d35c920b95
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.1 MB (98111383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7382cfde4760dcd8d917da671f1af5eea2423bdf29123e3d98f7cab60e90a4b4`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:41:46 GMT
ADD file:cf3b6f9c395392eaf2c629969f59c48cde60ae1c74c3dbb13886481999a7a4d5 in / 
# Sat, 16 Oct 2021 00:41:48 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:09:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:09:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 01:10:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1f0267805ccac7499fadaabf65e52d4564add2bc20ed25bcf77df24d8debb103`  
		Last Modified: Sat, 16 Oct 2021 00:42:57 GMT  
		Size: 27.1 MB (27120856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe453f45d32c58639c70b42127d12e8467533bc152ff663c5ffc8d0b5407293`  
		Last Modified: Sat, 16 Oct 2021 01:15:04 GMT  
		Size: 7.4 MB (7428503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df987c93c7f716b8ea845b480a00ccf4e4d962df89ed9f8cbefecdb1d9a96cf2`  
		Last Modified: Sat, 16 Oct 2021 01:15:03 GMT  
		Size: 3.5 MB (3542069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb4bb9db0d64c1d22f8065532581f6cdd28f20b4360950d6c5c3741db428c4f`  
		Last Modified: Sat, 16 Oct 2021 01:15:19 GMT  
		Size: 60.0 MB (60019955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:21.04`

```console
$ docker pull buildpack-deps@sha256:fd87af8c01206a890d8a97ab52da179dea62346dce07ca6b17b6bf4ffc642fc4
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
$ docker pull buildpack-deps@sha256:c2750d7d73f27c54b134f3afc5eff402d4d023a0f6610a2c14745f0778db55dd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.2 MB (239175401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97986f6e0169d2fcb6b4bb73a55fb278d78a9387cb1c6ef37f4415ed04d15ae4`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:53 GMT
ADD file:36081e580b6851b0f8a1176a307b99a673510dc87809a726cad514bd7f56d620 in / 
# Sat, 16 Oct 2021 01:47:53 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:08:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:08:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 03:08:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:09:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e61beefb4313333ca27a602845cbf2a6f7cba9c176bb999f14a4bdcfb6a54148`  
		Last Modified: Fri, 01 Oct 2021 02:46:09 GMT  
		Size: 30.2 MB (30174163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b2d75872cf44ae1d0e91f4b4298e3d382c845eefa7655b7f2325a88f17c9ad`  
		Last Modified: Sat, 16 Oct 2021 03:21:30 GMT  
		Size: 5.4 MB (5404762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8704bb2e0710d7b555bb044b098f06225f5697ad2878a8f1ae2ac285a3ed825e`  
		Last Modified: Sat, 16 Oct 2021 03:21:29 GMT  
		Size: 3.4 MB (3431928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f566ac9ad20f04707fbf26b5de866cd237d21a3c927fb1f30fe6b94f57040fba`  
		Last Modified: Sat, 16 Oct 2021 03:21:48 GMT  
		Size: 43.5 MB (43533098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5573408c4e367ec83c2be39c8e053c34e050ace99c62306c55a15ac0d0cc10c9`  
		Last Modified: Sat, 16 Oct 2021 03:22:21 GMT  
		Size: 156.6 MB (156631450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.04` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:2907a4ade782540beeadc530701ec593f2c1899d1f9ffc71d51962b7a8bf45be
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.1 MB (268143719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:689afc563871e8f713e32f83998d679743c14ac849d1e7a4e979dd31bb349631`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Oct 2021 11:08:18 GMT
ADD file:4fece2b915970b36002bf98a6f85f91c3b9bfeb80b685f7e5ee749080aea6540 in / 
# Tue, 05 Oct 2021 11:08:25 GMT
CMD ["bash"]
# Tue, 05 Oct 2021 15:11:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Oct 2021 15:12:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 05 Oct 2021 15:14:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 05 Oct 2021 15:22:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b16b9756d17acd6ced37d43568054b32fcebdd38ee4b9bdbf35dbc3e872d754d`  
		Last Modified: Tue, 05 Oct 2021 11:11:17 GMT  
		Size: 37.3 MB (37255452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a54cbd41484567ce0ebb693b3129bf830d0e454fbe8a0eec180d9fa9f976c0`  
		Last Modified: Tue, 05 Oct 2021 15:51:52 GMT  
		Size: 6.2 MB (6153990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afff0eec9aba68bd0b14d67496cf23585cea9e37314ecee6657b63816efcd9db`  
		Last Modified: Tue, 05 Oct 2021 15:51:49 GMT  
		Size: 4.5 MB (4523714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1536544f6a113307ef8771dc9e57d3b4974edc1869ee7d08a83f9422c79b1be`  
		Last Modified: Tue, 05 Oct 2021 15:52:37 GMT  
		Size: 49.5 MB (49467145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67a0bc2994fab6d2773059eb5766490eff6f06d4c5cead29d091d284b24873a`  
		Last Modified: Tue, 05 Oct 2021 15:54:11 GMT  
		Size: 170.7 MB (170743418 bytes)  
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
$ docker pull buildpack-deps@sha256:d8a6f33c53c107583b08147895c892edb834472807431b73571086744ca130db
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
$ docker pull buildpack-deps@sha256:39cb123dafa0028e4cb1095811c94c4a5de7a1769165a1e07d3a129988c951cf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (39010853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:239585f43a663f2752dc848bcfe0c2281cc48b9574e96d0d559cd42d54082ec2`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:53 GMT
ADD file:36081e580b6851b0f8a1176a307b99a673510dc87809a726cad514bd7f56d620 in / 
# Sat, 16 Oct 2021 01:47:53 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:08:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:08:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e61beefb4313333ca27a602845cbf2a6f7cba9c176bb999f14a4bdcfb6a54148`  
		Last Modified: Fri, 01 Oct 2021 02:46:09 GMT  
		Size: 30.2 MB (30174163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b2d75872cf44ae1d0e91f4b4298e3d382c845eefa7655b7f2325a88f17c9ad`  
		Last Modified: Sat, 16 Oct 2021 03:21:30 GMT  
		Size: 5.4 MB (5404762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8704bb2e0710d7b555bb044b098f06225f5697ad2878a8f1ae2ac285a3ed825e`  
		Last Modified: Sat, 16 Oct 2021 03:21:29 GMT  
		Size: 3.4 MB (3431928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.04-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:dd7f2c04edf3b324b852e429bfe162038e616ee28cac5ee5ce6fc9a36381c60f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47933156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:822a0098d55d4ee7d2286bdcb40edb8f012ba6f0fd689db8d6f09bda568dcc23`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Oct 2021 11:08:18 GMT
ADD file:4fece2b915970b36002bf98a6f85f91c3b9bfeb80b685f7e5ee749080aea6540 in / 
# Tue, 05 Oct 2021 11:08:25 GMT
CMD ["bash"]
# Tue, 05 Oct 2021 15:11:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Oct 2021 15:12:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b16b9756d17acd6ced37d43568054b32fcebdd38ee4b9bdbf35dbc3e872d754d`  
		Last Modified: Tue, 05 Oct 2021 11:11:17 GMT  
		Size: 37.3 MB (37255452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a54cbd41484567ce0ebb693b3129bf830d0e454fbe8a0eec180d9fa9f976c0`  
		Last Modified: Tue, 05 Oct 2021 15:51:52 GMT  
		Size: 6.2 MB (6153990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afff0eec9aba68bd0b14d67496cf23585cea9e37314ecee6657b63816efcd9db`  
		Last Modified: Tue, 05 Oct 2021 15:51:49 GMT  
		Size: 4.5 MB (4523714 bytes)  
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
$ docker pull buildpack-deps@sha256:c5defad7da7db30278b0750495097c0f2604d95701ffe4929ec0f7bcb8472a54
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
$ docker pull buildpack-deps@sha256:cb73476030b9b04ac7bb532dbfcd1ccad95222afd48d09abb5c4bfd8fe5e08c2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.5 MB (82543951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ac4d3b843ffa7164875abf17bfc13bd90748f10af8f0e6463fa5b18e52c79aa`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:53 GMT
ADD file:36081e580b6851b0f8a1176a307b99a673510dc87809a726cad514bd7f56d620 in / 
# Sat, 16 Oct 2021 01:47:53 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:08:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:08:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 03:08:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e61beefb4313333ca27a602845cbf2a6f7cba9c176bb999f14a4bdcfb6a54148`  
		Last Modified: Fri, 01 Oct 2021 02:46:09 GMT  
		Size: 30.2 MB (30174163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b2d75872cf44ae1d0e91f4b4298e3d382c845eefa7655b7f2325a88f17c9ad`  
		Last Modified: Sat, 16 Oct 2021 03:21:30 GMT  
		Size: 5.4 MB (5404762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8704bb2e0710d7b555bb044b098f06225f5697ad2878a8f1ae2ac285a3ed825e`  
		Last Modified: Sat, 16 Oct 2021 03:21:29 GMT  
		Size: 3.4 MB (3431928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f566ac9ad20f04707fbf26b5de866cd237d21a3c927fb1f30fe6b94f57040fba`  
		Last Modified: Sat, 16 Oct 2021 03:21:48 GMT  
		Size: 43.5 MB (43533098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.04-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:5b05bc413334c5377efe162a3f3ae34d56e16ea1da1e9806a8f9ddb8761778b3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.4 MB (97400301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bedde56204ff854faef6c52b62b435c3721bf587ac4719e9cbcc069e0ae5509a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Oct 2021 11:08:18 GMT
ADD file:4fece2b915970b36002bf98a6f85f91c3b9bfeb80b685f7e5ee749080aea6540 in / 
# Tue, 05 Oct 2021 11:08:25 GMT
CMD ["bash"]
# Tue, 05 Oct 2021 15:11:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Oct 2021 15:12:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 05 Oct 2021 15:14:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b16b9756d17acd6ced37d43568054b32fcebdd38ee4b9bdbf35dbc3e872d754d`  
		Last Modified: Tue, 05 Oct 2021 11:11:17 GMT  
		Size: 37.3 MB (37255452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a54cbd41484567ce0ebb693b3129bf830d0e454fbe8a0eec180d9fa9f976c0`  
		Last Modified: Tue, 05 Oct 2021 15:51:52 GMT  
		Size: 6.2 MB (6153990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afff0eec9aba68bd0b14d67496cf23585cea9e37314ecee6657b63816efcd9db`  
		Last Modified: Tue, 05 Oct 2021 15:51:49 GMT  
		Size: 4.5 MB (4523714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1536544f6a113307ef8771dc9e57d3b4974edc1869ee7d08a83f9422c79b1be`  
		Last Modified: Tue, 05 Oct 2021 15:52:37 GMT  
		Size: 49.5 MB (49467145 bytes)  
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
$ docker pull buildpack-deps@sha256:77d030141c1f974e8db2be4253d5f44be3222edfb94ca070c9a9bb4a603aeab2
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
$ docker pull buildpack-deps@sha256:84a1afe105bf52f9c41e8cd4b90eb1195d77281c54124d3bf89340527b1b2b2a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **406.7 MB (406684539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b9ef5692961b31df2550467196c52c2fea87a56286e0309e94001e75d07341c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Nov 2021 22:20:34 GMT
ADD file:c061cabbaa10b98eed8dcea770d97000a2861c407f5208a0327bef2b38a99fee in / 
# Thu, 04 Nov 2021 22:20:35 GMT
CMD ["bash"]
# Thu, 04 Nov 2021 22:56:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Nov 2021 22:57:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 04 Nov 2021 22:57:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 04 Nov 2021 23:01:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ae6e1b672be676522e8af69609544dd00b8517e394592a58194383b26e9b54c5`  
		Last Modified: Thu, 04 Nov 2021 22:21:31 GMT  
		Size: 30.4 MB (30378721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4488401b75c6ec432177829c795e1ec36857d568171ae1f197c2c24a9b7e7d8d`  
		Last Modified: Thu, 04 Nov 2021 23:03:09 GMT  
		Size: 3.7 MB (3693784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb8a4e0bca131c5b9e451c10a345a0a13be03cf5ac1220cdc85f170d17be763`  
		Last Modified: Thu, 04 Nov 2021 23:03:09 GMT  
		Size: 3.6 MB (3551867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:538adb79b719e15749a81b037e806769f285f50a60ca3418546e00ffb465a44f`  
		Last Modified: Thu, 04 Nov 2021 23:03:25 GMT  
		Size: 38.1 MB (38080223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d21bd11602fc3dd3a497fb9e548f63e527ab6ddf6d1a69ff6fc0e2a99f0591cc`  
		Last Modified: Thu, 04 Nov 2021 23:04:17 GMT  
		Size: 331.0 MB (330979944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.10` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:5e98f132603710520315c5f3c095c64779984ffe325463ef0f000d6c0f05b8f3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **371.1 MB (371071262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b7162038a1509bbaf31446b9e31729058b627dd8218ae0ff632d356e7488d25`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Nov 2021 22:31:15 GMT
ADD file:675ad5623adf2dafceb59e4a67c75ca26f664127c76fe61c1903cc85d16b9abb in / 
# Thu, 04 Nov 2021 22:31:16 GMT
CMD ["bash"]
# Thu, 04 Nov 2021 23:28:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Nov 2021 23:28:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 04 Nov 2021 23:29:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 04 Nov 2021 23:31:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f7dc858b30797c13a0706f9660d1290ae625ab3436fd5db984b0dac888ad9c8f`  
		Last Modified: Thu, 04 Nov 2021 22:34:32 GMT  
		Size: 26.9 MB (26917157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64923825f2b20992e031b3992dc8c85722c1421e18d7f0fd69532d01d31c2617`  
		Last Modified: Thu, 04 Nov 2021 23:37:31 GMT  
		Size: 3.4 MB (3443243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d36d145711f3ed07bdbf6134addb14e00b663cb32b4de67ff1674023832998`  
		Last Modified: Thu, 04 Nov 2021 23:37:30 GMT  
		Size: 3.7 MB (3742795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:016df4abc6b88c7564811d0545d3f7eeb911db620be98dce64597a05cd3747b7`  
		Last Modified: Thu, 04 Nov 2021 23:38:12 GMT  
		Size: 40.3 MB (40283870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529c6ecc92223423b997a4417f4c58eb16c9fab9a7e390ec178d925ea6721a52`  
		Last Modified: Thu, 04 Nov 2021 23:41:13 GMT  
		Size: 296.7 MB (296684197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.10` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c1478864379e7b484a8b644142cf4bdc8ba8ed80d282f48d9afda3341c9e8e61
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **399.3 MB (399325584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fdeb12cec56afc17f5f9e972ca22732876e8017aa4748442741c17e97bdfff2`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Nov 2021 21:55:45 GMT
ADD file:1b42b91df70bf5eb9529802354c8c97bb9ba991a7885a3fdd4ad5be4b662b70c in / 
# Thu, 04 Nov 2021 21:55:46 GMT
CMD ["bash"]
# Thu, 04 Nov 2021 22:28:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Nov 2021 22:29:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 04 Nov 2021 22:29:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 04 Nov 2021 22:30:32 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:07806c11d5adbc5d83daf2661f72147213f9056f681e452180dc14d81e368e17`  
		Last Modified: Thu, 04 Nov 2021 21:57:10 GMT  
		Size: 29.0 MB (29026100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a952a5c90bcb8e3a8ab1bd7854d8265e7fcb3cb0c0f417fb5722e8f3e0972208`  
		Last Modified: Thu, 04 Nov 2021 22:33:00 GMT  
		Size: 3.7 MB (3678628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cca9702f2a91f991f023bbb9b582e71befe4781bbaa74653b2458540b02c0e3`  
		Last Modified: Thu, 04 Nov 2021 22:32:59 GMT  
		Size: 3.3 MB (3327135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e1d1ea4e9af80ec48e6e5d034e77b64b8de00080ef82b379213f41b1da18b1`  
		Last Modified: Thu, 04 Nov 2021 22:33:17 GMT  
		Size: 38.0 MB (38032438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4b5048b8e4f553fd6380ef6399e0445920029686713f8c2cd8352c0b9164f5`  
		Last Modified: Thu, 04 Nov 2021 22:34:11 GMT  
		Size: 325.3 MB (325261283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.10` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:76524c8f33ad061c15feccd1916806689b3a3e14fc3715b09551725cba103641
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **414.3 MB (414270146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ec6e7f58a8e01be4d11e700d402ed21f4ce524da513527acb10feedfde15d94`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Nov 2021 23:51:29 GMT
ADD file:dc4e5dbd5333b274b2af1c57862eeb96c4b2eda9e8d1a5b766b4ff2aa242106f in / 
# Thu, 04 Nov 2021 23:51:35 GMT
CMD ["bash"]
# Fri, 05 Nov 2021 01:51:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 05 Nov 2021 01:51:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 05 Nov 2021 01:53:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 05 Nov 2021 01:58:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6fb8a15f7529caac80795ba7b74d3c07d163030311fab31ef7b9eda5d4612190`  
		Last Modified: Thu, 04 Nov 2021 23:53:39 GMT  
		Size: 36.2 MB (36174155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a811f8d539d495275857666e419e2349b4afd49b9e35684be52fa958a9edfc64`  
		Last Modified: Fri, 05 Nov 2021 02:01:11 GMT  
		Size: 4.1 MB (4146837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567f57d31cc6184d7de4f38b999b49a84d09a99cd73ecff5fc148f918d7a9f85`  
		Last Modified: Fri, 05 Nov 2021 02:01:11 GMT  
		Size: 4.2 MB (4242137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cfc0512fc4cbeb0f1888bd931fc2dbf9f49bc00278d9c2c5b7aa5272e519c1d`  
		Last Modified: Fri, 05 Nov 2021 02:01:31 GMT  
		Size: 42.7 MB (42707492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19cb8a7b5b5cfa913819716cdb765f5c157cba26b78fb1a9340991522e5bcbf8`  
		Last Modified: Fri, 05 Nov 2021 02:02:41 GMT  
		Size: 327.0 MB (326999525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.10` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:c6b355aa926760c8c218c7917ffa5fafedd30aa73f458aeec83f31cb551ba17c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.3 MB (266339613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee9a89d94c7b91730d83f4ec86752690d6a9704d313cfd4219e4c1c64d783e7d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 11 Nov 2021 01:34:25 GMT
ADD file:def88534019c26953298b38d1af30a296db3d6995d6c801bc98407de70a9e1a6 in / 
# Thu, 11 Nov 2021 01:34:26 GMT
CMD ["bash"]
# Thu, 11 Nov 2021 06:26:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 11 Nov 2021 06:27:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 11 Nov 2021 06:30:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 11 Nov 2021 06:36:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c236a68e6fcd6aac214c2851f12d0e004328b6cc65c84adea73ec2c8eccd27b8`  
		Last Modified: Thu, 11 Nov 2021 01:50:51 GMT  
		Size: 27.2 MB (27206693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32c0816a844c3da682a583d08b1d066cbf7fdaff37ecc1ffe756a1762b5116e`  
		Last Modified: Thu, 11 Nov 2021 06:54:43 GMT  
		Size: 3.5 MB (3490272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd32937a18c0c808ff182ae5991f2dcc6394079d138e4d6880d9013b9e5998a`  
		Last Modified: Thu, 11 Nov 2021 06:54:41 GMT  
		Size: 3.8 MB (3803776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20817c240d9af80288c0d7e22536e4e16be4622339e8522790aa1ddd56e8fd08`  
		Last Modified: Thu, 11 Nov 2021 06:56:39 GMT  
		Size: 40.8 MB (40763475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5caf44e6024c1f0dfa79f670bd50de448af089f51a535f18b001656877b49265`  
		Last Modified: Thu, 11 Nov 2021 07:02:24 GMT  
		Size: 191.1 MB (191075397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.10` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:8d5f495082abea977233155a08b50e5b98405fc110ad692f85e5f61b5c6175cf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **367.8 MB (367814921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb381a4dbf6e71916baefde96a33c513bf55b06d46571575a68a7158bf3c2b55`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Nov 2021 22:00:03 GMT
ADD file:ab83cb3e32154ba2db5167029d8e8d5388c50b5c29d8c79c713c0e0d2d692d27 in / 
# Thu, 04 Nov 2021 22:00:05 GMT
CMD ["bash"]
# Thu, 04 Nov 2021 22:18:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Nov 2021 22:19:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 04 Nov 2021 22:19:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 04 Nov 2021 22:20:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e737ddf26245fcdcc7eced9ccccb22176e9f1ba12d8f0d15cb1342c337544bdf`  
		Last Modified: Thu, 04 Nov 2021 22:01:24 GMT  
		Size: 30.5 MB (30525829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0355a8a2f0153f71261e3597b628202632603a052d63c9cecc0e1da9659b7c`  
		Last Modified: Thu, 04 Nov 2021 22:23:03 GMT  
		Size: 3.8 MB (3767643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f088a56f227fe3f111d256ae3c603419e2b9c7ee314548ef27c2479050a69e`  
		Last Modified: Thu, 04 Nov 2021 22:23:03 GMT  
		Size: 4.0 MB (3963241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d231728eaed51bc6e262952b25d2d76d8028ea980ea6f8651bf06147ac7981c`  
		Last Modified: Thu, 04 Nov 2021 22:23:15 GMT  
		Size: 38.3 MB (38324849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72d36bef3f492cf4db2c18617f56583fb674197398969239006ddf93f50495cc`  
		Last Modified: Thu, 04 Nov 2021 22:23:55 GMT  
		Size: 291.2 MB (291233359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:21.10-curl`

```console
$ docker pull buildpack-deps@sha256:b3afb9be9f6ff953e54c44375be156551f06d6b9ac5c003af34a32824ba7cd34
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
$ docker pull buildpack-deps@sha256:54c923092a83d0fd403372895cc7a052c5d93975a64600e8b2dc87c3ce47494a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37624372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5784379919f76e6e2636d7558d1932259ce9a619c55a89fd18de979439e5a863`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Nov 2021 22:20:34 GMT
ADD file:c061cabbaa10b98eed8dcea770d97000a2861c407f5208a0327bef2b38a99fee in / 
# Thu, 04 Nov 2021 22:20:35 GMT
CMD ["bash"]
# Thu, 04 Nov 2021 22:56:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Nov 2021 22:57:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ae6e1b672be676522e8af69609544dd00b8517e394592a58194383b26e9b54c5`  
		Last Modified: Thu, 04 Nov 2021 22:21:31 GMT  
		Size: 30.4 MB (30378721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4488401b75c6ec432177829c795e1ec36857d568171ae1f197c2c24a9b7e7d8d`  
		Last Modified: Thu, 04 Nov 2021 23:03:09 GMT  
		Size: 3.7 MB (3693784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb8a4e0bca131c5b9e451c10a345a0a13be03cf5ac1220cdc85f170d17be763`  
		Last Modified: Thu, 04 Nov 2021 23:03:09 GMT  
		Size: 3.6 MB (3551867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.10-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:cdf2e5e90315eff8c9fa17950a02925e550d668cabf6a092fd629fd2489cb835
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34103195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4c36290c105f7d65eff92415d0b8b56be4f54a2051c3e35b8e330c7dadda26e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Nov 2021 22:31:15 GMT
ADD file:675ad5623adf2dafceb59e4a67c75ca26f664127c76fe61c1903cc85d16b9abb in / 
# Thu, 04 Nov 2021 22:31:16 GMT
CMD ["bash"]
# Thu, 04 Nov 2021 23:28:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Nov 2021 23:28:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f7dc858b30797c13a0706f9660d1290ae625ab3436fd5db984b0dac888ad9c8f`  
		Last Modified: Thu, 04 Nov 2021 22:34:32 GMT  
		Size: 26.9 MB (26917157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64923825f2b20992e031b3992dc8c85722c1421e18d7f0fd69532d01d31c2617`  
		Last Modified: Thu, 04 Nov 2021 23:37:31 GMT  
		Size: 3.4 MB (3443243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d36d145711f3ed07bdbf6134addb14e00b663cb32b4de67ff1674023832998`  
		Last Modified: Thu, 04 Nov 2021 23:37:30 GMT  
		Size: 3.7 MB (3742795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.10-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:00c6025c7a15dfe57955537030d672bcdcaf4a2389fc446007e602d155927bf6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.0 MB (36031863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b11808ca59b32ca29aceb263695f64a95c22f3784efef11a16304f51f440ff1a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Nov 2021 21:55:45 GMT
ADD file:1b42b91df70bf5eb9529802354c8c97bb9ba991a7885a3fdd4ad5be4b662b70c in / 
# Thu, 04 Nov 2021 21:55:46 GMT
CMD ["bash"]
# Thu, 04 Nov 2021 22:28:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Nov 2021 22:29:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:07806c11d5adbc5d83daf2661f72147213f9056f681e452180dc14d81e368e17`  
		Last Modified: Thu, 04 Nov 2021 21:57:10 GMT  
		Size: 29.0 MB (29026100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a952a5c90bcb8e3a8ab1bd7854d8265e7fcb3cb0c0f417fb5722e8f3e0972208`  
		Last Modified: Thu, 04 Nov 2021 22:33:00 GMT  
		Size: 3.7 MB (3678628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cca9702f2a91f991f023bbb9b582e71befe4781bbaa74653b2458540b02c0e3`  
		Last Modified: Thu, 04 Nov 2021 22:32:59 GMT  
		Size: 3.3 MB (3327135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.10-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:0cc84931e7355f0a2ec18838056c982f9599d01d99f0a81c365098ed2373f8cd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.6 MB (44563129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:940ae21526802e5c51c15c215053b8095e827480a47aaea8d00e399c958e4dba`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Nov 2021 23:51:29 GMT
ADD file:dc4e5dbd5333b274b2af1c57862eeb96c4b2eda9e8d1a5b766b4ff2aa242106f in / 
# Thu, 04 Nov 2021 23:51:35 GMT
CMD ["bash"]
# Fri, 05 Nov 2021 01:51:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 05 Nov 2021 01:51:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6fb8a15f7529caac80795ba7b74d3c07d163030311fab31ef7b9eda5d4612190`  
		Last Modified: Thu, 04 Nov 2021 23:53:39 GMT  
		Size: 36.2 MB (36174155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a811f8d539d495275857666e419e2349b4afd49b9e35684be52fa958a9edfc64`  
		Last Modified: Fri, 05 Nov 2021 02:01:11 GMT  
		Size: 4.1 MB (4146837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567f57d31cc6184d7de4f38b999b49a84d09a99cd73ecff5fc148f918d7a9f85`  
		Last Modified: Fri, 05 Nov 2021 02:01:11 GMT  
		Size: 4.2 MB (4242137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.10-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:a60d9614189e9a414cd72cc5bcf35ff30825c9ba8c2ef9c68a3df23684370df2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34500741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:386b795e60ea56fff90f8871ec0d6d4c2fa29a17fe88c124d55251bb078e45b9`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 11 Nov 2021 01:34:25 GMT
ADD file:def88534019c26953298b38d1af30a296db3d6995d6c801bc98407de70a9e1a6 in / 
# Thu, 11 Nov 2021 01:34:26 GMT
CMD ["bash"]
# Thu, 11 Nov 2021 06:26:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 11 Nov 2021 06:27:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c236a68e6fcd6aac214c2851f12d0e004328b6cc65c84adea73ec2c8eccd27b8`  
		Last Modified: Thu, 11 Nov 2021 01:50:51 GMT  
		Size: 27.2 MB (27206693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32c0816a844c3da682a583d08b1d066cbf7fdaff37ecc1ffe756a1762b5116e`  
		Last Modified: Thu, 11 Nov 2021 06:54:43 GMT  
		Size: 3.5 MB (3490272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd32937a18c0c808ff182ae5991f2dcc6394079d138e4d6880d9013b9e5998a`  
		Last Modified: Thu, 11 Nov 2021 06:54:41 GMT  
		Size: 3.8 MB (3803776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.10-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:69d0be5d4a84d1fd9eccc366c301e3bb5eb1e5ee063ae63dfb73e0ab2b878b53
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38256713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4e776fddfc4e1399852bc124156b58b876d4f021cd53374abd1813b05be224c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Nov 2021 22:00:03 GMT
ADD file:ab83cb3e32154ba2db5167029d8e8d5388c50b5c29d8c79c713c0e0d2d692d27 in / 
# Thu, 04 Nov 2021 22:00:05 GMT
CMD ["bash"]
# Thu, 04 Nov 2021 22:18:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Nov 2021 22:19:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e737ddf26245fcdcc7eced9ccccb22176e9f1ba12d8f0d15cb1342c337544bdf`  
		Last Modified: Thu, 04 Nov 2021 22:01:24 GMT  
		Size: 30.5 MB (30525829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0355a8a2f0153f71261e3597b628202632603a052d63c9cecc0e1da9659b7c`  
		Last Modified: Thu, 04 Nov 2021 22:23:03 GMT  
		Size: 3.8 MB (3767643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f088a56f227fe3f111d256ae3c603419e2b9c7ee314548ef27c2479050a69e`  
		Last Modified: Thu, 04 Nov 2021 22:23:03 GMT  
		Size: 4.0 MB (3963241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:21.10-scm`

```console
$ docker pull buildpack-deps@sha256:bb68b5bf6258696aa2e152bfd8889269fc9f3f9c5b97287924f13739ea6ace1d
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
$ docker pull buildpack-deps@sha256:be7ea01ded251a2ca6d94d0c9f8153ef11a99c4f19603a96f01b918142d89bd5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75704595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb44de8b24049cedb568779358422987bb6b92d0a022d21f0e9440bde2381355`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Nov 2021 22:20:34 GMT
ADD file:c061cabbaa10b98eed8dcea770d97000a2861c407f5208a0327bef2b38a99fee in / 
# Thu, 04 Nov 2021 22:20:35 GMT
CMD ["bash"]
# Thu, 04 Nov 2021 22:56:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Nov 2021 22:57:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 04 Nov 2021 22:57:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ae6e1b672be676522e8af69609544dd00b8517e394592a58194383b26e9b54c5`  
		Last Modified: Thu, 04 Nov 2021 22:21:31 GMT  
		Size: 30.4 MB (30378721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4488401b75c6ec432177829c795e1ec36857d568171ae1f197c2c24a9b7e7d8d`  
		Last Modified: Thu, 04 Nov 2021 23:03:09 GMT  
		Size: 3.7 MB (3693784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb8a4e0bca131c5b9e451c10a345a0a13be03cf5ac1220cdc85f170d17be763`  
		Last Modified: Thu, 04 Nov 2021 23:03:09 GMT  
		Size: 3.6 MB (3551867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:538adb79b719e15749a81b037e806769f285f50a60ca3418546e00ffb465a44f`  
		Last Modified: Thu, 04 Nov 2021 23:03:25 GMT  
		Size: 38.1 MB (38080223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.10-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:c5609d52dc9fb38b4aacee4d68f362376ba20f2b951f9839df10238602a1df9f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.4 MB (74387065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:083634dd134e2787b5bdc31a4b94d37646c1fca8035481fd0462bf0215a072c3`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Nov 2021 22:31:15 GMT
ADD file:675ad5623adf2dafceb59e4a67c75ca26f664127c76fe61c1903cc85d16b9abb in / 
# Thu, 04 Nov 2021 22:31:16 GMT
CMD ["bash"]
# Thu, 04 Nov 2021 23:28:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Nov 2021 23:28:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 04 Nov 2021 23:29:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f7dc858b30797c13a0706f9660d1290ae625ab3436fd5db984b0dac888ad9c8f`  
		Last Modified: Thu, 04 Nov 2021 22:34:32 GMT  
		Size: 26.9 MB (26917157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64923825f2b20992e031b3992dc8c85722c1421e18d7f0fd69532d01d31c2617`  
		Last Modified: Thu, 04 Nov 2021 23:37:31 GMT  
		Size: 3.4 MB (3443243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d36d145711f3ed07bdbf6134addb14e00b663cb32b4de67ff1674023832998`  
		Last Modified: Thu, 04 Nov 2021 23:37:30 GMT  
		Size: 3.7 MB (3742795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:016df4abc6b88c7564811d0545d3f7eeb911db620be98dce64597a05cd3747b7`  
		Last Modified: Thu, 04 Nov 2021 23:38:12 GMT  
		Size: 40.3 MB (40283870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.10-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:6ca52d36f45191c2bff56479c7addc641c520e3b721d237287a1a6e6a2295e7e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.1 MB (74064301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e02fffcd9134167d6655e1c30a85beecb06ef2c9233cdef78e37897b5d398341`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Nov 2021 21:55:45 GMT
ADD file:1b42b91df70bf5eb9529802354c8c97bb9ba991a7885a3fdd4ad5be4b662b70c in / 
# Thu, 04 Nov 2021 21:55:46 GMT
CMD ["bash"]
# Thu, 04 Nov 2021 22:28:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Nov 2021 22:29:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 04 Nov 2021 22:29:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:07806c11d5adbc5d83daf2661f72147213f9056f681e452180dc14d81e368e17`  
		Last Modified: Thu, 04 Nov 2021 21:57:10 GMT  
		Size: 29.0 MB (29026100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a952a5c90bcb8e3a8ab1bd7854d8265e7fcb3cb0c0f417fb5722e8f3e0972208`  
		Last Modified: Thu, 04 Nov 2021 22:33:00 GMT  
		Size: 3.7 MB (3678628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cca9702f2a91f991f023bbb9b582e71befe4781bbaa74653b2458540b02c0e3`  
		Last Modified: Thu, 04 Nov 2021 22:32:59 GMT  
		Size: 3.3 MB (3327135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e1d1ea4e9af80ec48e6e5d034e77b64b8de00080ef82b379213f41b1da18b1`  
		Last Modified: Thu, 04 Nov 2021 22:33:17 GMT  
		Size: 38.0 MB (38032438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.10-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:eed517a6832af7446961327af826bf0c50b3fc7d9259158a2bc4dd3dc53759c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.3 MB (87270621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94972edd2bba9d41b3a39c0aef62bc5e7650c595afdbbd8b3ca9ce835ef6c6e4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Nov 2021 23:51:29 GMT
ADD file:dc4e5dbd5333b274b2af1c57862eeb96c4b2eda9e8d1a5b766b4ff2aa242106f in / 
# Thu, 04 Nov 2021 23:51:35 GMT
CMD ["bash"]
# Fri, 05 Nov 2021 01:51:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 05 Nov 2021 01:51:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 05 Nov 2021 01:53:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6fb8a15f7529caac80795ba7b74d3c07d163030311fab31ef7b9eda5d4612190`  
		Last Modified: Thu, 04 Nov 2021 23:53:39 GMT  
		Size: 36.2 MB (36174155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a811f8d539d495275857666e419e2349b4afd49b9e35684be52fa958a9edfc64`  
		Last Modified: Fri, 05 Nov 2021 02:01:11 GMT  
		Size: 4.1 MB (4146837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567f57d31cc6184d7de4f38b999b49a84d09a99cd73ecff5fc148f918d7a9f85`  
		Last Modified: Fri, 05 Nov 2021 02:01:11 GMT  
		Size: 4.2 MB (4242137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cfc0512fc4cbeb0f1888bd931fc2dbf9f49bc00278d9c2c5b7aa5272e519c1d`  
		Last Modified: Fri, 05 Nov 2021 02:01:31 GMT  
		Size: 42.7 MB (42707492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.10-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:1646f127c48e431100e6930d603da4cef39744d303aff6bfe9a3f5d35ba69e1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.3 MB (75264216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d52e65f7ce2ae95fda50dd675073c828cf1f9e113d34ed156decaeb6b34711fc`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 11 Nov 2021 01:34:25 GMT
ADD file:def88534019c26953298b38d1af30a296db3d6995d6c801bc98407de70a9e1a6 in / 
# Thu, 11 Nov 2021 01:34:26 GMT
CMD ["bash"]
# Thu, 11 Nov 2021 06:26:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 11 Nov 2021 06:27:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 11 Nov 2021 06:30:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c236a68e6fcd6aac214c2851f12d0e004328b6cc65c84adea73ec2c8eccd27b8`  
		Last Modified: Thu, 11 Nov 2021 01:50:51 GMT  
		Size: 27.2 MB (27206693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32c0816a844c3da682a583d08b1d066cbf7fdaff37ecc1ffe756a1762b5116e`  
		Last Modified: Thu, 11 Nov 2021 06:54:43 GMT  
		Size: 3.5 MB (3490272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd32937a18c0c808ff182ae5991f2dcc6394079d138e4d6880d9013b9e5998a`  
		Last Modified: Thu, 11 Nov 2021 06:54:41 GMT  
		Size: 3.8 MB (3803776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20817c240d9af80288c0d7e22536e4e16be4622339e8522790aa1ddd56e8fd08`  
		Last Modified: Thu, 11 Nov 2021 06:56:39 GMT  
		Size: 40.8 MB (40763475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.10-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b961b4b9338629accb7eb8c51ddf4512dee4ea4f483996fde0ae3b33285dc076
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.6 MB (76581562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84b6e0cec4c3e1a5925b93493e48cd160b3afbf055e9831774038268ea7ef6bf`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Nov 2021 22:00:03 GMT
ADD file:ab83cb3e32154ba2db5167029d8e8d5388c50b5c29d8c79c713c0e0d2d692d27 in / 
# Thu, 04 Nov 2021 22:00:05 GMT
CMD ["bash"]
# Thu, 04 Nov 2021 22:18:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Nov 2021 22:19:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 04 Nov 2021 22:19:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e737ddf26245fcdcc7eced9ccccb22176e9f1ba12d8f0d15cb1342c337544bdf`  
		Last Modified: Thu, 04 Nov 2021 22:01:24 GMT  
		Size: 30.5 MB (30525829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0355a8a2f0153f71261e3597b628202632603a052d63c9cecc0e1da9659b7c`  
		Last Modified: Thu, 04 Nov 2021 22:23:03 GMT  
		Size: 3.8 MB (3767643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f088a56f227fe3f111d256ae3c603419e2b9c7ee314548ef27c2479050a69e`  
		Last Modified: Thu, 04 Nov 2021 22:23:03 GMT  
		Size: 4.0 MB (3963241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d231728eaed51bc6e262952b25d2d76d8028ea980ea6f8651bf06147ac7981c`  
		Last Modified: Thu, 04 Nov 2021 22:23:15 GMT  
		Size: 38.3 MB (38324849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bionic`

```console
$ docker pull buildpack-deps@sha256:b2b2faaae9b30af6432903f81f858e6362cede40078ad6b8fc7456e0045c9993
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
$ docker pull buildpack-deps@sha256:19c0527602ef9047ea9af278bd2e7c739b4639471a44a2e9462b14f8b619cec7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.4 MB (205381635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c0fc413befe38312de14b98f4ecb6c76ea42726f0169b3d760775a153ca9434`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:38 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Sat, 16 Oct 2021 01:47:38 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:04:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:04:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 03:05:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:06:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a555366df07c0f7aae069a38b120e5b8e6e95f359b898d0032574413b8b2c1`  
		Last Modified: Sat, 16 Oct 2021 03:19:21 GMT  
		Size: 6.1 MB (6084243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233462b381c92a25d3bf01a6a656557732c43fb811b0b5173d611ac8fd767a94`  
		Last Modified: Sat, 16 Oct 2021 03:19:20 GMT  
		Size: 2.6 MB (2570190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237b11e5d0bf83fb3fb6bdb6b3cfd1967ea6e80fd7bf3b2f3f6167b48ba59cbd`  
		Last Modified: Sat, 16 Oct 2021 03:19:39 GMT  
		Size: 43.3 MB (43277011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f134b5b86813b51223749bd3bdbe427289e06813ec214b870337081a650822`  
		Last Modified: Sat, 16 Oct 2021 03:20:09 GMT  
		Size: 129.7 MB (129722715 bytes)  
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
$ docker pull buildpack-deps@sha256:8fd11f4c0036db05fb68618db00da04b0c79c13f44859c75bb7208f2e1dd64fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.2 MB (246225436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:098c5a0af01f04f9df9faef2c21612259a54295d1e4ac9ab63471dde03939d4c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Oct 2021 11:07:29 GMT
ADD file:fd96554dfb72307c3cf9292c343050a8b9f0848735b7555820f0068914ebd758 in / 
# Tue, 05 Oct 2021 11:07:35 GMT
CMD ["bash"]
# Tue, 05 Oct 2021 14:41:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Oct 2021 14:42:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 05 Oct 2021 14:46:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 05 Oct 2021 14:57:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:db28fc1e594e5598e665c54ac1b7fd602d86dddaf8bb237a72303cec22a9185c`  
		Last Modified: Tue, 05 Oct 2021 11:10:31 GMT  
		Size: 30.4 MB (30432921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb1c3498d7cd3adcb6d716b98adcea053880272423eb1a9939a7426d428cfd8`  
		Last Modified: Tue, 05 Oct 2021 15:46:03 GMT  
		Size: 7.1 MB (7058539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:494fb7e48f3a6cbd76b9eaab065228a859bdd7e6f41a24d6aa2cf74d77d31e73`  
		Last Modified: Tue, 05 Oct 2021 15:45:58 GMT  
		Size: 3.7 MB (3719778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961571b34653877509a0b15ed874ac56391305c5a20707a48fdf723b3becd986`  
		Last Modified: Tue, 05 Oct 2021 15:46:51 GMT  
		Size: 53.7 MB (53722746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e23c150699147a85f182ea8b9a515a5693a4957bd9f3d7a86057372d8888d231`  
		Last Modified: Tue, 05 Oct 2021 15:48:34 GMT  
		Size: 151.3 MB (151291452 bytes)  
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
$ docker pull buildpack-deps@sha256:d910ddef17dc4c1e788ed6f495c671dc76199b485090f1114409077b13ef7d2d
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
$ docker pull buildpack-deps@sha256:b3aa99deddad631d348b89d6c671ec7bd6d1fd898210f07ed15f38b9527174d0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.4 MB (32381909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc96931ce78d81afa20b59e979221712e50c103543abd31b3f45a8d2d4ed29ec`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:38 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Sat, 16 Oct 2021 01:47:38 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:04:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:04:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a555366df07c0f7aae069a38b120e5b8e6e95f359b898d0032574413b8b2c1`  
		Last Modified: Sat, 16 Oct 2021 03:19:21 GMT  
		Size: 6.1 MB (6084243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233462b381c92a25d3bf01a6a656557732c43fb811b0b5173d611ac8fd767a94`  
		Last Modified: Sat, 16 Oct 2021 03:19:20 GMT  
		Size: 2.6 MB (2570190 bytes)  
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
$ docker pull buildpack-deps@sha256:83e8be4ead24277419d0cd40f98276cfb93f497d55128a5c2db9eac556213a4c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41211238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c4951cd140e5db022882ab2a533d8ee9c6728be12eaa2480606c112538681a7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Oct 2021 11:07:29 GMT
ADD file:fd96554dfb72307c3cf9292c343050a8b9f0848735b7555820f0068914ebd758 in / 
# Tue, 05 Oct 2021 11:07:35 GMT
CMD ["bash"]
# Tue, 05 Oct 2021 14:41:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Oct 2021 14:42:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:db28fc1e594e5598e665c54ac1b7fd602d86dddaf8bb237a72303cec22a9185c`  
		Last Modified: Tue, 05 Oct 2021 11:10:31 GMT  
		Size: 30.4 MB (30432921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb1c3498d7cd3adcb6d716b98adcea053880272423eb1a9939a7426d428cfd8`  
		Last Modified: Tue, 05 Oct 2021 15:46:03 GMT  
		Size: 7.1 MB (7058539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:494fb7e48f3a6cbd76b9eaab065228a859bdd7e6f41a24d6aa2cf74d77d31e73`  
		Last Modified: Tue, 05 Oct 2021 15:45:58 GMT  
		Size: 3.7 MB (3719778 bytes)  
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
$ docker pull buildpack-deps@sha256:a161d52291bf8c954c5c827dca5ef294681a85fc96aa37eec6b14d4d093a26dc
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
$ docker pull buildpack-deps@sha256:4cd7d49c2897395988195e6981f71613db7fe5968de61afdf95af231ada24c78
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75658920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5408604964ea4bbf7712a3f19081f5d0aeb3813f010484bb8d592e9dd6603469`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:38 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Sat, 16 Oct 2021 01:47:38 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:04:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:04:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 03:05:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a555366df07c0f7aae069a38b120e5b8e6e95f359b898d0032574413b8b2c1`  
		Last Modified: Sat, 16 Oct 2021 03:19:21 GMT  
		Size: 6.1 MB (6084243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233462b381c92a25d3bf01a6a656557732c43fb811b0b5173d611ac8fd767a94`  
		Last Modified: Sat, 16 Oct 2021 03:19:20 GMT  
		Size: 2.6 MB (2570190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237b11e5d0bf83fb3fb6bdb6b3cfd1967ea6e80fd7bf3b2f3f6167b48ba59cbd`  
		Last Modified: Sat, 16 Oct 2021 03:19:39 GMT  
		Size: 43.3 MB (43277011 bytes)  
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
$ docker pull buildpack-deps@sha256:d4a4d531a63f36ca9d9b778f021e88bedc03615312d12bc138ae8829798e9d40
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.9 MB (94933984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55b74a920f641c6acbe8e3557e6b0420efaa1a94b372cdffb52a99991e04d210`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Oct 2021 11:07:29 GMT
ADD file:fd96554dfb72307c3cf9292c343050a8b9f0848735b7555820f0068914ebd758 in / 
# Tue, 05 Oct 2021 11:07:35 GMT
CMD ["bash"]
# Tue, 05 Oct 2021 14:41:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Oct 2021 14:42:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 05 Oct 2021 14:46:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:db28fc1e594e5598e665c54ac1b7fd602d86dddaf8bb237a72303cec22a9185c`  
		Last Modified: Tue, 05 Oct 2021 11:10:31 GMT  
		Size: 30.4 MB (30432921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb1c3498d7cd3adcb6d716b98adcea053880272423eb1a9939a7426d428cfd8`  
		Last Modified: Tue, 05 Oct 2021 15:46:03 GMT  
		Size: 7.1 MB (7058539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:494fb7e48f3a6cbd76b9eaab065228a859bdd7e6f41a24d6aa2cf74d77d31e73`  
		Last Modified: Tue, 05 Oct 2021 15:45:58 GMT  
		Size: 3.7 MB (3719778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961571b34653877509a0b15ed874ac56391305c5a20707a48fdf723b3becd986`  
		Last Modified: Tue, 05 Oct 2021 15:46:51 GMT  
		Size: 53.7 MB (53722746 bytes)  
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
$ docker pull buildpack-deps@sha256:39d6d1b626103d5d8daecf321abe9d8a1ce5cc8cbff2cd3195b4fdb04af654f3
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
$ docker pull buildpack-deps@sha256:067329836a99c56bd087b255c70cf2e7bb7f0c1965d8a12be769c86a062c12a4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.0 MB (322022992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48a4688637227faef31aa5134c34ca2ec85dd07beebcf327c38566eb3eb8ef79`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:15:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66b7f31b095b7fa01d8ba10e600a192bab43a1311f50216cf6fa9a45d0f435e`  
		Last Modified: Wed, 17 Nov 2021 03:24:18 GMT  
		Size: 196.5 MB (196498701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:095b3e58e31205572ba70b19cefdc7ec5de99683e74c0c8f095e3d564b2e1f0b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.1 MB (295100343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc59e839989efbe22d3c9e21e3cefb3c810799f569486d4f5493b98c454a3bb1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 00:49:54 GMT
ADD file:b9969604315238de271e1769a4b8dd85cdf0d33f9fac387e940d5195ac3030a1 in / 
# Tue, 12 Oct 2021 00:49:55 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:40:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:41:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 05:42:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:44:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a97c782f2538791984ce12c859cada96e395e3950d4cb7d1238e08acd2eb74ec`  
		Last Modified: Tue, 12 Oct 2021 01:05:12 GMT  
		Size: 52.5 MB (52452198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34dc529b005dbeff70906cd4baf2310c918ae6379fdf53ef632c3cd1203aa38`  
		Last Modified: Tue, 12 Oct 2021 06:01:18 GMT  
		Size: 5.1 MB (5063794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2876b7f933f68a5b4f35f854cc8c651bf3d21476fe2bb0a786e6376f389b44b`  
		Last Modified: Tue, 12 Oct 2021 06:01:20 GMT  
		Size: 10.6 MB (10571017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c918a5faa65bffd689b9869a942e77a3fbc7d89566be880da188d6050f4f627`  
		Last Modified: Tue, 12 Oct 2021 06:02:11 GMT  
		Size: 52.3 MB (52322898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3127725d64ae6922801ff988a903c7db9c780283ffb0ed82afa5763076b47be7`  
		Last Modified: Tue, 12 Oct 2021 06:04:12 GMT  
		Size: 174.7 MB (174690436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:d56f41aa9c8faf2f038f7d533362e91ee583358bc719176d20f3c17daad0fb9f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.5 MB (282546908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7d3fb1baab35afcb64347548d5cecdba2a8cd3c4299b815347de10b18e7fa29`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 01:59:07 GMT
ADD file:43b45f65ff4ba720f6f9a107b5f80818d5ea6ebc4835840b11e9a506351da32f in / 
# Wed, 17 Nov 2021 01:59:08 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:41:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:42:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 02:43:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:45:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dbbf55137aab3c7acd1e012a70f1ea1adeaef8d39b474829965d3480a02bf572`  
		Last Modified: Wed, 17 Nov 2021 02:14:27 GMT  
		Size: 50.1 MB (50134152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb1ae7a04cee77523f9e09a62b28632c56a700d0c481be7cddc566c835e7a71d`  
		Last Modified: Wed, 17 Nov 2021 03:04:13 GMT  
		Size: 4.9 MB (4922782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66894dfea839186e94448f6c25a37c6b3b1b42cece6332cc9d36336917e18a4`  
		Last Modified: Wed, 17 Nov 2021 03:04:14 GMT  
		Size: 10.2 MB (10216965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4502933ba6aa2071501257e094faa363699dc23995f798a124d688c2523240af`  
		Last Modified: Wed, 17 Nov 2021 03:05:05 GMT  
		Size: 50.3 MB (50327664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b521106771559ec34e350caa7c1220e7d91669cfdd392f09bf61b4de0ffbfed6`  
		Last Modified: Wed, 17 Nov 2021 03:06:54 GMT  
		Size: 166.9 MB (166945345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:53545965440c95434bfc95e564fd274f086892b89a42ff4ff145f60ef5ba02df
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.3 MB (313267051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:455c971696419e341265a976576201f36454718c107fcd51d4c07ecf67d23d13`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:59 GMT
ADD file:eb667e18226da8a1ca5a41beacddc65cd1efec01c3d01e50845c5e89e91ea17c in / 
# Wed, 17 Nov 2021 02:40:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:26:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:26:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:27:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:27:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce18cd0ba11c2dfa8c1a2d2b325e1e019b14d4ae25ffdeffb0f9686c5496bf5c`  
		Last Modified: Wed, 17 Nov 2021 02:46:45 GMT  
		Size: 53.6 MB (53619024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f138a340a2373acc72dcc4ea9ef08bdf5648aabc5fe08f7e8d25222ca63b7ee`  
		Last Modified: Wed, 17 Nov 2021 13:36:26 GMT  
		Size: 4.9 MB (4937639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34c030205ccb8656e30a58f96bb1edbe7c59bf17f3329ae3c442ec897f2b270`  
		Last Modified: Wed, 17 Nov 2021 13:36:27 GMT  
		Size: 10.7 MB (10655878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7a1cfcc2070fbe1e702751d85f7074b93d142f6beb03ef66e9ba1c58bcc3e3`  
		Last Modified: Wed, 17 Nov 2021 13:36:49 GMT  
		Size: 54.7 MB (54669696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3503a35f6e45ec76f6c25673ef4934feb88c3c35ee30ffc8bf7437a0ade8e15`  
		Last Modified: Wed, 17 Nov 2021 13:37:28 GMT  
		Size: 189.4 MB (189384814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; 386

```console
$ docker pull buildpack-deps@sha256:22b4c7d5f90e61044a709672c2f9f4172afc8d87432cb5e8ec6165670064022b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.8 MB (327786933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd6b36232cd4509daee36d1370c035efee46f839cd7eca26d55136f8274a2db8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:39:30 GMT
ADD file:e007d6eff02dbc696e1166db315b97a77ae8aa65f2e66ca8074765dde9c70a59 in / 
# Tue, 12 Oct 2021 01:39:31 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:35:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:36:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 04:36:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:37:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6911c8f66691266d86e2cafa67ca005d919f357436fac971c694d37625b5ba90`  
		Last Modified: Tue, 12 Oct 2021 01:47:06 GMT  
		Size: 55.9 MB (55923419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a0f31369a20c178b1d5c84f192412ed962068e8932d5821eefb00bc7d1cbc1a`  
		Last Modified: Tue, 12 Oct 2021 04:47:26 GMT  
		Size: 5.3 MB (5283102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97aa3d222d7e8d6e0b06e57e5bd03168c422475942f92d09a487bd98d09bb742`  
		Last Modified: Tue, 12 Oct 2021 04:47:27 GMT  
		Size: 11.3 MB (11250699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae99d06bab5fc31ba3db9436a22c452db74a7b5e559a451de2d971a493abe52`  
		Last Modified: Tue, 12 Oct 2021 04:48:03 GMT  
		Size: 55.9 MB (55917451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ceaeace1516b23dd6c26014f977ec910629b0f1e818efcba72285c444c745dc`  
		Last Modified: Tue, 12 Oct 2021 04:49:16 GMT  
		Size: 199.4 MB (199412262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:a2b66ff7f5602d629f435424734849d38a6e15416a23b64b2d23e13178660e84
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.1 MB (301083355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a25bde1d7937a6f6dd29e4c251d24e4a821689a59f57bb28e96e734a349c0faa`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:09:46 GMT
ADD file:2971df49f24648b8d5166d87e392e2547d5b03469356f20d112ce6feb3c329fc in / 
# Wed, 17 Nov 2021 02:09:47 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:29:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:30:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 08:31:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:33:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b095a0b63d99a4c4cd9c1c353f381a69ef041e6f80798d807ae51a34b04920a0`  
		Last Modified: Wed, 17 Nov 2021 02:18:22 GMT  
		Size: 53.2 MB (53183806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2e37aff1692726b1ea3dd0b4eeb684072527295f8e981d3c45825327daea19`  
		Last Modified: Wed, 17 Nov 2021 08:45:38 GMT  
		Size: 5.1 MB (5114925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d4c0302ddd7a6cb573a156076dba9c593e09a0c321b32ae0f1da2bd36bc754`  
		Last Modified: Wed, 17 Nov 2021 08:45:41 GMT  
		Size: 10.9 MB (10873360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cde5eca075420fcfc6498f454dc040f1e236dea180a82a0d27d7a739ffd41c1`  
		Last Modified: Wed, 17 Nov 2021 08:46:32 GMT  
		Size: 53.3 MB (53296603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b326e913cf09f7b591a15250a21e659e1a1490c8db287698247813607f511be`  
		Last Modified: Wed, 17 Nov 2021 08:48:42 GMT  
		Size: 178.6 MB (178614661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3ad89b390c0582bf3f9073da22edc33da00fa72294f690312f20c8670974f6ae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.6 MB (330552911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c32d3a8d6d884cd659ea67e7f174cd8ba989c9582a46828d4a63585aeaf8c56f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 03:27:04 GMT
ADD file:85375acb19da58f9eabaa67f8cb425cd1ff2dadb2888bbd9dbfa6223d16fef23 in / 
# Wed, 17 Nov 2021 03:27:20 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 07:40:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 07:40:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 07:42:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 07:51:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ede9cd7c8f1d380c971a130fb3d8a3914bf3a9106702164c23b2cce536fa618c`  
		Last Modified: Wed, 17 Nov 2021 03:52:39 GMT  
		Size: 58.8 MB (58819505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743814bfd79326104da0238d8edced6b14f63b95734b6dc0e2b7a9d83356b0cb`  
		Last Modified: Wed, 17 Nov 2021 08:25:58 GMT  
		Size: 5.4 MB (5402000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca978d94a6543bbd1c60026602b64e810b4bf65e052dcf19adf2b4d6b518bf8`  
		Last Modified: Wed, 17 Nov 2021 08:25:59 GMT  
		Size: 11.6 MB (11626016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d785f1d8909cb3a3e46844611c28e15781da809be0073e40af017d6e5631d0`  
		Last Modified: Wed, 17 Nov 2021 08:26:57 GMT  
		Size: 58.9 MB (58851458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18fadd6314eacb7e881a9590b8566952a97cc84d87002b2f80c125e36f166f91`  
		Last Modified: Wed, 17 Nov 2021 08:28:32 GMT  
		Size: 195.9 MB (195853932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b771ceede0a02f3c3e45fbf245a79af43a82d8a5a89e280847ac77f34783db7f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.6 MB (295637108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:424bab9df7f41f34456e281a4d38395352c0b8a719a123e6e3da820dad5b62e2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:07 GMT
ADD file:b7524e775a2033d246d1096765a0eb6eaa5ba6ed6c8b395522579d2c4e7a2e38 in / 
# Wed, 17 Nov 2021 02:42:09 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:07:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:07:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:08:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:09:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ffa47acd07831fbc96680a705da20704bac0016c20dc3c454ecd45cda44b368d`  
		Last Modified: Wed, 17 Nov 2021 02:48:05 GMT  
		Size: 53.2 MB (53207179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c950336719691da019c99e4ff78fe559ab0308ea145757994bdb7be34c6d224`  
		Last Modified: Wed, 17 Nov 2021 03:17:18 GMT  
		Size: 5.1 MB (5137199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d769af2ca44d1c7c206e7190cd71df7cb5ff3df2dd45e1dd52ea447ffb547b1a`  
		Last Modified: Wed, 17 Nov 2021 03:17:19 GMT  
		Size: 10.8 MB (10761499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3bbc68017b41a8cc07b10d715e2a23108c5addefa80b01cac1a2ef075bb1acd`  
		Last Modified: Wed, 17 Nov 2021 03:17:36 GMT  
		Size: 54.0 MB (54041155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5890dc05b0932fa2fcd5ebf331e2dbb96bf6af4989173b3745e7228388fc8f0a`  
		Last Modified: Wed, 17 Nov 2021 03:18:03 GMT  
		Size: 172.5 MB (172490076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bullseye-curl`

```console
$ docker pull buildpack-deps@sha256:55e8b08399933366af5bf7339d286a42b69484a144be7a9505b9652bb3abc9d4
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
$ docker pull buildpack-deps@sha256:0edf02c125a1738634b314fe74509188fe8ec80d4fe0e5dcb6a8e2c69b752eda
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.0 MB (70957967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4210c06ad2290080f1e15b81fcab4884d6d092607663ed35830d2cb7f05d88df`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:8f64ae6a92bbcdf3bd87aa336ab8cfbe025c94f2871fb30c7c869ddf5b398637
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68087009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:452c0670207bd3308452b37f769e1991141d3955fb9c449d6651538516664d78`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 00:49:54 GMT
ADD file:b9969604315238de271e1769a4b8dd85cdf0d33f9fac387e940d5195ac3030a1 in / 
# Tue, 12 Oct 2021 00:49:55 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:40:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:41:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a97c782f2538791984ce12c859cada96e395e3950d4cb7d1238e08acd2eb74ec`  
		Last Modified: Tue, 12 Oct 2021 01:05:12 GMT  
		Size: 52.5 MB (52452198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34dc529b005dbeff70906cd4baf2310c918ae6379fdf53ef632c3cd1203aa38`  
		Last Modified: Tue, 12 Oct 2021 06:01:18 GMT  
		Size: 5.1 MB (5063794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2876b7f933f68a5b4f35f854cc8c651bf3d21476fe2bb0a786e6376f389b44b`  
		Last Modified: Tue, 12 Oct 2021 06:01:20 GMT  
		Size: 10.6 MB (10571017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:e0db5a4c0ddaf3021a476cd83cb48a47baae27cafc02c61fd6151c2b113034fd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65273899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a096ebca0a1dcf6c812935690d2f1ceba23cdc7565b5dedf1b01adb266c3296a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 01:59:07 GMT
ADD file:43b45f65ff4ba720f6f9a107b5f80818d5ea6ebc4835840b11e9a506351da32f in / 
# Wed, 17 Nov 2021 01:59:08 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:41:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:42:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:dbbf55137aab3c7acd1e012a70f1ea1adeaef8d39b474829965d3480a02bf572`  
		Last Modified: Wed, 17 Nov 2021 02:14:27 GMT  
		Size: 50.1 MB (50134152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb1ae7a04cee77523f9e09a62b28632c56a700d0c481be7cddc566c835e7a71d`  
		Last Modified: Wed, 17 Nov 2021 03:04:13 GMT  
		Size: 4.9 MB (4922782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66894dfea839186e94448f6c25a37c6b3b1b42cece6332cc9d36336917e18a4`  
		Last Modified: Wed, 17 Nov 2021 03:04:14 GMT  
		Size: 10.2 MB (10216965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c52337b05fa1f275820e562dc39597db3ec027dbc6930cd6c1424233776c385c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69212541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:638dd156261f84c328de4551fcff54679fa0628f7b63b62344e169cb0cfdf82c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:59 GMT
ADD file:eb667e18226da8a1ca5a41beacddc65cd1efec01c3d01e50845c5e89e91ea17c in / 
# Wed, 17 Nov 2021 02:40:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:26:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:26:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ce18cd0ba11c2dfa8c1a2d2b325e1e019b14d4ae25ffdeffb0f9686c5496bf5c`  
		Last Modified: Wed, 17 Nov 2021 02:46:45 GMT  
		Size: 53.6 MB (53619024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f138a340a2373acc72dcc4ea9ef08bdf5648aabc5fe08f7e8d25222ca63b7ee`  
		Last Modified: Wed, 17 Nov 2021 13:36:26 GMT  
		Size: 4.9 MB (4937639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34c030205ccb8656e30a58f96bb1edbe7c59bf17f3329ae3c442ec897f2b270`  
		Last Modified: Wed, 17 Nov 2021 13:36:27 GMT  
		Size: 10.7 MB (10655878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:307bd4c6b80d221cc5ffaa51a6561a19f142cbe2349df40cd823c45df8a66d0c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72457220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1fe930770d8d6583e5406717d0128e6efa4aa9438733ab028c7df182c036184`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:39:30 GMT
ADD file:e007d6eff02dbc696e1166db315b97a77ae8aa65f2e66ca8074765dde9c70a59 in / 
# Tue, 12 Oct 2021 01:39:31 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:35:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:36:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6911c8f66691266d86e2cafa67ca005d919f357436fac971c694d37625b5ba90`  
		Last Modified: Tue, 12 Oct 2021 01:47:06 GMT  
		Size: 55.9 MB (55923419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a0f31369a20c178b1d5c84f192412ed962068e8932d5821eefb00bc7d1cbc1a`  
		Last Modified: Tue, 12 Oct 2021 04:47:26 GMT  
		Size: 5.3 MB (5283102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97aa3d222d7e8d6e0b06e57e5bd03168c422475942f92d09a487bd98d09bb742`  
		Last Modified: Tue, 12 Oct 2021 04:47:27 GMT  
		Size: 11.3 MB (11250699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:c8e1c20d487b63fa0111dd8c6dbb3e8cad660d4ad92dfedcc288dbcf88b52ae1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69172091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e01b4e0250266355d14651090fbb68f4b5950f1e1e3e93ad45e1d024d3e8db78`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:09:46 GMT
ADD file:2971df49f24648b8d5166d87e392e2547d5b03469356f20d112ce6feb3c329fc in / 
# Wed, 17 Nov 2021 02:09:47 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:29:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:30:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b095a0b63d99a4c4cd9c1c353f381a69ef041e6f80798d807ae51a34b04920a0`  
		Last Modified: Wed, 17 Nov 2021 02:18:22 GMT  
		Size: 53.2 MB (53183806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2e37aff1692726b1ea3dd0b4eeb684072527295f8e981d3c45825327daea19`  
		Last Modified: Wed, 17 Nov 2021 08:45:38 GMT  
		Size: 5.1 MB (5114925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d4c0302ddd7a6cb573a156076dba9c593e09a0c321b32ae0f1da2bd36bc754`  
		Last Modified: Wed, 17 Nov 2021 08:45:41 GMT  
		Size: 10.9 MB (10873360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:ffc112a46cd4cb66176c5d7b815903b1652b33a26fb9f38d3233e1892293d496
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.8 MB (75847521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17cfe935fd31679e71de8a6756361a413d64351be692488a2fd6c0de16648ada`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 03:27:04 GMT
ADD file:85375acb19da58f9eabaa67f8cb425cd1ff2dadb2888bbd9dbfa6223d16fef23 in / 
# Wed, 17 Nov 2021 03:27:20 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 07:40:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 07:40:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ede9cd7c8f1d380c971a130fb3d8a3914bf3a9106702164c23b2cce536fa618c`  
		Last Modified: Wed, 17 Nov 2021 03:52:39 GMT  
		Size: 58.8 MB (58819505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743814bfd79326104da0238d8edced6b14f63b95734b6dc0e2b7a9d83356b0cb`  
		Last Modified: Wed, 17 Nov 2021 08:25:58 GMT  
		Size: 5.4 MB (5402000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca978d94a6543bbd1c60026602b64e810b4bf65e052dcf19adf2b4d6b518bf8`  
		Last Modified: Wed, 17 Nov 2021 08:25:59 GMT  
		Size: 11.6 MB (11626016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:864eebbaafc1154c0017d16100182a15ea13c7dd81a1e2474b581c03a8e4d27c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69105877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d1c13a820b2c0e693a7fcd87c7888df8a0f95367ff8e2381ec07faf8e711307`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:07 GMT
ADD file:b7524e775a2033d246d1096765a0eb6eaa5ba6ed6c8b395522579d2c4e7a2e38 in / 
# Wed, 17 Nov 2021 02:42:09 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:07:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:07:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ffa47acd07831fbc96680a705da20704bac0016c20dc3c454ecd45cda44b368d`  
		Last Modified: Wed, 17 Nov 2021 02:48:05 GMT  
		Size: 53.2 MB (53207179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c950336719691da019c99e4ff78fe559ab0308ea145757994bdb7be34c6d224`  
		Last Modified: Wed, 17 Nov 2021 03:17:18 GMT  
		Size: 5.1 MB (5137199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d769af2ca44d1c7c206e7190cd71df7cb5ff3df2dd45e1dd52ea447ffb547b1a`  
		Last Modified: Wed, 17 Nov 2021 03:17:19 GMT  
		Size: 10.8 MB (10761499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bullseye-scm`

```console
$ docker pull buildpack-deps@sha256:993f6b93af203b5057bca0bf5858d22798c837de81f63c65326cf4bd25734d20
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
$ docker pull buildpack-deps@sha256:705b87b1c31cbc5283ea312fb0af16deeda2d00a9121f33d1779813dff4dd55b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.5 MB (125524291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e81de6f42b69f2697b8b01a08799441414abcedf96ec293b306eddb6d0d6c8ba`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:ab1b571f15dc9620590ae51b9e2a70cfb75b6438013b7a3599f47e39f6c7d600
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.4 MB (120409907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e962133851ffbc9d390eb7b46532392de0c1e19443d48ed2c7a52c4ca877cc2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 00:49:54 GMT
ADD file:b9969604315238de271e1769a4b8dd85cdf0d33f9fac387e940d5195ac3030a1 in / 
# Tue, 12 Oct 2021 00:49:55 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:40:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:41:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 05:42:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a97c782f2538791984ce12c859cada96e395e3950d4cb7d1238e08acd2eb74ec`  
		Last Modified: Tue, 12 Oct 2021 01:05:12 GMT  
		Size: 52.5 MB (52452198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34dc529b005dbeff70906cd4baf2310c918ae6379fdf53ef632c3cd1203aa38`  
		Last Modified: Tue, 12 Oct 2021 06:01:18 GMT  
		Size: 5.1 MB (5063794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2876b7f933f68a5b4f35f854cc8c651bf3d21476fe2bb0a786e6376f389b44b`  
		Last Modified: Tue, 12 Oct 2021 06:01:20 GMT  
		Size: 10.6 MB (10571017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c918a5faa65bffd689b9869a942e77a3fbc7d89566be880da188d6050f4f627`  
		Last Modified: Tue, 12 Oct 2021 06:02:11 GMT  
		Size: 52.3 MB (52322898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:19565c156eedbb4210675b27d3f633814a7f585b53d58729e1fe465da7904001
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.6 MB (115601563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31f5dfdc32269a08b775b7b18972781651a1103e34bb2eb596fda4bcd843f1af`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 01:59:07 GMT
ADD file:43b45f65ff4ba720f6f9a107b5f80818d5ea6ebc4835840b11e9a506351da32f in / 
# Wed, 17 Nov 2021 01:59:08 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:41:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:42:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 02:43:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dbbf55137aab3c7acd1e012a70f1ea1adeaef8d39b474829965d3480a02bf572`  
		Last Modified: Wed, 17 Nov 2021 02:14:27 GMT  
		Size: 50.1 MB (50134152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb1ae7a04cee77523f9e09a62b28632c56a700d0c481be7cddc566c835e7a71d`  
		Last Modified: Wed, 17 Nov 2021 03:04:13 GMT  
		Size: 4.9 MB (4922782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66894dfea839186e94448f6c25a37c6b3b1b42cece6332cc9d36336917e18a4`  
		Last Modified: Wed, 17 Nov 2021 03:04:14 GMT  
		Size: 10.2 MB (10216965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4502933ba6aa2071501257e094faa363699dc23995f798a124d688c2523240af`  
		Last Modified: Wed, 17 Nov 2021 03:05:05 GMT  
		Size: 50.3 MB (50327664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d98321260829308a2348a158000abedf1fcd03e58d44ac414c3d077d1c110c70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.9 MB (123882237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32fa5708561ca81a99850197b076caf6f432ccb91bee5a5df1a4e6a478d3ec3f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:59 GMT
ADD file:eb667e18226da8a1ca5a41beacddc65cd1efec01c3d01e50845c5e89e91ea17c in / 
# Wed, 17 Nov 2021 02:40:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:26:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:26:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:27:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce18cd0ba11c2dfa8c1a2d2b325e1e019b14d4ae25ffdeffb0f9686c5496bf5c`  
		Last Modified: Wed, 17 Nov 2021 02:46:45 GMT  
		Size: 53.6 MB (53619024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f138a340a2373acc72dcc4ea9ef08bdf5648aabc5fe08f7e8d25222ca63b7ee`  
		Last Modified: Wed, 17 Nov 2021 13:36:26 GMT  
		Size: 4.9 MB (4937639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34c030205ccb8656e30a58f96bb1edbe7c59bf17f3329ae3c442ec897f2b270`  
		Last Modified: Wed, 17 Nov 2021 13:36:27 GMT  
		Size: 10.7 MB (10655878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7a1cfcc2070fbe1e702751d85f7074b93d142f6beb03ef66e9ba1c58bcc3e3`  
		Last Modified: Wed, 17 Nov 2021 13:36:49 GMT  
		Size: 54.7 MB (54669696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:16abe77eeca3b6e96cff6cf2bbff639647cf581d03efc6c7dcb8ab3fb5fa8bd2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128374671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:363c0a8d58ad2bab650032b97601a821766dc54ba78827525e9e45381d993d08`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:39:30 GMT
ADD file:e007d6eff02dbc696e1166db315b97a77ae8aa65f2e66ca8074765dde9c70a59 in / 
# Tue, 12 Oct 2021 01:39:31 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:35:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:36:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 04:36:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6911c8f66691266d86e2cafa67ca005d919f357436fac971c694d37625b5ba90`  
		Last Modified: Tue, 12 Oct 2021 01:47:06 GMT  
		Size: 55.9 MB (55923419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a0f31369a20c178b1d5c84f192412ed962068e8932d5821eefb00bc7d1cbc1a`  
		Last Modified: Tue, 12 Oct 2021 04:47:26 GMT  
		Size: 5.3 MB (5283102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97aa3d222d7e8d6e0b06e57e5bd03168c422475942f92d09a487bd98d09bb742`  
		Last Modified: Tue, 12 Oct 2021 04:47:27 GMT  
		Size: 11.3 MB (11250699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae99d06bab5fc31ba3db9436a22c452db74a7b5e559a451de2d971a493abe52`  
		Last Modified: Tue, 12 Oct 2021 04:48:03 GMT  
		Size: 55.9 MB (55917451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:a5be5277770524bd35dd921bc7f03adf64d8bf76eeee88ba1a6fb10f62aa65a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.5 MB (122468694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afe05d4524b16661e35a811e3b2f3a1ea3e0fc1ca56eb4306839c755f24c34ef`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:09:46 GMT
ADD file:2971df49f24648b8d5166d87e392e2547d5b03469356f20d112ce6feb3c329fc in / 
# Wed, 17 Nov 2021 02:09:47 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:29:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:30:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 08:31:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b095a0b63d99a4c4cd9c1c353f381a69ef041e6f80798d807ae51a34b04920a0`  
		Last Modified: Wed, 17 Nov 2021 02:18:22 GMT  
		Size: 53.2 MB (53183806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2e37aff1692726b1ea3dd0b4eeb684072527295f8e981d3c45825327daea19`  
		Last Modified: Wed, 17 Nov 2021 08:45:38 GMT  
		Size: 5.1 MB (5114925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d4c0302ddd7a6cb573a156076dba9c593e09a0c321b32ae0f1da2bd36bc754`  
		Last Modified: Wed, 17 Nov 2021 08:45:41 GMT  
		Size: 10.9 MB (10873360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cde5eca075420fcfc6498f454dc040f1e236dea180a82a0d27d7a739ffd41c1`  
		Last Modified: Wed, 17 Nov 2021 08:46:32 GMT  
		Size: 53.3 MB (53296603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:faf4c1b1a0373960c09ef3f862d4fcd8e9c6bc9b842a86cdf1ab3405f45a9f3c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134698979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b960badc27a250634b2e76a6871d276d149dcd0fe0fe615bbf2f54db9efc221b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 03:27:04 GMT
ADD file:85375acb19da58f9eabaa67f8cb425cd1ff2dadb2888bbd9dbfa6223d16fef23 in / 
# Wed, 17 Nov 2021 03:27:20 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 07:40:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 07:40:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 07:42:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ede9cd7c8f1d380c971a130fb3d8a3914bf3a9106702164c23b2cce536fa618c`  
		Last Modified: Wed, 17 Nov 2021 03:52:39 GMT  
		Size: 58.8 MB (58819505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743814bfd79326104da0238d8edced6b14f63b95734b6dc0e2b7a9d83356b0cb`  
		Last Modified: Wed, 17 Nov 2021 08:25:58 GMT  
		Size: 5.4 MB (5402000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca978d94a6543bbd1c60026602b64e810b4bf65e052dcf19adf2b4d6b518bf8`  
		Last Modified: Wed, 17 Nov 2021 08:25:59 GMT  
		Size: 11.6 MB (11626016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d785f1d8909cb3a3e46844611c28e15781da809be0073e40af017d6e5631d0`  
		Last Modified: Wed, 17 Nov 2021 08:26:57 GMT  
		Size: 58.9 MB (58851458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:673b0a54f0e03e540c534b0dfc3525d90049ec556ed645e24d83e7eaa1dd159f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123147032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ec10947074405be072d3cee591cea9230aa7dd19dafc623039d1644d6083ca4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:07 GMT
ADD file:b7524e775a2033d246d1096765a0eb6eaa5ba6ed6c8b395522579d2c4e7a2e38 in / 
# Wed, 17 Nov 2021 02:42:09 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:07:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:07:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:08:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ffa47acd07831fbc96680a705da20704bac0016c20dc3c454ecd45cda44b368d`  
		Last Modified: Wed, 17 Nov 2021 02:48:05 GMT  
		Size: 53.2 MB (53207179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c950336719691da019c99e4ff78fe559ab0308ea145757994bdb7be34c6d224`  
		Last Modified: Wed, 17 Nov 2021 03:17:18 GMT  
		Size: 5.1 MB (5137199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d769af2ca44d1c7c206e7190cd71df7cb5ff3df2dd45e1dd52ea447ffb547b1a`  
		Last Modified: Wed, 17 Nov 2021 03:17:19 GMT  
		Size: 10.8 MB (10761499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3bbc68017b41a8cc07b10d715e2a23108c5addefa80b01cac1a2ef075bb1acd`  
		Last Modified: Wed, 17 Nov 2021 03:17:36 GMT  
		Size: 54.0 MB (54041155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:buster`

```console
$ docker pull buildpack-deps@sha256:33cb41bdc60ac651ee2fb97714dc86af89bf1cf52fb8827f350aff333ddcd490
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
$ docker pull buildpack-deps@sha256:40214612fb01ceeb7860226a8a782a8d50a4850847f78981cf364d8084d147de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.5 MB (312533991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0413fe230a75e8ed7ab2771c02492189116b86729fd184bba5339a1bac348050`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:51 GMT
ADD file:cb5ed7070880d4c0177fbe6dd278adb7926e38cd73e6abd582fd8d67e4bbf06c in / 
# Wed, 17 Nov 2021 02:20:51 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:15:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:15:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:16:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:17:16 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1230f17f526cb07307d41462355b10488b994e8bdafe0d8f275a405fa3b33831`  
		Last Modified: Wed, 17 Nov 2021 02:26:06 GMT  
		Size: 50.4 MB (50437098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17d0de332ca1b34d53ca41c2b39ea52ce72f8c1e81c5200e27a8bade3e6ecbb`  
		Last Modified: Wed, 17 Nov 2021 03:24:34 GMT  
		Size: 7.8 MB (7833787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7474d56348f5333567750c1e5f06f899477fd437330627341eafa71bfa1a36ab`  
		Last Modified: Wed, 17 Nov 2021 03:24:34 GMT  
		Size: 10.0 MB (9997183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211c565de40518c5dac4498ccebbf3833fcfaa5db17d4bf94e6bef466136278b`  
		Last Modified: Wed, 17 Nov 2021 03:24:55 GMT  
		Size: 51.8 MB (51840474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71337a3dfc6f79fe42b06f2f3872667ca6d9ebac8029afcf6df3b0ee321f509f`  
		Last Modified: Wed, 17 Nov 2021 03:25:36 GMT  
		Size: 192.4 MB (192425449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:992531625663e82ea52458ff2a822637f40c4e415c9b30c62882cc47da243925
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.1 MB (286144717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea6ba2c3224423f294f623719618096fa1d795d97560237193e8196cb8ab8d61`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 00:50:58 GMT
ADD file:f9432d6da0faddeaa117c57c0c007cd56738ef01549baf71e5c59939b7e69b6c in / 
# Tue, 12 Oct 2021 00:50:59 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:45:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:45:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 05:46:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:48:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ae00de77d9c27fe3ba9ea06833b273e4fc0aa128a3a61d3992632e6e3941a78c`  
		Last Modified: Tue, 12 Oct 2021 01:07:01 GMT  
		Size: 48.2 MB (48154085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52282bf2103fc337ab7cc23ebfae979096e6f901b62960b03952c2d52e9978db`  
		Last Modified: Tue, 12 Oct 2021 06:04:31 GMT  
		Size: 7.4 MB (7377193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b1aa5c1e770fff74bdcd066b443f1e1e49f677ae77ec80d22c50e20be8c3b3`  
		Last Modified: Tue, 12 Oct 2021 06:04:32 GMT  
		Size: 9.7 MB (9687494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b03f47e60dacc119379be5c6a6d690ee9ebe00c3a3f7755e295b572e9d4817aa`  
		Last Modified: Tue, 12 Oct 2021 06:05:19 GMT  
		Size: 49.6 MB (49574809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f680c95108ec6b108b9dcd987cc473d268506328d38866d5b6aa0e44ff73c8dd`  
		Last Modified: Tue, 12 Oct 2021 06:07:13 GMT  
		Size: 171.4 MB (171351136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:b7df7895ed903ba0d50d3c0b59280a0b329ac98b9b89a1997c0a1db9cdba9b31
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.4 MB (278351711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3172590d3c7dc0fb07cd01d18ebc7811c421c9409f6f8624ff870b62a5a0351e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:00:12 GMT
ADD file:d71807613acdf86685f6d640a90e27b7b63cfe0f13d88668ee943aca089d8876 in / 
# Wed, 17 Nov 2021 02:00:13 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:45:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:45:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 02:46:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:48:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10acd81022d17f452439d0385615fa066b8f0ddcf3c1a803872eec5bdc6acf64`  
		Last Modified: Wed, 17 Nov 2021 02:16:00 GMT  
		Size: 45.9 MB (45918099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a9604eb6c465f658d6422593d504030155029fe0c4302451d4369030c29144`  
		Last Modified: Wed, 17 Nov 2021 03:07:14 GMT  
		Size: 7.1 MB (7125194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b043b954c4f0757e89df96897cea2cf1f93c6275466008e4ba7a4b1089c7dd3d`  
		Last Modified: Wed, 17 Nov 2021 03:07:15 GMT  
		Size: 9.3 MB (9343839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf41461745fd89900c4b7cc794c93de081420bd83223b46e1495ff96748685c`  
		Last Modified: Wed, 17 Nov 2021 03:07:59 GMT  
		Size: 47.4 MB (47356485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4cebe2126c416f6186078f6b19742a166f0d535016a910ed5bd1bed73ab5ab`  
		Last Modified: Wed, 17 Nov 2021 03:09:46 GMT  
		Size: 168.6 MB (168608094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a781bc03f60fd23b4f3bc527115eae336c4406da469a32b05e5a8cb879285c0c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.8 MB (302842791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d89bb85d03bfdc93c6f242b95047eda9fd8a32f57973d9615c0bf809eb00c27f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:27 GMT
ADD file:c7e9e884b1494f96e33e9d9a892b51367af8943edb282c4101cc99ea78a7753f in / 
# Wed, 17 Nov 2021 02:40:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:28:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:28:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:28:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:29:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:626979e62c56e192812e818d52b82f063d9f9514b1b7bae14e534e4a7c98117a`  
		Last Modified: Wed, 17 Nov 2021 02:47:40 GMT  
		Size: 49.2 MB (49222990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134a528370d5dcbf5b6ba2d8c20f576504448e8f2d1debb5d2a4950a38a3ff2d`  
		Last Modified: Wed, 17 Nov 2021 13:37:44 GMT  
		Size: 7.7 MB (7695161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e12e3364b52ad043d8e79f750863ed4ca2878c4fdf45ded974508febc55fdd`  
		Last Modified: Wed, 17 Nov 2021 13:37:44 GMT  
		Size: 9.8 MB (9767133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a7f2500f9574b0a495bfb031c2d52e83c96dd545ef2185737f8032567e70677`  
		Last Modified: Wed, 17 Nov 2021 13:38:03 GMT  
		Size: 52.2 MB (52165947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16922d4fa4f2c649c56a586e06135309b0cc7e160a17c909e5eb349988df61aa`  
		Last Modified: Wed, 17 Nov 2021 13:38:38 GMT  
		Size: 184.0 MB (183991560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; 386

```console
$ docker pull buildpack-deps@sha256:07a84d8bf937d4befea7f1d2878f2f7b46a31fdc00d5d6891072304ae83b4d06
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.9 MB (321944968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00f2f20bac236128ca2d426c71e0fc49ae840c119b299d797809f4c224bc7948`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:40:01 GMT
ADD file:1461fa0362c70b5b7a677c57dd48633827fd9635a9cb136730aa7581cc523b46 in / 
# Tue, 12 Oct 2021 01:40:02 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:37:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:38:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 04:38:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:39:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f4b233498baa64e956a5f70979351e206bd085bd547a3cf25c08b154348df726`  
		Last Modified: Tue, 12 Oct 2021 01:48:07 GMT  
		Size: 51.2 MB (51207606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece122ff48522de249e81ee22f617bf84d59b003d3c79f44331163046a937e4c`  
		Last Modified: Tue, 12 Oct 2021 04:49:37 GMT  
		Size: 8.0 MB (8000221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:378307f52e8eeddb964324804377cd9fd65b1bf7b848c5b690e63ef92f1fe3d5`  
		Last Modified: Tue, 12 Oct 2021 04:49:37 GMT  
		Size: 10.3 MB (10339916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559cdd7287c6a9a0f142216d3645f886b4a777073daae85c51de968330bb9f9d`  
		Last Modified: Tue, 12 Oct 2021 04:50:08 GMT  
		Size: 53.4 MB (53437801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:325db7f1d3dd664f85cad29c0867f78c550d2b5c426ed460bf5283c008942bb6`  
		Last Modified: Tue, 12 Oct 2021 04:50:59 GMT  
		Size: 199.0 MB (198959424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:30c758f087fd5312ed4d5cfbda2905fd550e0d3738afdeb1030499c4f12a1ccc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.1 MB (297128262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c90dc68a1536bdf0771a84535d0ccf2a3e57ae0ac87df32c471fe9265da620b0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:10:39 GMT
ADD file:4769a173ec92e69a1b5cd79af0ed018bf150d1ee278de07f4bdab45f55f3c818 in / 
# Wed, 17 Nov 2021 02:10:40 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:34:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:34:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 08:36:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:39:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8c028c43f55209ca75650433b923c8952e16d106529242daad16c3be3efd66a3`  
		Last Modified: Wed, 17 Nov 2021 02:19:53 GMT  
		Size: 49.1 MB (49079535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:762a68d988b283d25c4ea122ea03a45caa2b4174b9d1df992298cef4bc15678f`  
		Last Modified: Wed, 17 Nov 2021 08:48:59 GMT  
		Size: 7.3 MB (7253673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a792c079b6714bc5d104fd824622583cd79ee86bf0cd4bd3930290e5bea3a81`  
		Last Modified: Wed, 17 Nov 2021 08:48:59 GMT  
		Size: 10.0 MB (10016437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0c1cd6c6ead61c438a2c08e4c9cc9d3c5ff225d437de4052cd5b03699bdae3`  
		Last Modified: Wed, 17 Nov 2021 08:49:46 GMT  
		Size: 50.8 MB (50844942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4347eaf923b6e261b09fec9e7c6e3e06fee0595ef1609e0e9f25be6a2b8428`  
		Last Modified: Wed, 17 Nov 2021 08:51:52 GMT  
		Size: 179.9 MB (179933675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:b87c8fcad8f67a37fdb8dd3764fdcc849043fe943f3f5ac261f37c0aed85d80e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.9 MB (333943769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30105f5450a73d27a5f54e7976ea986d267e0f70bccf47c138963ac685d08dc2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 03:29:10 GMT
ADD file:fc0d43ba74311deef20b2131cca3a8e86b083624d63560251191adca21417f2f in / 
# Wed, 17 Nov 2021 03:29:20 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 07:52:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 07:53:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 07:55:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:06:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:aad6e1fe6f7c56b0e1b5850f40e4fec91ffaed4b6235e730f5c7ff43db397d3d`  
		Last Modified: Wed, 17 Nov 2021 03:56:39 GMT  
		Size: 54.2 MB (54183702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38c773e3945e9939b7299519ac8a7f3ad909af69c2d7291d8dfb6e7fa6eccfe`  
		Last Modified: Wed, 17 Nov 2021 08:28:50 GMT  
		Size: 8.3 MB (8272985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65e0d54cc06e26d154b6f6e9746c8de2af93d9f635c280336663372f382fcd46`  
		Last Modified: Wed, 17 Nov 2021 08:28:49 GMT  
		Size: 10.7 MB (10727776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3239f513a520f7d81f241b123128d80a0c91d3ef8697270ffae67898934cb4f9`  
		Last Modified: Wed, 17 Nov 2021 08:29:36 GMT  
		Size: 57.5 MB (57457385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f80735649ead4029d67b9d28dac87b66bb06e2548f5c0d68c5f9877855d41c`  
		Last Modified: Wed, 17 Nov 2021 08:31:23 GMT  
		Size: 203.3 MB (203301921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:2a549a62e97fa58428a04001462c87f88b3fa92be5fcce03ca6280f6de3c9e46
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.6 MB (294582808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a55feeaee694c81b717cd5fcae296288c5700416bf32d57d56cc2249119570da`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:40 GMT
ADD file:dc4ee96f81059accdc88a686f80f1714bc9d2f383af71c0d130c08560cea115e in / 
# Wed, 17 Nov 2021 02:42:42 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:10:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:10:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:10:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:11:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c12eae84d2674466d924a139a276e361afa9f63de21cf77eae19bd94eaac2629`  
		Last Modified: Wed, 17 Nov 2021 02:48:42 GMT  
		Size: 49.0 MB (49005439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564a8b4bf4cf08933f04084cd556e9c716474b9801854ea7c4473c9804894516`  
		Last Modified: Wed, 17 Nov 2021 03:18:14 GMT  
		Size: 7.4 MB (7401273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ffdc4b0bb501f5f5214892baa1a5d53d44ce92b645995a43fe2cfeb2ffec6d1`  
		Last Modified: Wed, 17 Nov 2021 03:18:14 GMT  
		Size: 9.9 MB (9883156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb48942b4b14ee80905b23bc6babae28a961847a914becfe41686d368d8693d`  
		Last Modified: Wed, 17 Nov 2021 03:18:28 GMT  
		Size: 51.4 MB (51380227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3deaef082aa42f5164fd0beb9cf445ba4867c9ad41c784080a427bc615a02df9`  
		Last Modified: Wed, 17 Nov 2021 03:18:54 GMT  
		Size: 176.9 MB (176912713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:buster-curl`

```console
$ docker pull buildpack-deps@sha256:d58c6560d64100478b91c5a36db1baa7299fd98f69cba651c222abd37b5b6396
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
$ docker pull buildpack-deps@sha256:a0bba8f1fd79022a347c88c8ba94f43b7b9a85b2a241a977a2d15ff65f3b9974
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68268068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae7b4dd26afae147336976cacba2d6de091e5f31ce99148eadb745564c75cdf8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:51 GMT
ADD file:cb5ed7070880d4c0177fbe6dd278adb7926e38cd73e6abd582fd8d67e4bbf06c in / 
# Wed, 17 Nov 2021 02:20:51 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:15:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:15:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1230f17f526cb07307d41462355b10488b994e8bdafe0d8f275a405fa3b33831`  
		Last Modified: Wed, 17 Nov 2021 02:26:06 GMT  
		Size: 50.4 MB (50437098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17d0de332ca1b34d53ca41c2b39ea52ce72f8c1e81c5200e27a8bade3e6ecbb`  
		Last Modified: Wed, 17 Nov 2021 03:24:34 GMT  
		Size: 7.8 MB (7833787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7474d56348f5333567750c1e5f06f899477fd437330627341eafa71bfa1a36ab`  
		Last Modified: Wed, 17 Nov 2021 03:24:34 GMT  
		Size: 10.0 MB (9997183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:b140abc457f97daff918385b366ef37a61f11bd24028a0f05be0fd904723f38c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65218772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ca71e57b57c8f55f460a4ef80141da4552e2dd1317eccfae4a8f32e70126712`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 00:50:58 GMT
ADD file:f9432d6da0faddeaa117c57c0c007cd56738ef01549baf71e5c59939b7e69b6c in / 
# Tue, 12 Oct 2021 00:50:59 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:45:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:45:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ae00de77d9c27fe3ba9ea06833b273e4fc0aa128a3a61d3992632e6e3941a78c`  
		Last Modified: Tue, 12 Oct 2021 01:07:01 GMT  
		Size: 48.2 MB (48154085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52282bf2103fc337ab7cc23ebfae979096e6f901b62960b03952c2d52e9978db`  
		Last Modified: Tue, 12 Oct 2021 06:04:31 GMT  
		Size: 7.4 MB (7377193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b1aa5c1e770fff74bdcd066b443f1e1e49f677ae77ec80d22c50e20be8c3b3`  
		Last Modified: Tue, 12 Oct 2021 06:04:32 GMT  
		Size: 9.7 MB (9687494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:e724e938ae162d22679aa13688acc32788d5193b4f552dfd33702ad1843e3bc7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62387132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b37d37a14a96bf4731ecee8b62e9002e52f378b5a25d0f6668dbc7a96554394a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:00:12 GMT
ADD file:d71807613acdf86685f6d640a90e27b7b63cfe0f13d88668ee943aca089d8876 in / 
# Wed, 17 Nov 2021 02:00:13 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:45:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:45:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:10acd81022d17f452439d0385615fa066b8f0ddcf3c1a803872eec5bdc6acf64`  
		Last Modified: Wed, 17 Nov 2021 02:16:00 GMT  
		Size: 45.9 MB (45918099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a9604eb6c465f658d6422593d504030155029fe0c4302451d4369030c29144`  
		Last Modified: Wed, 17 Nov 2021 03:07:14 GMT  
		Size: 7.1 MB (7125194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b043b954c4f0757e89df96897cea2cf1f93c6275466008e4ba7a4b1089c7dd3d`  
		Last Modified: Wed, 17 Nov 2021 03:07:15 GMT  
		Size: 9.3 MB (9343839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:10f1a26aec27e58769c26f86b48604d74076ae1af479444ae540e2b73260466b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66685284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af10d3fa6817ac70b7abf7cf182c08ca8c2e382178327e9aaf6bf86ea8ebccf5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:27 GMT
ADD file:c7e9e884b1494f96e33e9d9a892b51367af8943edb282c4101cc99ea78a7753f in / 
# Wed, 17 Nov 2021 02:40:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:28:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:28:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:626979e62c56e192812e818d52b82f063d9f9514b1b7bae14e534e4a7c98117a`  
		Last Modified: Wed, 17 Nov 2021 02:47:40 GMT  
		Size: 49.2 MB (49222990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134a528370d5dcbf5b6ba2d8c20f576504448e8f2d1debb5d2a4950a38a3ff2d`  
		Last Modified: Wed, 17 Nov 2021 13:37:44 GMT  
		Size: 7.7 MB (7695161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e12e3364b52ad043d8e79f750863ed4ca2878c4fdf45ded974508febc55fdd`  
		Last Modified: Wed, 17 Nov 2021 13:37:44 GMT  
		Size: 9.8 MB (9767133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:2486e26715fffc0103cff821dabfb04a4065f77b779ab7740ee9ef68bf6628bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69547743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eddce9da46d7c9304a8b60a2eea1e90ec1647b65c857487a9d68b7bb1635d413`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:40:01 GMT
ADD file:1461fa0362c70b5b7a677c57dd48633827fd9635a9cb136730aa7581cc523b46 in / 
# Tue, 12 Oct 2021 01:40:02 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:37:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:38:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f4b233498baa64e956a5f70979351e206bd085bd547a3cf25c08b154348df726`  
		Last Modified: Tue, 12 Oct 2021 01:48:07 GMT  
		Size: 51.2 MB (51207606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece122ff48522de249e81ee22f617bf84d59b003d3c79f44331163046a937e4c`  
		Last Modified: Tue, 12 Oct 2021 04:49:37 GMT  
		Size: 8.0 MB (8000221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:378307f52e8eeddb964324804377cd9fd65b1bf7b848c5b690e63ef92f1fe3d5`  
		Last Modified: Tue, 12 Oct 2021 04:49:37 GMT  
		Size: 10.3 MB (10339916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:7c61cd32ed32b3b639ddb2468350c4b45a105bc0f5c2e23daa4aa97ded77e997
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66349645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9969b21b9718be805e11858a4a3a51a6bfb015e4b3d34d1c36cd3b7571ec5119`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:10:39 GMT
ADD file:4769a173ec92e69a1b5cd79af0ed018bf150d1ee278de07f4bdab45f55f3c818 in / 
# Wed, 17 Nov 2021 02:10:40 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:34:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:34:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8c028c43f55209ca75650433b923c8952e16d106529242daad16c3be3efd66a3`  
		Last Modified: Wed, 17 Nov 2021 02:19:53 GMT  
		Size: 49.1 MB (49079535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:762a68d988b283d25c4ea122ea03a45caa2b4174b9d1df992298cef4bc15678f`  
		Last Modified: Wed, 17 Nov 2021 08:48:59 GMT  
		Size: 7.3 MB (7253673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a792c079b6714bc5d104fd824622583cd79ee86bf0cd4bd3930290e5bea3a81`  
		Last Modified: Wed, 17 Nov 2021 08:48:59 GMT  
		Size: 10.0 MB (10016437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:93ced9b6d18e78790cbd7fda169627b5233452d7cc6896e6d819d3fb0662f4c4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73184463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:804b950ad439852a9015c271a4046743a5293839cf6d652ded639eceefbc214c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 03:29:10 GMT
ADD file:fc0d43ba74311deef20b2131cca3a8e86b083624d63560251191adca21417f2f in / 
# Wed, 17 Nov 2021 03:29:20 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 07:52:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 07:53:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:aad6e1fe6f7c56b0e1b5850f40e4fec91ffaed4b6235e730f5c7ff43db397d3d`  
		Last Modified: Wed, 17 Nov 2021 03:56:39 GMT  
		Size: 54.2 MB (54183702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38c773e3945e9939b7299519ac8a7f3ad909af69c2d7291d8dfb6e7fa6eccfe`  
		Last Modified: Wed, 17 Nov 2021 08:28:50 GMT  
		Size: 8.3 MB (8272985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65e0d54cc06e26d154b6f6e9746c8de2af93d9f635c280336663372f382fcd46`  
		Last Modified: Wed, 17 Nov 2021 08:28:49 GMT  
		Size: 10.7 MB (10727776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:2f148905d6fe03767f7cb6e8c4fcbd6b5a200f0a6b8a9907394dc5154a203300
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66289868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65862f040a1b0973ae86d1e0f56a13ec80e7c12e566a3f87dab7af1ec5238448`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:40 GMT
ADD file:dc4ee96f81059accdc88a686f80f1714bc9d2f383af71c0d130c08560cea115e in / 
# Wed, 17 Nov 2021 02:42:42 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:10:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:10:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c12eae84d2674466d924a139a276e361afa9f63de21cf77eae19bd94eaac2629`  
		Last Modified: Wed, 17 Nov 2021 02:48:42 GMT  
		Size: 49.0 MB (49005439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564a8b4bf4cf08933f04084cd556e9c716474b9801854ea7c4473c9804894516`  
		Last Modified: Wed, 17 Nov 2021 03:18:14 GMT  
		Size: 7.4 MB (7401273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ffdc4b0bb501f5f5214892baa1a5d53d44ce92b645995a43fe2cfeb2ffec6d1`  
		Last Modified: Wed, 17 Nov 2021 03:18:14 GMT  
		Size: 9.9 MB (9883156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:buster-scm`

```console
$ docker pull buildpack-deps@sha256:b50bfcdde34728e1f8ba9ac0c1d1fcd44c4959a97b1577ae54a856fc2295f917
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
$ docker pull buildpack-deps@sha256:b024630c704ae32d7b5d99d3665a0a8e2d56001e59cfa84c36e9e2228c358dbe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120108542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c6e8b3f9456db8dd890d42a41fcb77c190b0d283f8ca01f471e275d1c209d6b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:51 GMT
ADD file:cb5ed7070880d4c0177fbe6dd278adb7926e38cd73e6abd582fd8d67e4bbf06c in / 
# Wed, 17 Nov 2021 02:20:51 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:15:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:15:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:16:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1230f17f526cb07307d41462355b10488b994e8bdafe0d8f275a405fa3b33831`  
		Last Modified: Wed, 17 Nov 2021 02:26:06 GMT  
		Size: 50.4 MB (50437098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17d0de332ca1b34d53ca41c2b39ea52ce72f8c1e81c5200e27a8bade3e6ecbb`  
		Last Modified: Wed, 17 Nov 2021 03:24:34 GMT  
		Size: 7.8 MB (7833787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7474d56348f5333567750c1e5f06f899477fd437330627341eafa71bfa1a36ab`  
		Last Modified: Wed, 17 Nov 2021 03:24:34 GMT  
		Size: 10.0 MB (9997183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211c565de40518c5dac4498ccebbf3833fcfaa5db17d4bf94e6bef466136278b`  
		Last Modified: Wed, 17 Nov 2021 03:24:55 GMT  
		Size: 51.8 MB (51840474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:80937d7a95e48544fa440d8ff13fc0b9d30ec833fad447077c9e608976313fe0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114793581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ba5c3d966befcbb226c6a48c41f0915d5314c95ec5b05b6da617cbe79855c80`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 00:50:58 GMT
ADD file:f9432d6da0faddeaa117c57c0c007cd56738ef01549baf71e5c59939b7e69b6c in / 
# Tue, 12 Oct 2021 00:50:59 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:45:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:45:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 05:46:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ae00de77d9c27fe3ba9ea06833b273e4fc0aa128a3a61d3992632e6e3941a78c`  
		Last Modified: Tue, 12 Oct 2021 01:07:01 GMT  
		Size: 48.2 MB (48154085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52282bf2103fc337ab7cc23ebfae979096e6f901b62960b03952c2d52e9978db`  
		Last Modified: Tue, 12 Oct 2021 06:04:31 GMT  
		Size: 7.4 MB (7377193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b1aa5c1e770fff74bdcd066b443f1e1e49f677ae77ec80d22c50e20be8c3b3`  
		Last Modified: Tue, 12 Oct 2021 06:04:32 GMT  
		Size: 9.7 MB (9687494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b03f47e60dacc119379be5c6a6d690ee9ebe00c3a3f7755e295b572e9d4817aa`  
		Last Modified: Tue, 12 Oct 2021 06:05:19 GMT  
		Size: 49.6 MB (49574809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:38e7ee8c93b1073e32b5e8444018fdf2fed12d6f0e0162718b120b70f00725bf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109743617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c99199676eacaf17a961d89b17bcf60f3ba4bcaa4bad06ab06550ed01003e885`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:00:12 GMT
ADD file:d71807613acdf86685f6d640a90e27b7b63cfe0f13d88668ee943aca089d8876 in / 
# Wed, 17 Nov 2021 02:00:13 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:45:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:45:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 02:46:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10acd81022d17f452439d0385615fa066b8f0ddcf3c1a803872eec5bdc6acf64`  
		Last Modified: Wed, 17 Nov 2021 02:16:00 GMT  
		Size: 45.9 MB (45918099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a9604eb6c465f658d6422593d504030155029fe0c4302451d4369030c29144`  
		Last Modified: Wed, 17 Nov 2021 03:07:14 GMT  
		Size: 7.1 MB (7125194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b043b954c4f0757e89df96897cea2cf1f93c6275466008e4ba7a4b1089c7dd3d`  
		Last Modified: Wed, 17 Nov 2021 03:07:15 GMT  
		Size: 9.3 MB (9343839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf41461745fd89900c4b7cc794c93de081420bd83223b46e1495ff96748685c`  
		Last Modified: Wed, 17 Nov 2021 03:07:59 GMT  
		Size: 47.4 MB (47356485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ae9e47c84e1cb304d5585a7cabe72277e995c683344e652437eae69be73404f4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.9 MB (118851231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16caaa63c991b5d1a70fd8dfded47c4d0a820cc1ec1de6dd0877379c7d244150`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:27 GMT
ADD file:c7e9e884b1494f96e33e9d9a892b51367af8943edb282c4101cc99ea78a7753f in / 
# Wed, 17 Nov 2021 02:40:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:28:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:28:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:28:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:626979e62c56e192812e818d52b82f063d9f9514b1b7bae14e534e4a7c98117a`  
		Last Modified: Wed, 17 Nov 2021 02:47:40 GMT  
		Size: 49.2 MB (49222990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134a528370d5dcbf5b6ba2d8c20f576504448e8f2d1debb5d2a4950a38a3ff2d`  
		Last Modified: Wed, 17 Nov 2021 13:37:44 GMT  
		Size: 7.7 MB (7695161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e12e3364b52ad043d8e79f750863ed4ca2878c4fdf45ded974508febc55fdd`  
		Last Modified: Wed, 17 Nov 2021 13:37:44 GMT  
		Size: 9.8 MB (9767133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a7f2500f9574b0a495bfb031c2d52e83c96dd545ef2185737f8032567e70677`  
		Last Modified: Wed, 17 Nov 2021 13:38:03 GMT  
		Size: 52.2 MB (52165947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:0d0d9bd21ec4cf4c15da749cd2dace32bc7a91f60d2e70dea7636c686c0c197f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (122985544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b468e2beeabc6c15ba9fdf021ec223e3ba84fc3ea63cceb1a4d97d4c4553232a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:40:01 GMT
ADD file:1461fa0362c70b5b7a677c57dd48633827fd9635a9cb136730aa7581cc523b46 in / 
# Tue, 12 Oct 2021 01:40:02 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:37:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:38:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 04:38:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f4b233498baa64e956a5f70979351e206bd085bd547a3cf25c08b154348df726`  
		Last Modified: Tue, 12 Oct 2021 01:48:07 GMT  
		Size: 51.2 MB (51207606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece122ff48522de249e81ee22f617bf84d59b003d3c79f44331163046a937e4c`  
		Last Modified: Tue, 12 Oct 2021 04:49:37 GMT  
		Size: 8.0 MB (8000221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:378307f52e8eeddb964324804377cd9fd65b1bf7b848c5b690e63ef92f1fe3d5`  
		Last Modified: Tue, 12 Oct 2021 04:49:37 GMT  
		Size: 10.3 MB (10339916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559cdd7287c6a9a0f142216d3645f886b4a777073daae85c51de968330bb9f9d`  
		Last Modified: Tue, 12 Oct 2021 04:50:08 GMT  
		Size: 53.4 MB (53437801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:2bce12967fadf2de5d6317e7098ce12b55856bf06a7037fb2fd24422a4e81e88
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.2 MB (117194587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c9da7943e7aefd994faf5843414c15b9bec44d6c353d37797bd5a778b9cb19b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:10:39 GMT
ADD file:4769a173ec92e69a1b5cd79af0ed018bf150d1ee278de07f4bdab45f55f3c818 in / 
# Wed, 17 Nov 2021 02:10:40 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:34:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:34:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 08:36:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8c028c43f55209ca75650433b923c8952e16d106529242daad16c3be3efd66a3`  
		Last Modified: Wed, 17 Nov 2021 02:19:53 GMT  
		Size: 49.1 MB (49079535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:762a68d988b283d25c4ea122ea03a45caa2b4174b9d1df992298cef4bc15678f`  
		Last Modified: Wed, 17 Nov 2021 08:48:59 GMT  
		Size: 7.3 MB (7253673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a792c079b6714bc5d104fd824622583cd79ee86bf0cd4bd3930290e5bea3a81`  
		Last Modified: Wed, 17 Nov 2021 08:48:59 GMT  
		Size: 10.0 MB (10016437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0c1cd6c6ead61c438a2c08e4c9cc9d3c5ff225d437de4052cd5b03699bdae3`  
		Last Modified: Wed, 17 Nov 2021 08:49:46 GMT  
		Size: 50.8 MB (50844942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:369458b8d3ff683d522860c70940db01c7723d2d956ad0ec28cd3401b6db7c0c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.6 MB (130641848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60323d251a71f8deeea46542dac34070eb1f8f93ba89d8953ee518ea2ef6f9ae`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 03:29:10 GMT
ADD file:fc0d43ba74311deef20b2131cca3a8e86b083624d63560251191adca21417f2f in / 
# Wed, 17 Nov 2021 03:29:20 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 07:52:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 07:53:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 07:55:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:aad6e1fe6f7c56b0e1b5850f40e4fec91ffaed4b6235e730f5c7ff43db397d3d`  
		Last Modified: Wed, 17 Nov 2021 03:56:39 GMT  
		Size: 54.2 MB (54183702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38c773e3945e9939b7299519ac8a7f3ad909af69c2d7291d8dfb6e7fa6eccfe`  
		Last Modified: Wed, 17 Nov 2021 08:28:50 GMT  
		Size: 8.3 MB (8272985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65e0d54cc06e26d154b6f6e9746c8de2af93d9f635c280336663372f382fcd46`  
		Last Modified: Wed, 17 Nov 2021 08:28:49 GMT  
		Size: 10.7 MB (10727776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3239f513a520f7d81f241b123128d80a0c91d3ef8697270ffae67898934cb4f9`  
		Last Modified: Wed, 17 Nov 2021 08:29:36 GMT  
		Size: 57.5 MB (57457385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:f5e9778f889dea21e925be77a1a076e7f0c4589927b4612209c4db9b2bef5331
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117670095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fd015a72e8350a3bbb306e91dd17a1d82b36ee73f2c0b7348bda5ac13840988`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:40 GMT
ADD file:dc4ee96f81059accdc88a686f80f1714bc9d2f383af71c0d130c08560cea115e in / 
# Wed, 17 Nov 2021 02:42:42 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:10:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:10:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:10:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c12eae84d2674466d924a139a276e361afa9f63de21cf77eae19bd94eaac2629`  
		Last Modified: Wed, 17 Nov 2021 02:48:42 GMT  
		Size: 49.0 MB (49005439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564a8b4bf4cf08933f04084cd556e9c716474b9801854ea7c4473c9804894516`  
		Last Modified: Wed, 17 Nov 2021 03:18:14 GMT  
		Size: 7.4 MB (7401273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ffdc4b0bb501f5f5214892baa1a5d53d44ce92b645995a43fe2cfeb2ffec6d1`  
		Last Modified: Wed, 17 Nov 2021 03:18:14 GMT  
		Size: 9.9 MB (9883156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb48942b4b14ee80905b23bc6babae28a961847a914becfe41686d368d8693d`  
		Last Modified: Wed, 17 Nov 2021 03:18:28 GMT  
		Size: 51.4 MB (51380227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:curl`

```console
$ docker pull buildpack-deps@sha256:55e8b08399933366af5bf7339d286a42b69484a144be7a9505b9652bb3abc9d4
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
$ docker pull buildpack-deps@sha256:0edf02c125a1738634b314fe74509188fe8ec80d4fe0e5dcb6a8e2c69b752eda
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.0 MB (70957967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4210c06ad2290080f1e15b81fcab4884d6d092607663ed35830d2cb7f05d88df`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:8f64ae6a92bbcdf3bd87aa336ab8cfbe025c94f2871fb30c7c869ddf5b398637
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68087009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:452c0670207bd3308452b37f769e1991141d3955fb9c449d6651538516664d78`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 00:49:54 GMT
ADD file:b9969604315238de271e1769a4b8dd85cdf0d33f9fac387e940d5195ac3030a1 in / 
# Tue, 12 Oct 2021 00:49:55 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:40:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:41:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a97c782f2538791984ce12c859cada96e395e3950d4cb7d1238e08acd2eb74ec`  
		Last Modified: Tue, 12 Oct 2021 01:05:12 GMT  
		Size: 52.5 MB (52452198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34dc529b005dbeff70906cd4baf2310c918ae6379fdf53ef632c3cd1203aa38`  
		Last Modified: Tue, 12 Oct 2021 06:01:18 GMT  
		Size: 5.1 MB (5063794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2876b7f933f68a5b4f35f854cc8c651bf3d21476fe2bb0a786e6376f389b44b`  
		Last Modified: Tue, 12 Oct 2021 06:01:20 GMT  
		Size: 10.6 MB (10571017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:e0db5a4c0ddaf3021a476cd83cb48a47baae27cafc02c61fd6151c2b113034fd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65273899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a096ebca0a1dcf6c812935690d2f1ceba23cdc7565b5dedf1b01adb266c3296a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 01:59:07 GMT
ADD file:43b45f65ff4ba720f6f9a107b5f80818d5ea6ebc4835840b11e9a506351da32f in / 
# Wed, 17 Nov 2021 01:59:08 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:41:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:42:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:dbbf55137aab3c7acd1e012a70f1ea1adeaef8d39b474829965d3480a02bf572`  
		Last Modified: Wed, 17 Nov 2021 02:14:27 GMT  
		Size: 50.1 MB (50134152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb1ae7a04cee77523f9e09a62b28632c56a700d0c481be7cddc566c835e7a71d`  
		Last Modified: Wed, 17 Nov 2021 03:04:13 GMT  
		Size: 4.9 MB (4922782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66894dfea839186e94448f6c25a37c6b3b1b42cece6332cc9d36336917e18a4`  
		Last Modified: Wed, 17 Nov 2021 03:04:14 GMT  
		Size: 10.2 MB (10216965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c52337b05fa1f275820e562dc39597db3ec027dbc6930cd6c1424233776c385c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69212541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:638dd156261f84c328de4551fcff54679fa0628f7b63b62344e169cb0cfdf82c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:59 GMT
ADD file:eb667e18226da8a1ca5a41beacddc65cd1efec01c3d01e50845c5e89e91ea17c in / 
# Wed, 17 Nov 2021 02:40:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:26:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:26:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ce18cd0ba11c2dfa8c1a2d2b325e1e019b14d4ae25ffdeffb0f9686c5496bf5c`  
		Last Modified: Wed, 17 Nov 2021 02:46:45 GMT  
		Size: 53.6 MB (53619024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f138a340a2373acc72dcc4ea9ef08bdf5648aabc5fe08f7e8d25222ca63b7ee`  
		Last Modified: Wed, 17 Nov 2021 13:36:26 GMT  
		Size: 4.9 MB (4937639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34c030205ccb8656e30a58f96bb1edbe7c59bf17f3329ae3c442ec897f2b270`  
		Last Modified: Wed, 17 Nov 2021 13:36:27 GMT  
		Size: 10.7 MB (10655878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:307bd4c6b80d221cc5ffaa51a6561a19f142cbe2349df40cd823c45df8a66d0c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72457220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1fe930770d8d6583e5406717d0128e6efa4aa9438733ab028c7df182c036184`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:39:30 GMT
ADD file:e007d6eff02dbc696e1166db315b97a77ae8aa65f2e66ca8074765dde9c70a59 in / 
# Tue, 12 Oct 2021 01:39:31 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:35:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:36:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6911c8f66691266d86e2cafa67ca005d919f357436fac971c694d37625b5ba90`  
		Last Modified: Tue, 12 Oct 2021 01:47:06 GMT  
		Size: 55.9 MB (55923419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a0f31369a20c178b1d5c84f192412ed962068e8932d5821eefb00bc7d1cbc1a`  
		Last Modified: Tue, 12 Oct 2021 04:47:26 GMT  
		Size: 5.3 MB (5283102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97aa3d222d7e8d6e0b06e57e5bd03168c422475942f92d09a487bd98d09bb742`  
		Last Modified: Tue, 12 Oct 2021 04:47:27 GMT  
		Size: 11.3 MB (11250699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:c8e1c20d487b63fa0111dd8c6dbb3e8cad660d4ad92dfedcc288dbcf88b52ae1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69172091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e01b4e0250266355d14651090fbb68f4b5950f1e1e3e93ad45e1d024d3e8db78`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:09:46 GMT
ADD file:2971df49f24648b8d5166d87e392e2547d5b03469356f20d112ce6feb3c329fc in / 
# Wed, 17 Nov 2021 02:09:47 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:29:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:30:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b095a0b63d99a4c4cd9c1c353f381a69ef041e6f80798d807ae51a34b04920a0`  
		Last Modified: Wed, 17 Nov 2021 02:18:22 GMT  
		Size: 53.2 MB (53183806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2e37aff1692726b1ea3dd0b4eeb684072527295f8e981d3c45825327daea19`  
		Last Modified: Wed, 17 Nov 2021 08:45:38 GMT  
		Size: 5.1 MB (5114925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d4c0302ddd7a6cb573a156076dba9c593e09a0c321b32ae0f1da2bd36bc754`  
		Last Modified: Wed, 17 Nov 2021 08:45:41 GMT  
		Size: 10.9 MB (10873360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:ffc112a46cd4cb66176c5d7b815903b1652b33a26fb9f38d3233e1892293d496
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.8 MB (75847521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17cfe935fd31679e71de8a6756361a413d64351be692488a2fd6c0de16648ada`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 03:27:04 GMT
ADD file:85375acb19da58f9eabaa67f8cb425cd1ff2dadb2888bbd9dbfa6223d16fef23 in / 
# Wed, 17 Nov 2021 03:27:20 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 07:40:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 07:40:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ede9cd7c8f1d380c971a130fb3d8a3914bf3a9106702164c23b2cce536fa618c`  
		Last Modified: Wed, 17 Nov 2021 03:52:39 GMT  
		Size: 58.8 MB (58819505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743814bfd79326104da0238d8edced6b14f63b95734b6dc0e2b7a9d83356b0cb`  
		Last Modified: Wed, 17 Nov 2021 08:25:58 GMT  
		Size: 5.4 MB (5402000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca978d94a6543bbd1c60026602b64e810b4bf65e052dcf19adf2b4d6b518bf8`  
		Last Modified: Wed, 17 Nov 2021 08:25:59 GMT  
		Size: 11.6 MB (11626016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:864eebbaafc1154c0017d16100182a15ea13c7dd81a1e2474b581c03a8e4d27c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69105877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d1c13a820b2c0e693a7fcd87c7888df8a0f95367ff8e2381ec07faf8e711307`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:07 GMT
ADD file:b7524e775a2033d246d1096765a0eb6eaa5ba6ed6c8b395522579d2c4e7a2e38 in / 
# Wed, 17 Nov 2021 02:42:09 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:07:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:07:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ffa47acd07831fbc96680a705da20704bac0016c20dc3c454ecd45cda44b368d`  
		Last Modified: Wed, 17 Nov 2021 02:48:05 GMT  
		Size: 53.2 MB (53207179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c950336719691da019c99e4ff78fe559ab0308ea145757994bdb7be34c6d224`  
		Last Modified: Wed, 17 Nov 2021 03:17:18 GMT  
		Size: 5.1 MB (5137199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d769af2ca44d1c7c206e7190cd71df7cb5ff3df2dd45e1dd52ea447ffb547b1a`  
		Last Modified: Wed, 17 Nov 2021 03:17:19 GMT  
		Size: 10.8 MB (10761499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:focal`

```console
$ docker pull buildpack-deps@sha256:8046d17468dec05d82ec79681bf1c5e0f43ada1c2efd4222dd9d90023a226bc7
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
$ docker pull buildpack-deps@sha256:704e4e9e47293f392f16e1f74eb96784ee4ec426c416d006295e71856e550a9d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.8 MB (241796219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:701bdfc5b1f5072d2996e2f7a86ffd244192c9c42231d090abb7b8c44734cb03`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:43:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:43:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 01:44:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:47:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d2365e1e08bb86c1668a76475087cb6db5b42ba70cff99e936b0dda67d9215`  
		Last Modified: Sat, 16 Oct 2021 01:54:19 GMT  
		Size: 7.8 MB (7774998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577c425bc29205ed0c522c9332f7199d4e5805576b76cfa97ff9e345cdb268a5`  
		Last Modified: Sat, 16 Oct 2021 01:54:18 GMT  
		Size: 3.6 MB (3624513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fcda6c22ed5cb34aaea71f2bd9622535b40c91c4f8cc26f304720b510f9a6f`  
		Last Modified: Sat, 16 Oct 2021 01:54:38 GMT  
		Size: 60.7 MB (60722104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91046370e281131f8cd808e9fd0ec37c4f175001570c9196d54443154f9eaaa5`  
		Last Modified: Sat, 16 Oct 2021 01:55:07 GMT  
		Size: 141.1 MB (141107503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:4215ea236dbf14f9f94442857a9d9345f2fff063927f027cb9c724e78f76e6d5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.2 MB (207220779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78ce8d17eb298ae091fe14706ba52064dee049eb0d9a6f40dc060768396b945f`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:12:00 GMT
ADD file:625e3906181f4bd86e59a0e9748f67fcb1391a2e65e36c729e71353381a49757 in / 
# Sat, 16 Oct 2021 01:12:00 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:52:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:52:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 02:53:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:55:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8795d4da4abd6abcafe7285749aa85d3a164999e84720a3845f764e56e306771`  
		Last Modified: Sat, 16 Oct 2021 01:15:01 GMT  
		Size: 24.1 MB (24064451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a23aff9df2cf391d11feae54be8e82799a837823112a6dac845d32dc72eca02`  
		Last Modified: Sat, 16 Oct 2021 03:04:40 GMT  
		Size: 6.8 MB (6770106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce73020529e5c4c05a06cf469c45636d454253e819779803de574708312ec61`  
		Last Modified: Sat, 16 Oct 2021 03:04:37 GMT  
		Size: 3.1 MB (3104081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9998d3d2297827b1708a84f36e166391af9aecaafd91bf2d67b2dff8b1ad8a`  
		Last Modified: Sat, 16 Oct 2021 03:05:32 GMT  
		Size: 55.5 MB (55453746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fee38c0bd1ce11408a904c46f60d7de2595b0cda7b99bcbf74c2b5994bb1fad`  
		Last Modified: Sat, 16 Oct 2021 03:06:56 GMT  
		Size: 117.8 MB (117828395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a1b289eb033907eb4c99d514e204e8144577faee1302fed2fd86915bd0fa0c70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.5 MB (231499713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13278dccc5e41ca5c8bb7391753d4dd6554de1ad70743b7ca632257ea042f26f`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:06:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:06:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 03:06:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:07:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d32ba945c264e68ad0217898b4deb849a7b2b26d5877601d63d4545e29806e8`  
		Last Modified: Sat, 16 Oct 2021 03:20:27 GMT  
		Size: 7.6 MB (7639827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8491af4d3a3f4c7eace39c71ad3060a1909e99874d90b33647db45e9ce4482fa`  
		Last Modified: Sat, 16 Oct 2021 03:20:21 GMT  
		Size: 3.4 MB (3386522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cfb326f9da9ecc7f75c6f18d8aad46bf48677fba9bfb90d7d598271ee287959`  
		Last Modified: Sat, 16 Oct 2021 03:20:47 GMT  
		Size: 60.8 MB (60775123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dcedfdcd571b25c3f063cf324a265be0fbcf93e8208e31ccacb40a358cd4e11`  
		Last Modified: Sat, 16 Oct 2021 03:21:18 GMT  
		Size: 132.5 MB (132527341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:982eea1c9873499f87ffadcd10757d03ad62c3da04c72580d5ccff88fdfdfbca
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.4 MB (265361410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9424c0457501b56ce0517f9c6cca49b325fa99cc3f8c8d59fed4db28749bfba`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:36:38 GMT
ADD file:9246bf887411af1b286de95d779c11581dcef3c0d5a29e434162f0c085a7ce85 in / 
# Sat, 16 Oct 2021 00:36:44 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:08:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:09:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 01:11:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:17:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:77ba7971d651af68e20e7cbb6603a3f7acd8ef2893066767a93db104723556f2`  
		Last Modified: Sat, 16 Oct 2021 00:38:38 GMT  
		Size: 33.3 MB (33287238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b70bd5d2bc58b580d50736dbb70b528bdcd2910275584c8774c52efd29b8838`  
		Last Modified: Sat, 16 Oct 2021 01:29:38 GMT  
		Size: 8.7 MB (8728083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5e49a7fcde36f5b4cd0c87bace3ad307d0709d6942ff3ec27c5090922c1c7c`  
		Last Modified: Sat, 16 Oct 2021 01:29:16 GMT  
		Size: 4.5 MB (4456437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9332a33dc6df6ad95548ba3915b3a1235486dee9aacc7d13206604539866d440`  
		Last Modified: Sat, 16 Oct 2021 01:30:25 GMT  
		Size: 69.4 MB (69387759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b303db83d7ca2e64579e38fcb0676cf4f073f2f7a2f91e3088057f0b1a20a7`  
		Last Modified: Sat, 16 Oct 2021 01:31:04 GMT  
		Size: 149.5 MB (149501893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:451b83fcf3e41a5ee8bb7eabced23808496c11485d512282551948f7fa4f73b1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.6 MB (222629035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4bd65308571622b527359b75449d6e2a2a52e1563b6b374998b2462690dee78`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:41:46 GMT
ADD file:cf3b6f9c395392eaf2c629969f59c48cde60ae1c74c3dbb13886481999a7a4d5 in / 
# Sat, 16 Oct 2021 00:41:48 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:09:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:09:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 01:10:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:10:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1f0267805ccac7499fadaabf65e52d4564add2bc20ed25bcf77df24d8debb103`  
		Last Modified: Sat, 16 Oct 2021 00:42:57 GMT  
		Size: 27.1 MB (27120856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe453f45d32c58639c70b42127d12e8467533bc152ff663c5ffc8d0b5407293`  
		Last Modified: Sat, 16 Oct 2021 01:15:04 GMT  
		Size: 7.4 MB (7428503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df987c93c7f716b8ea845b480a00ccf4e4d962df89ed9f8cbefecdb1d9a96cf2`  
		Last Modified: Sat, 16 Oct 2021 01:15:03 GMT  
		Size: 3.5 MB (3542069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb4bb9db0d64c1d22f8065532581f6cdd28f20b4360950d6c5c3741db428c4f`  
		Last Modified: Sat, 16 Oct 2021 01:15:19 GMT  
		Size: 60.0 MB (60019955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07117226d68472223964833e6e866764854828a538fdf2ceb27bb6a66fd9fca5`  
		Last Modified: Sat, 16 Oct 2021 01:15:41 GMT  
		Size: 124.5 MB (124517652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:focal-curl`

```console
$ docker pull buildpack-deps@sha256:47084e6d055f10f777634a540c0ec891300768a8fc014ee86e38ad8a961bafa2
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
$ docker pull buildpack-deps@sha256:b1bb273927172a3307daf2e435ad3eaedac707b52aed1a80a6559b5045aa918b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.0 MB (39966612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:699ca4594065556769c48f4df863439f7854e2dc3d247de1ca0ef27c44f306fd`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:43:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:43:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d2365e1e08bb86c1668a76475087cb6db5b42ba70cff99e936b0dda67d9215`  
		Last Modified: Sat, 16 Oct 2021 01:54:19 GMT  
		Size: 7.8 MB (7774998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577c425bc29205ed0c522c9332f7199d4e5805576b76cfa97ff9e345cdb268a5`  
		Last Modified: Sat, 16 Oct 2021 01:54:18 GMT  
		Size: 3.6 MB (3624513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:5ac106cdf6e5b13b0618a85b4eed39d1b3ddee354c7bf1ba5da0f0554c9a9b9b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33938638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4e7f6efd6008f76b37ff18082e23ab310aac81c1e795dec85a64e7fe4f5f7cf`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:12:00 GMT
ADD file:625e3906181f4bd86e59a0e9748f67fcb1391a2e65e36c729e71353381a49757 in / 
# Sat, 16 Oct 2021 01:12:00 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:52:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:52:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8795d4da4abd6abcafe7285749aa85d3a164999e84720a3845f764e56e306771`  
		Last Modified: Sat, 16 Oct 2021 01:15:01 GMT  
		Size: 24.1 MB (24064451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a23aff9df2cf391d11feae54be8e82799a837823112a6dac845d32dc72eca02`  
		Last Modified: Sat, 16 Oct 2021 03:04:40 GMT  
		Size: 6.8 MB (6770106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce73020529e5c4c05a06cf469c45636d454253e819779803de574708312ec61`  
		Last Modified: Sat, 16 Oct 2021 03:04:37 GMT  
		Size: 3.1 MB (3104081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:5ab6253594e45232ef897f4704055eea3babf20a475e9747ce10766d44c4fdc6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38197249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:369dd1ca9197a48ea1f1e4db32de5c2bebef7886c4477c290b342f8f85be72d8`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:06:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:06:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d32ba945c264e68ad0217898b4deb849a7b2b26d5877601d63d4545e29806e8`  
		Last Modified: Sat, 16 Oct 2021 03:20:27 GMT  
		Size: 7.6 MB (7639827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8491af4d3a3f4c7eace39c71ad3060a1909e99874d90b33647db45e9ce4482fa`  
		Last Modified: Sat, 16 Oct 2021 03:20:21 GMT  
		Size: 3.4 MB (3386522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:eef3c0a41f6cfc83f7c300350cc0da51c3d3185a17d758edbcdc8b4e2b6c3ccf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46471758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44c8645449e8182a2157126f6b3219cb1ec8436d8919a30c6ef1e8eff0cf511c`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:36:38 GMT
ADD file:9246bf887411af1b286de95d779c11581dcef3c0d5a29e434162f0c085a7ce85 in / 
# Sat, 16 Oct 2021 00:36:44 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:08:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:09:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:77ba7971d651af68e20e7cbb6603a3f7acd8ef2893066767a93db104723556f2`  
		Last Modified: Sat, 16 Oct 2021 00:38:38 GMT  
		Size: 33.3 MB (33287238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b70bd5d2bc58b580d50736dbb70b528bdcd2910275584c8774c52efd29b8838`  
		Last Modified: Sat, 16 Oct 2021 01:29:38 GMT  
		Size: 8.7 MB (8728083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5e49a7fcde36f5b4cd0c87bace3ad307d0709d6942ff3ec27c5090922c1c7c`  
		Last Modified: Sat, 16 Oct 2021 01:29:16 GMT  
		Size: 4.5 MB (4456437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:8102a47411513107d38819cf1c50c53a59b006b8758ef1760d08cf6ef9189d53
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34121525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81fb5dedcf54f0770eebdd37611586bf30053249c901ae7232aa30b16ab13d82`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:14:21 GMT
ADD file:9e85e474b240689ee9bae50d5101df1d6128c335d61a8010cd69202f778a773f in / 
# Sat, 16 Oct 2021 00:14:22 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 00:55:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 00:56:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:828cfd0a7a30e2a8cf76cca67b8314a0738943c0ea83f167ea5b8bd084c19324`  
		Last Modified: Sat, 16 Oct 2021 00:27:58 GMT  
		Size: 24.2 MB (24226165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0acf80d7193afc4761abdd46a164fd3130cfdb676ff3801645cb819e88404dad`  
		Last Modified: Sat, 16 Oct 2021 01:28:59 GMT  
		Size: 6.8 MB (6750726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab037bb968a07aace1a589724d7eb8ec30de3a596a4227fa9fc39de318067cb`  
		Last Modified: Sat, 16 Oct 2021 01:28:54 GMT  
		Size: 3.1 MB (3144634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:df2267e8f1ad540996bba096ece6a0ac191843ccd329f8acea0b78f977e3433f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.1 MB (38091428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f3fe3fc44fce5558d3d6596b6c1c62d958ff8a740b249bcb858c65f15c905f7`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:41:46 GMT
ADD file:cf3b6f9c395392eaf2c629969f59c48cde60ae1c74c3dbb13886481999a7a4d5 in / 
# Sat, 16 Oct 2021 00:41:48 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:09:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:09:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1f0267805ccac7499fadaabf65e52d4564add2bc20ed25bcf77df24d8debb103`  
		Last Modified: Sat, 16 Oct 2021 00:42:57 GMT  
		Size: 27.1 MB (27120856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe453f45d32c58639c70b42127d12e8467533bc152ff663c5ffc8d0b5407293`  
		Last Modified: Sat, 16 Oct 2021 01:15:04 GMT  
		Size: 7.4 MB (7428503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df987c93c7f716b8ea845b480a00ccf4e4d962df89ed9f8cbefecdb1d9a96cf2`  
		Last Modified: Sat, 16 Oct 2021 01:15:03 GMT  
		Size: 3.5 MB (3542069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:focal-scm`

```console
$ docker pull buildpack-deps@sha256:222ddf4dba302cca6ac700a276e8bb278ce853044531129cb2fccec37d3f622d
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
$ docker pull buildpack-deps@sha256:db28fe2833804601492020af431060420b8ff94b84c08e332edff1754ca43cc7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.7 MB (100688716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfe4a06be9ec9a6f2ed84a88ec5a2efd03025dfebdadaa46558c9a8ae2086f1f`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:43:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:43:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 01:44:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d2365e1e08bb86c1668a76475087cb6db5b42ba70cff99e936b0dda67d9215`  
		Last Modified: Sat, 16 Oct 2021 01:54:19 GMT  
		Size: 7.8 MB (7774998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577c425bc29205ed0c522c9332f7199d4e5805576b76cfa97ff9e345cdb268a5`  
		Last Modified: Sat, 16 Oct 2021 01:54:18 GMT  
		Size: 3.6 MB (3624513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fcda6c22ed5cb34aaea71f2bd9622535b40c91c4f8cc26f304720b510f9a6f`  
		Last Modified: Sat, 16 Oct 2021 01:54:38 GMT  
		Size: 60.7 MB (60722104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:c9f054bee4df38a6541850b189dbf384ed8fbaa5db4819a2ebc183f1f8e40d48
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.4 MB (89392384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8f483864653a58be09108cba02450a5d4f63047b5b1a94b83f052739ad0dbb2`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:12:00 GMT
ADD file:625e3906181f4bd86e59a0e9748f67fcb1391a2e65e36c729e71353381a49757 in / 
# Sat, 16 Oct 2021 01:12:00 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:52:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:52:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 02:53:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8795d4da4abd6abcafe7285749aa85d3a164999e84720a3845f764e56e306771`  
		Last Modified: Sat, 16 Oct 2021 01:15:01 GMT  
		Size: 24.1 MB (24064451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a23aff9df2cf391d11feae54be8e82799a837823112a6dac845d32dc72eca02`  
		Last Modified: Sat, 16 Oct 2021 03:04:40 GMT  
		Size: 6.8 MB (6770106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce73020529e5c4c05a06cf469c45636d454253e819779803de574708312ec61`  
		Last Modified: Sat, 16 Oct 2021 03:04:37 GMT  
		Size: 3.1 MB (3104081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9998d3d2297827b1708a84f36e166391af9aecaafd91bf2d67b2dff8b1ad8a`  
		Last Modified: Sat, 16 Oct 2021 03:05:32 GMT  
		Size: 55.5 MB (55453746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f2c785f3366e906ddfb3628fc19d27edf4085e718b958ee51da3f053cc4fb963
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.0 MB (98972372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28368350ce887feb38c7efd949a238df59747b3b785649046168c4a048339e0e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:06:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:06:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 03:06:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d32ba945c264e68ad0217898b4deb849a7b2b26d5877601d63d4545e29806e8`  
		Last Modified: Sat, 16 Oct 2021 03:20:27 GMT  
		Size: 7.6 MB (7639827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8491af4d3a3f4c7eace39c71ad3060a1909e99874d90b33647db45e9ce4482fa`  
		Last Modified: Sat, 16 Oct 2021 03:20:21 GMT  
		Size: 3.4 MB (3386522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cfb326f9da9ecc7f75c6f18d8aad46bf48677fba9bfb90d7d598271ee287959`  
		Last Modified: Sat, 16 Oct 2021 03:20:47 GMT  
		Size: 60.8 MB (60775123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:326e4176f66a5c4be1ac29828e60f739348b5ba008dc4e2361c427756faa6b02
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115859517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0326065a3f294abcae80a83eedf20dd7b4d76df25a85d8bea0e01f32bc0a25f`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:36:38 GMT
ADD file:9246bf887411af1b286de95d779c11581dcef3c0d5a29e434162f0c085a7ce85 in / 
# Sat, 16 Oct 2021 00:36:44 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:08:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:09:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 01:11:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:77ba7971d651af68e20e7cbb6603a3f7acd8ef2893066767a93db104723556f2`  
		Last Modified: Sat, 16 Oct 2021 00:38:38 GMT  
		Size: 33.3 MB (33287238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b70bd5d2bc58b580d50736dbb70b528bdcd2910275584c8774c52efd29b8838`  
		Last Modified: Sat, 16 Oct 2021 01:29:38 GMT  
		Size: 8.7 MB (8728083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5e49a7fcde36f5b4cd0c87bace3ad307d0709d6942ff3ec27c5090922c1c7c`  
		Last Modified: Sat, 16 Oct 2021 01:29:16 GMT  
		Size: 4.5 MB (4456437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9332a33dc6df6ad95548ba3915b3a1235486dee9aacc7d13206604539866d440`  
		Last Modified: Sat, 16 Oct 2021 01:30:25 GMT  
		Size: 69.4 MB (69387759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:32c03e9661aebe7ea0b551909060f7933d21dd26b8cff2f9bba539d35c920b95
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.1 MB (98111383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7382cfde4760dcd8d917da671f1af5eea2423bdf29123e3d98f7cab60e90a4b4`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:41:46 GMT
ADD file:cf3b6f9c395392eaf2c629969f59c48cde60ae1c74c3dbb13886481999a7a4d5 in / 
# Sat, 16 Oct 2021 00:41:48 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:09:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:09:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 01:10:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1f0267805ccac7499fadaabf65e52d4564add2bc20ed25bcf77df24d8debb103`  
		Last Modified: Sat, 16 Oct 2021 00:42:57 GMT  
		Size: 27.1 MB (27120856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe453f45d32c58639c70b42127d12e8467533bc152ff663c5ffc8d0b5407293`  
		Last Modified: Sat, 16 Oct 2021 01:15:04 GMT  
		Size: 7.4 MB (7428503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df987c93c7f716b8ea845b480a00ccf4e4d962df89ed9f8cbefecdb1d9a96cf2`  
		Last Modified: Sat, 16 Oct 2021 01:15:03 GMT  
		Size: 3.5 MB (3542069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb4bb9db0d64c1d22f8065532581f6cdd28f20b4360950d6c5c3741db428c4f`  
		Last Modified: Sat, 16 Oct 2021 01:15:19 GMT  
		Size: 60.0 MB (60019955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:hirsute`

```console
$ docker pull buildpack-deps@sha256:fd87af8c01206a890d8a97ab52da179dea62346dce07ca6b17b6bf4ffc642fc4
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
$ docker pull buildpack-deps@sha256:c2750d7d73f27c54b134f3afc5eff402d4d023a0f6610a2c14745f0778db55dd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.2 MB (239175401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97986f6e0169d2fcb6b4bb73a55fb278d78a9387cb1c6ef37f4415ed04d15ae4`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:53 GMT
ADD file:36081e580b6851b0f8a1176a307b99a673510dc87809a726cad514bd7f56d620 in / 
# Sat, 16 Oct 2021 01:47:53 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:08:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:08:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 03:08:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:09:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e61beefb4313333ca27a602845cbf2a6f7cba9c176bb999f14a4bdcfb6a54148`  
		Last Modified: Fri, 01 Oct 2021 02:46:09 GMT  
		Size: 30.2 MB (30174163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b2d75872cf44ae1d0e91f4b4298e3d382c845eefa7655b7f2325a88f17c9ad`  
		Last Modified: Sat, 16 Oct 2021 03:21:30 GMT  
		Size: 5.4 MB (5404762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8704bb2e0710d7b555bb044b098f06225f5697ad2878a8f1ae2ac285a3ed825e`  
		Last Modified: Sat, 16 Oct 2021 03:21:29 GMT  
		Size: 3.4 MB (3431928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f566ac9ad20f04707fbf26b5de866cd237d21a3c927fb1f30fe6b94f57040fba`  
		Last Modified: Sat, 16 Oct 2021 03:21:48 GMT  
		Size: 43.5 MB (43533098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5573408c4e367ec83c2be39c8e053c34e050ace99c62306c55a15ac0d0cc10c9`  
		Last Modified: Sat, 16 Oct 2021 03:22:21 GMT  
		Size: 156.6 MB (156631450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:2907a4ade782540beeadc530701ec593f2c1899d1f9ffc71d51962b7a8bf45be
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.1 MB (268143719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:689afc563871e8f713e32f83998d679743c14ac849d1e7a4e979dd31bb349631`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Oct 2021 11:08:18 GMT
ADD file:4fece2b915970b36002bf98a6f85f91c3b9bfeb80b685f7e5ee749080aea6540 in / 
# Tue, 05 Oct 2021 11:08:25 GMT
CMD ["bash"]
# Tue, 05 Oct 2021 15:11:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Oct 2021 15:12:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 05 Oct 2021 15:14:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 05 Oct 2021 15:22:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b16b9756d17acd6ced37d43568054b32fcebdd38ee4b9bdbf35dbc3e872d754d`  
		Last Modified: Tue, 05 Oct 2021 11:11:17 GMT  
		Size: 37.3 MB (37255452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a54cbd41484567ce0ebb693b3129bf830d0e454fbe8a0eec180d9fa9f976c0`  
		Last Modified: Tue, 05 Oct 2021 15:51:52 GMT  
		Size: 6.2 MB (6153990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afff0eec9aba68bd0b14d67496cf23585cea9e37314ecee6657b63816efcd9db`  
		Last Modified: Tue, 05 Oct 2021 15:51:49 GMT  
		Size: 4.5 MB (4523714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1536544f6a113307ef8771dc9e57d3b4974edc1869ee7d08a83f9422c79b1be`  
		Last Modified: Tue, 05 Oct 2021 15:52:37 GMT  
		Size: 49.5 MB (49467145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67a0bc2994fab6d2773059eb5766490eff6f06d4c5cead29d091d284b24873a`  
		Last Modified: Tue, 05 Oct 2021 15:54:11 GMT  
		Size: 170.7 MB (170743418 bytes)  
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
$ docker pull buildpack-deps@sha256:d8a6f33c53c107583b08147895c892edb834472807431b73571086744ca130db
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
$ docker pull buildpack-deps@sha256:39cb123dafa0028e4cb1095811c94c4a5de7a1769165a1e07d3a129988c951cf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (39010853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:239585f43a663f2752dc848bcfe0c2281cc48b9574e96d0d559cd42d54082ec2`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:53 GMT
ADD file:36081e580b6851b0f8a1176a307b99a673510dc87809a726cad514bd7f56d620 in / 
# Sat, 16 Oct 2021 01:47:53 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:08:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:08:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e61beefb4313333ca27a602845cbf2a6f7cba9c176bb999f14a4bdcfb6a54148`  
		Last Modified: Fri, 01 Oct 2021 02:46:09 GMT  
		Size: 30.2 MB (30174163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b2d75872cf44ae1d0e91f4b4298e3d382c845eefa7655b7f2325a88f17c9ad`  
		Last Modified: Sat, 16 Oct 2021 03:21:30 GMT  
		Size: 5.4 MB (5404762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8704bb2e0710d7b555bb044b098f06225f5697ad2878a8f1ae2ac285a3ed825e`  
		Last Modified: Sat, 16 Oct 2021 03:21:29 GMT  
		Size: 3.4 MB (3431928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:dd7f2c04edf3b324b852e429bfe162038e616ee28cac5ee5ce6fc9a36381c60f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47933156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:822a0098d55d4ee7d2286bdcb40edb8f012ba6f0fd689db8d6f09bda568dcc23`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Oct 2021 11:08:18 GMT
ADD file:4fece2b915970b36002bf98a6f85f91c3b9bfeb80b685f7e5ee749080aea6540 in / 
# Tue, 05 Oct 2021 11:08:25 GMT
CMD ["bash"]
# Tue, 05 Oct 2021 15:11:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Oct 2021 15:12:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b16b9756d17acd6ced37d43568054b32fcebdd38ee4b9bdbf35dbc3e872d754d`  
		Last Modified: Tue, 05 Oct 2021 11:11:17 GMT  
		Size: 37.3 MB (37255452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a54cbd41484567ce0ebb693b3129bf830d0e454fbe8a0eec180d9fa9f976c0`  
		Last Modified: Tue, 05 Oct 2021 15:51:52 GMT  
		Size: 6.2 MB (6153990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afff0eec9aba68bd0b14d67496cf23585cea9e37314ecee6657b63816efcd9db`  
		Last Modified: Tue, 05 Oct 2021 15:51:49 GMT  
		Size: 4.5 MB (4523714 bytes)  
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
$ docker pull buildpack-deps@sha256:c5defad7da7db30278b0750495097c0f2604d95701ffe4929ec0f7bcb8472a54
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
$ docker pull buildpack-deps@sha256:cb73476030b9b04ac7bb532dbfcd1ccad95222afd48d09abb5c4bfd8fe5e08c2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.5 MB (82543951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ac4d3b843ffa7164875abf17bfc13bd90748f10af8f0e6463fa5b18e52c79aa`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:53 GMT
ADD file:36081e580b6851b0f8a1176a307b99a673510dc87809a726cad514bd7f56d620 in / 
# Sat, 16 Oct 2021 01:47:53 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:08:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:08:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 03:08:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e61beefb4313333ca27a602845cbf2a6f7cba9c176bb999f14a4bdcfb6a54148`  
		Last Modified: Fri, 01 Oct 2021 02:46:09 GMT  
		Size: 30.2 MB (30174163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b2d75872cf44ae1d0e91f4b4298e3d382c845eefa7655b7f2325a88f17c9ad`  
		Last Modified: Sat, 16 Oct 2021 03:21:30 GMT  
		Size: 5.4 MB (5404762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8704bb2e0710d7b555bb044b098f06225f5697ad2878a8f1ae2ac285a3ed825e`  
		Last Modified: Sat, 16 Oct 2021 03:21:29 GMT  
		Size: 3.4 MB (3431928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f566ac9ad20f04707fbf26b5de866cd237d21a3c927fb1f30fe6b94f57040fba`  
		Last Modified: Sat, 16 Oct 2021 03:21:48 GMT  
		Size: 43.5 MB (43533098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:5b05bc413334c5377efe162a3f3ae34d56e16ea1da1e9806a8f9ddb8761778b3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.4 MB (97400301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bedde56204ff854faef6c52b62b435c3721bf587ac4719e9cbcc069e0ae5509a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Oct 2021 11:08:18 GMT
ADD file:4fece2b915970b36002bf98a6f85f91c3b9bfeb80b685f7e5ee749080aea6540 in / 
# Tue, 05 Oct 2021 11:08:25 GMT
CMD ["bash"]
# Tue, 05 Oct 2021 15:11:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Oct 2021 15:12:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 05 Oct 2021 15:14:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b16b9756d17acd6ced37d43568054b32fcebdd38ee4b9bdbf35dbc3e872d754d`  
		Last Modified: Tue, 05 Oct 2021 11:11:17 GMT  
		Size: 37.3 MB (37255452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a54cbd41484567ce0ebb693b3129bf830d0e454fbe8a0eec180d9fa9f976c0`  
		Last Modified: Tue, 05 Oct 2021 15:51:52 GMT  
		Size: 6.2 MB (6153990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afff0eec9aba68bd0b14d67496cf23585cea9e37314ecee6657b63816efcd9db`  
		Last Modified: Tue, 05 Oct 2021 15:51:49 GMT  
		Size: 4.5 MB (4523714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1536544f6a113307ef8771dc9e57d3b4974edc1869ee7d08a83f9422c79b1be`  
		Last Modified: Tue, 05 Oct 2021 15:52:37 GMT  
		Size: 49.5 MB (49467145 bytes)  
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
$ docker pull buildpack-deps@sha256:77d030141c1f974e8db2be4253d5f44be3222edfb94ca070c9a9bb4a603aeab2
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
$ docker pull buildpack-deps@sha256:84a1afe105bf52f9c41e8cd4b90eb1195d77281c54124d3bf89340527b1b2b2a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **406.7 MB (406684539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b9ef5692961b31df2550467196c52c2fea87a56286e0309e94001e75d07341c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Nov 2021 22:20:34 GMT
ADD file:c061cabbaa10b98eed8dcea770d97000a2861c407f5208a0327bef2b38a99fee in / 
# Thu, 04 Nov 2021 22:20:35 GMT
CMD ["bash"]
# Thu, 04 Nov 2021 22:56:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Nov 2021 22:57:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 04 Nov 2021 22:57:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 04 Nov 2021 23:01:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ae6e1b672be676522e8af69609544dd00b8517e394592a58194383b26e9b54c5`  
		Last Modified: Thu, 04 Nov 2021 22:21:31 GMT  
		Size: 30.4 MB (30378721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4488401b75c6ec432177829c795e1ec36857d568171ae1f197c2c24a9b7e7d8d`  
		Last Modified: Thu, 04 Nov 2021 23:03:09 GMT  
		Size: 3.7 MB (3693784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb8a4e0bca131c5b9e451c10a345a0a13be03cf5ac1220cdc85f170d17be763`  
		Last Modified: Thu, 04 Nov 2021 23:03:09 GMT  
		Size: 3.6 MB (3551867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:538adb79b719e15749a81b037e806769f285f50a60ca3418546e00ffb465a44f`  
		Last Modified: Thu, 04 Nov 2021 23:03:25 GMT  
		Size: 38.1 MB (38080223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d21bd11602fc3dd3a497fb9e548f63e527ab6ddf6d1a69ff6fc0e2a99f0591cc`  
		Last Modified: Thu, 04 Nov 2021 23:04:17 GMT  
		Size: 331.0 MB (330979944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:5e98f132603710520315c5f3c095c64779984ffe325463ef0f000d6c0f05b8f3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **371.1 MB (371071262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b7162038a1509bbaf31446b9e31729058b627dd8218ae0ff632d356e7488d25`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Nov 2021 22:31:15 GMT
ADD file:675ad5623adf2dafceb59e4a67c75ca26f664127c76fe61c1903cc85d16b9abb in / 
# Thu, 04 Nov 2021 22:31:16 GMT
CMD ["bash"]
# Thu, 04 Nov 2021 23:28:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Nov 2021 23:28:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 04 Nov 2021 23:29:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 04 Nov 2021 23:31:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f7dc858b30797c13a0706f9660d1290ae625ab3436fd5db984b0dac888ad9c8f`  
		Last Modified: Thu, 04 Nov 2021 22:34:32 GMT  
		Size: 26.9 MB (26917157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64923825f2b20992e031b3992dc8c85722c1421e18d7f0fd69532d01d31c2617`  
		Last Modified: Thu, 04 Nov 2021 23:37:31 GMT  
		Size: 3.4 MB (3443243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d36d145711f3ed07bdbf6134addb14e00b663cb32b4de67ff1674023832998`  
		Last Modified: Thu, 04 Nov 2021 23:37:30 GMT  
		Size: 3.7 MB (3742795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:016df4abc6b88c7564811d0545d3f7eeb911db620be98dce64597a05cd3747b7`  
		Last Modified: Thu, 04 Nov 2021 23:38:12 GMT  
		Size: 40.3 MB (40283870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529c6ecc92223423b997a4417f4c58eb16c9fab9a7e390ec178d925ea6721a52`  
		Last Modified: Thu, 04 Nov 2021 23:41:13 GMT  
		Size: 296.7 MB (296684197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c1478864379e7b484a8b644142cf4bdc8ba8ed80d282f48d9afda3341c9e8e61
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **399.3 MB (399325584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fdeb12cec56afc17f5f9e972ca22732876e8017aa4748442741c17e97bdfff2`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Nov 2021 21:55:45 GMT
ADD file:1b42b91df70bf5eb9529802354c8c97bb9ba991a7885a3fdd4ad5be4b662b70c in / 
# Thu, 04 Nov 2021 21:55:46 GMT
CMD ["bash"]
# Thu, 04 Nov 2021 22:28:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Nov 2021 22:29:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 04 Nov 2021 22:29:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 04 Nov 2021 22:30:32 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:07806c11d5adbc5d83daf2661f72147213f9056f681e452180dc14d81e368e17`  
		Last Modified: Thu, 04 Nov 2021 21:57:10 GMT  
		Size: 29.0 MB (29026100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a952a5c90bcb8e3a8ab1bd7854d8265e7fcb3cb0c0f417fb5722e8f3e0972208`  
		Last Modified: Thu, 04 Nov 2021 22:33:00 GMT  
		Size: 3.7 MB (3678628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cca9702f2a91f991f023bbb9b582e71befe4781bbaa74653b2458540b02c0e3`  
		Last Modified: Thu, 04 Nov 2021 22:32:59 GMT  
		Size: 3.3 MB (3327135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e1d1ea4e9af80ec48e6e5d034e77b64b8de00080ef82b379213f41b1da18b1`  
		Last Modified: Thu, 04 Nov 2021 22:33:17 GMT  
		Size: 38.0 MB (38032438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4b5048b8e4f553fd6380ef6399e0445920029686713f8c2cd8352c0b9164f5`  
		Last Modified: Thu, 04 Nov 2021 22:34:11 GMT  
		Size: 325.3 MB (325261283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:76524c8f33ad061c15feccd1916806689b3a3e14fc3715b09551725cba103641
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **414.3 MB (414270146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ec6e7f58a8e01be4d11e700d402ed21f4ce524da513527acb10feedfde15d94`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Nov 2021 23:51:29 GMT
ADD file:dc4e5dbd5333b274b2af1c57862eeb96c4b2eda9e8d1a5b766b4ff2aa242106f in / 
# Thu, 04 Nov 2021 23:51:35 GMT
CMD ["bash"]
# Fri, 05 Nov 2021 01:51:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 05 Nov 2021 01:51:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 05 Nov 2021 01:53:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 05 Nov 2021 01:58:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6fb8a15f7529caac80795ba7b74d3c07d163030311fab31ef7b9eda5d4612190`  
		Last Modified: Thu, 04 Nov 2021 23:53:39 GMT  
		Size: 36.2 MB (36174155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a811f8d539d495275857666e419e2349b4afd49b9e35684be52fa958a9edfc64`  
		Last Modified: Fri, 05 Nov 2021 02:01:11 GMT  
		Size: 4.1 MB (4146837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567f57d31cc6184d7de4f38b999b49a84d09a99cd73ecff5fc148f918d7a9f85`  
		Last Modified: Fri, 05 Nov 2021 02:01:11 GMT  
		Size: 4.2 MB (4242137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cfc0512fc4cbeb0f1888bd931fc2dbf9f49bc00278d9c2c5b7aa5272e519c1d`  
		Last Modified: Fri, 05 Nov 2021 02:01:31 GMT  
		Size: 42.7 MB (42707492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19cb8a7b5b5cfa913819716cdb765f5c157cba26b78fb1a9340991522e5bcbf8`  
		Last Modified: Fri, 05 Nov 2021 02:02:41 GMT  
		Size: 327.0 MB (326999525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:c6b355aa926760c8c218c7917ffa5fafedd30aa73f458aeec83f31cb551ba17c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.3 MB (266339613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee9a89d94c7b91730d83f4ec86752690d6a9704d313cfd4219e4c1c64d783e7d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 11 Nov 2021 01:34:25 GMT
ADD file:def88534019c26953298b38d1af30a296db3d6995d6c801bc98407de70a9e1a6 in / 
# Thu, 11 Nov 2021 01:34:26 GMT
CMD ["bash"]
# Thu, 11 Nov 2021 06:26:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 11 Nov 2021 06:27:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 11 Nov 2021 06:30:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 11 Nov 2021 06:36:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c236a68e6fcd6aac214c2851f12d0e004328b6cc65c84adea73ec2c8eccd27b8`  
		Last Modified: Thu, 11 Nov 2021 01:50:51 GMT  
		Size: 27.2 MB (27206693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32c0816a844c3da682a583d08b1d066cbf7fdaff37ecc1ffe756a1762b5116e`  
		Last Modified: Thu, 11 Nov 2021 06:54:43 GMT  
		Size: 3.5 MB (3490272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd32937a18c0c808ff182ae5991f2dcc6394079d138e4d6880d9013b9e5998a`  
		Last Modified: Thu, 11 Nov 2021 06:54:41 GMT  
		Size: 3.8 MB (3803776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20817c240d9af80288c0d7e22536e4e16be4622339e8522790aa1ddd56e8fd08`  
		Last Modified: Thu, 11 Nov 2021 06:56:39 GMT  
		Size: 40.8 MB (40763475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5caf44e6024c1f0dfa79f670bd50de448af089f51a535f18b001656877b49265`  
		Last Modified: Thu, 11 Nov 2021 07:02:24 GMT  
		Size: 191.1 MB (191075397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:8d5f495082abea977233155a08b50e5b98405fc110ad692f85e5f61b5c6175cf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **367.8 MB (367814921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb381a4dbf6e71916baefde96a33c513bf55b06d46571575a68a7158bf3c2b55`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Nov 2021 22:00:03 GMT
ADD file:ab83cb3e32154ba2db5167029d8e8d5388c50b5c29d8c79c713c0e0d2d692d27 in / 
# Thu, 04 Nov 2021 22:00:05 GMT
CMD ["bash"]
# Thu, 04 Nov 2021 22:18:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Nov 2021 22:19:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 04 Nov 2021 22:19:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 04 Nov 2021 22:20:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e737ddf26245fcdcc7eced9ccccb22176e9f1ba12d8f0d15cb1342c337544bdf`  
		Last Modified: Thu, 04 Nov 2021 22:01:24 GMT  
		Size: 30.5 MB (30525829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0355a8a2f0153f71261e3597b628202632603a052d63c9cecc0e1da9659b7c`  
		Last Modified: Thu, 04 Nov 2021 22:23:03 GMT  
		Size: 3.8 MB (3767643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f088a56f227fe3f111d256ae3c603419e2b9c7ee314548ef27c2479050a69e`  
		Last Modified: Thu, 04 Nov 2021 22:23:03 GMT  
		Size: 4.0 MB (3963241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d231728eaed51bc6e262952b25d2d76d8028ea980ea6f8651bf06147ac7981c`  
		Last Modified: Thu, 04 Nov 2021 22:23:15 GMT  
		Size: 38.3 MB (38324849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72d36bef3f492cf4db2c18617f56583fb674197398969239006ddf93f50495cc`  
		Last Modified: Thu, 04 Nov 2021 22:23:55 GMT  
		Size: 291.2 MB (291233359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:impish-curl`

```console
$ docker pull buildpack-deps@sha256:b3afb9be9f6ff953e54c44375be156551f06d6b9ac5c003af34a32824ba7cd34
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
$ docker pull buildpack-deps@sha256:54c923092a83d0fd403372895cc7a052c5d93975a64600e8b2dc87c3ce47494a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37624372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5784379919f76e6e2636d7558d1932259ce9a619c55a89fd18de979439e5a863`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Nov 2021 22:20:34 GMT
ADD file:c061cabbaa10b98eed8dcea770d97000a2861c407f5208a0327bef2b38a99fee in / 
# Thu, 04 Nov 2021 22:20:35 GMT
CMD ["bash"]
# Thu, 04 Nov 2021 22:56:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Nov 2021 22:57:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ae6e1b672be676522e8af69609544dd00b8517e394592a58194383b26e9b54c5`  
		Last Modified: Thu, 04 Nov 2021 22:21:31 GMT  
		Size: 30.4 MB (30378721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4488401b75c6ec432177829c795e1ec36857d568171ae1f197c2c24a9b7e7d8d`  
		Last Modified: Thu, 04 Nov 2021 23:03:09 GMT  
		Size: 3.7 MB (3693784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb8a4e0bca131c5b9e451c10a345a0a13be03cf5ac1220cdc85f170d17be763`  
		Last Modified: Thu, 04 Nov 2021 23:03:09 GMT  
		Size: 3.6 MB (3551867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:cdf2e5e90315eff8c9fa17950a02925e550d668cabf6a092fd629fd2489cb835
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34103195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4c36290c105f7d65eff92415d0b8b56be4f54a2051c3e35b8e330c7dadda26e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Nov 2021 22:31:15 GMT
ADD file:675ad5623adf2dafceb59e4a67c75ca26f664127c76fe61c1903cc85d16b9abb in / 
# Thu, 04 Nov 2021 22:31:16 GMT
CMD ["bash"]
# Thu, 04 Nov 2021 23:28:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Nov 2021 23:28:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f7dc858b30797c13a0706f9660d1290ae625ab3436fd5db984b0dac888ad9c8f`  
		Last Modified: Thu, 04 Nov 2021 22:34:32 GMT  
		Size: 26.9 MB (26917157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64923825f2b20992e031b3992dc8c85722c1421e18d7f0fd69532d01d31c2617`  
		Last Modified: Thu, 04 Nov 2021 23:37:31 GMT  
		Size: 3.4 MB (3443243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d36d145711f3ed07bdbf6134addb14e00b663cb32b4de67ff1674023832998`  
		Last Modified: Thu, 04 Nov 2021 23:37:30 GMT  
		Size: 3.7 MB (3742795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:00c6025c7a15dfe57955537030d672bcdcaf4a2389fc446007e602d155927bf6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.0 MB (36031863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b11808ca59b32ca29aceb263695f64a95c22f3784efef11a16304f51f440ff1a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Nov 2021 21:55:45 GMT
ADD file:1b42b91df70bf5eb9529802354c8c97bb9ba991a7885a3fdd4ad5be4b662b70c in / 
# Thu, 04 Nov 2021 21:55:46 GMT
CMD ["bash"]
# Thu, 04 Nov 2021 22:28:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Nov 2021 22:29:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:07806c11d5adbc5d83daf2661f72147213f9056f681e452180dc14d81e368e17`  
		Last Modified: Thu, 04 Nov 2021 21:57:10 GMT  
		Size: 29.0 MB (29026100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a952a5c90bcb8e3a8ab1bd7854d8265e7fcb3cb0c0f417fb5722e8f3e0972208`  
		Last Modified: Thu, 04 Nov 2021 22:33:00 GMT  
		Size: 3.7 MB (3678628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cca9702f2a91f991f023bbb9b582e71befe4781bbaa74653b2458540b02c0e3`  
		Last Modified: Thu, 04 Nov 2021 22:32:59 GMT  
		Size: 3.3 MB (3327135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:0cc84931e7355f0a2ec18838056c982f9599d01d99f0a81c365098ed2373f8cd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.6 MB (44563129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:940ae21526802e5c51c15c215053b8095e827480a47aaea8d00e399c958e4dba`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Nov 2021 23:51:29 GMT
ADD file:dc4e5dbd5333b274b2af1c57862eeb96c4b2eda9e8d1a5b766b4ff2aa242106f in / 
# Thu, 04 Nov 2021 23:51:35 GMT
CMD ["bash"]
# Fri, 05 Nov 2021 01:51:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 05 Nov 2021 01:51:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6fb8a15f7529caac80795ba7b74d3c07d163030311fab31ef7b9eda5d4612190`  
		Last Modified: Thu, 04 Nov 2021 23:53:39 GMT  
		Size: 36.2 MB (36174155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a811f8d539d495275857666e419e2349b4afd49b9e35684be52fa958a9edfc64`  
		Last Modified: Fri, 05 Nov 2021 02:01:11 GMT  
		Size: 4.1 MB (4146837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567f57d31cc6184d7de4f38b999b49a84d09a99cd73ecff5fc148f918d7a9f85`  
		Last Modified: Fri, 05 Nov 2021 02:01:11 GMT  
		Size: 4.2 MB (4242137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:a60d9614189e9a414cd72cc5bcf35ff30825c9ba8c2ef9c68a3df23684370df2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34500741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:386b795e60ea56fff90f8871ec0d6d4c2fa29a17fe88c124d55251bb078e45b9`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 11 Nov 2021 01:34:25 GMT
ADD file:def88534019c26953298b38d1af30a296db3d6995d6c801bc98407de70a9e1a6 in / 
# Thu, 11 Nov 2021 01:34:26 GMT
CMD ["bash"]
# Thu, 11 Nov 2021 06:26:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 11 Nov 2021 06:27:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c236a68e6fcd6aac214c2851f12d0e004328b6cc65c84adea73ec2c8eccd27b8`  
		Last Modified: Thu, 11 Nov 2021 01:50:51 GMT  
		Size: 27.2 MB (27206693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32c0816a844c3da682a583d08b1d066cbf7fdaff37ecc1ffe756a1762b5116e`  
		Last Modified: Thu, 11 Nov 2021 06:54:43 GMT  
		Size: 3.5 MB (3490272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd32937a18c0c808ff182ae5991f2dcc6394079d138e4d6880d9013b9e5998a`  
		Last Modified: Thu, 11 Nov 2021 06:54:41 GMT  
		Size: 3.8 MB (3803776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:69d0be5d4a84d1fd9eccc366c301e3bb5eb1e5ee063ae63dfb73e0ab2b878b53
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38256713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4e776fddfc4e1399852bc124156b58b876d4f021cd53374abd1813b05be224c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Nov 2021 22:00:03 GMT
ADD file:ab83cb3e32154ba2db5167029d8e8d5388c50b5c29d8c79c713c0e0d2d692d27 in / 
# Thu, 04 Nov 2021 22:00:05 GMT
CMD ["bash"]
# Thu, 04 Nov 2021 22:18:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Nov 2021 22:19:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e737ddf26245fcdcc7eced9ccccb22176e9f1ba12d8f0d15cb1342c337544bdf`  
		Last Modified: Thu, 04 Nov 2021 22:01:24 GMT  
		Size: 30.5 MB (30525829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0355a8a2f0153f71261e3597b628202632603a052d63c9cecc0e1da9659b7c`  
		Last Modified: Thu, 04 Nov 2021 22:23:03 GMT  
		Size: 3.8 MB (3767643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f088a56f227fe3f111d256ae3c603419e2b9c7ee314548ef27c2479050a69e`  
		Last Modified: Thu, 04 Nov 2021 22:23:03 GMT  
		Size: 4.0 MB (3963241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:impish-scm`

```console
$ docker pull buildpack-deps@sha256:bb68b5bf6258696aa2e152bfd8889269fc9f3f9c5b97287924f13739ea6ace1d
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
$ docker pull buildpack-deps@sha256:be7ea01ded251a2ca6d94d0c9f8153ef11a99c4f19603a96f01b918142d89bd5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75704595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb44de8b24049cedb568779358422987bb6b92d0a022d21f0e9440bde2381355`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Nov 2021 22:20:34 GMT
ADD file:c061cabbaa10b98eed8dcea770d97000a2861c407f5208a0327bef2b38a99fee in / 
# Thu, 04 Nov 2021 22:20:35 GMT
CMD ["bash"]
# Thu, 04 Nov 2021 22:56:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Nov 2021 22:57:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 04 Nov 2021 22:57:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ae6e1b672be676522e8af69609544dd00b8517e394592a58194383b26e9b54c5`  
		Last Modified: Thu, 04 Nov 2021 22:21:31 GMT  
		Size: 30.4 MB (30378721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4488401b75c6ec432177829c795e1ec36857d568171ae1f197c2c24a9b7e7d8d`  
		Last Modified: Thu, 04 Nov 2021 23:03:09 GMT  
		Size: 3.7 MB (3693784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb8a4e0bca131c5b9e451c10a345a0a13be03cf5ac1220cdc85f170d17be763`  
		Last Modified: Thu, 04 Nov 2021 23:03:09 GMT  
		Size: 3.6 MB (3551867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:538adb79b719e15749a81b037e806769f285f50a60ca3418546e00ffb465a44f`  
		Last Modified: Thu, 04 Nov 2021 23:03:25 GMT  
		Size: 38.1 MB (38080223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:c5609d52dc9fb38b4aacee4d68f362376ba20f2b951f9839df10238602a1df9f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.4 MB (74387065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:083634dd134e2787b5bdc31a4b94d37646c1fca8035481fd0462bf0215a072c3`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Nov 2021 22:31:15 GMT
ADD file:675ad5623adf2dafceb59e4a67c75ca26f664127c76fe61c1903cc85d16b9abb in / 
# Thu, 04 Nov 2021 22:31:16 GMT
CMD ["bash"]
# Thu, 04 Nov 2021 23:28:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Nov 2021 23:28:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 04 Nov 2021 23:29:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f7dc858b30797c13a0706f9660d1290ae625ab3436fd5db984b0dac888ad9c8f`  
		Last Modified: Thu, 04 Nov 2021 22:34:32 GMT  
		Size: 26.9 MB (26917157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64923825f2b20992e031b3992dc8c85722c1421e18d7f0fd69532d01d31c2617`  
		Last Modified: Thu, 04 Nov 2021 23:37:31 GMT  
		Size: 3.4 MB (3443243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d36d145711f3ed07bdbf6134addb14e00b663cb32b4de67ff1674023832998`  
		Last Modified: Thu, 04 Nov 2021 23:37:30 GMT  
		Size: 3.7 MB (3742795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:016df4abc6b88c7564811d0545d3f7eeb911db620be98dce64597a05cd3747b7`  
		Last Modified: Thu, 04 Nov 2021 23:38:12 GMT  
		Size: 40.3 MB (40283870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:6ca52d36f45191c2bff56479c7addc641c520e3b721d237287a1a6e6a2295e7e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.1 MB (74064301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e02fffcd9134167d6655e1c30a85beecb06ef2c9233cdef78e37897b5d398341`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Nov 2021 21:55:45 GMT
ADD file:1b42b91df70bf5eb9529802354c8c97bb9ba991a7885a3fdd4ad5be4b662b70c in / 
# Thu, 04 Nov 2021 21:55:46 GMT
CMD ["bash"]
# Thu, 04 Nov 2021 22:28:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Nov 2021 22:29:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 04 Nov 2021 22:29:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:07806c11d5adbc5d83daf2661f72147213f9056f681e452180dc14d81e368e17`  
		Last Modified: Thu, 04 Nov 2021 21:57:10 GMT  
		Size: 29.0 MB (29026100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a952a5c90bcb8e3a8ab1bd7854d8265e7fcb3cb0c0f417fb5722e8f3e0972208`  
		Last Modified: Thu, 04 Nov 2021 22:33:00 GMT  
		Size: 3.7 MB (3678628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cca9702f2a91f991f023bbb9b582e71befe4781bbaa74653b2458540b02c0e3`  
		Last Modified: Thu, 04 Nov 2021 22:32:59 GMT  
		Size: 3.3 MB (3327135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e1d1ea4e9af80ec48e6e5d034e77b64b8de00080ef82b379213f41b1da18b1`  
		Last Modified: Thu, 04 Nov 2021 22:33:17 GMT  
		Size: 38.0 MB (38032438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:eed517a6832af7446961327af826bf0c50b3fc7d9259158a2bc4dd3dc53759c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.3 MB (87270621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94972edd2bba9d41b3a39c0aef62bc5e7650c595afdbbd8b3ca9ce835ef6c6e4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Nov 2021 23:51:29 GMT
ADD file:dc4e5dbd5333b274b2af1c57862eeb96c4b2eda9e8d1a5b766b4ff2aa242106f in / 
# Thu, 04 Nov 2021 23:51:35 GMT
CMD ["bash"]
# Fri, 05 Nov 2021 01:51:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 05 Nov 2021 01:51:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 05 Nov 2021 01:53:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6fb8a15f7529caac80795ba7b74d3c07d163030311fab31ef7b9eda5d4612190`  
		Last Modified: Thu, 04 Nov 2021 23:53:39 GMT  
		Size: 36.2 MB (36174155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a811f8d539d495275857666e419e2349b4afd49b9e35684be52fa958a9edfc64`  
		Last Modified: Fri, 05 Nov 2021 02:01:11 GMT  
		Size: 4.1 MB (4146837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567f57d31cc6184d7de4f38b999b49a84d09a99cd73ecff5fc148f918d7a9f85`  
		Last Modified: Fri, 05 Nov 2021 02:01:11 GMT  
		Size: 4.2 MB (4242137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cfc0512fc4cbeb0f1888bd931fc2dbf9f49bc00278d9c2c5b7aa5272e519c1d`  
		Last Modified: Fri, 05 Nov 2021 02:01:31 GMT  
		Size: 42.7 MB (42707492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:1646f127c48e431100e6930d603da4cef39744d303aff6bfe9a3f5d35ba69e1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.3 MB (75264216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d52e65f7ce2ae95fda50dd675073c828cf1f9e113d34ed156decaeb6b34711fc`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 11 Nov 2021 01:34:25 GMT
ADD file:def88534019c26953298b38d1af30a296db3d6995d6c801bc98407de70a9e1a6 in / 
# Thu, 11 Nov 2021 01:34:26 GMT
CMD ["bash"]
# Thu, 11 Nov 2021 06:26:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 11 Nov 2021 06:27:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 11 Nov 2021 06:30:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c236a68e6fcd6aac214c2851f12d0e004328b6cc65c84adea73ec2c8eccd27b8`  
		Last Modified: Thu, 11 Nov 2021 01:50:51 GMT  
		Size: 27.2 MB (27206693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32c0816a844c3da682a583d08b1d066cbf7fdaff37ecc1ffe756a1762b5116e`  
		Last Modified: Thu, 11 Nov 2021 06:54:43 GMT  
		Size: 3.5 MB (3490272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd32937a18c0c808ff182ae5991f2dcc6394079d138e4d6880d9013b9e5998a`  
		Last Modified: Thu, 11 Nov 2021 06:54:41 GMT  
		Size: 3.8 MB (3803776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20817c240d9af80288c0d7e22536e4e16be4622339e8522790aa1ddd56e8fd08`  
		Last Modified: Thu, 11 Nov 2021 06:56:39 GMT  
		Size: 40.8 MB (40763475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b961b4b9338629accb7eb8c51ddf4512dee4ea4f483996fde0ae3b33285dc076
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.6 MB (76581562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84b6e0cec4c3e1a5925b93493e48cd160b3afbf055e9831774038268ea7ef6bf`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Nov 2021 22:00:03 GMT
ADD file:ab83cb3e32154ba2db5167029d8e8d5388c50b5c29d8c79c713c0e0d2d692d27 in / 
# Thu, 04 Nov 2021 22:00:05 GMT
CMD ["bash"]
# Thu, 04 Nov 2021 22:18:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Nov 2021 22:19:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 04 Nov 2021 22:19:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e737ddf26245fcdcc7eced9ccccb22176e9f1ba12d8f0d15cb1342c337544bdf`  
		Last Modified: Thu, 04 Nov 2021 22:01:24 GMT  
		Size: 30.5 MB (30525829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0355a8a2f0153f71261e3597b628202632603a052d63c9cecc0e1da9659b7c`  
		Last Modified: Thu, 04 Nov 2021 22:23:03 GMT  
		Size: 3.8 MB (3767643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f088a56f227fe3f111d256ae3c603419e2b9c7ee314548ef27c2479050a69e`  
		Last Modified: Thu, 04 Nov 2021 22:23:03 GMT  
		Size: 4.0 MB (3963241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d231728eaed51bc6e262952b25d2d76d8028ea980ea6f8651bf06147ac7981c`  
		Last Modified: Thu, 04 Nov 2021 22:23:15 GMT  
		Size: 38.3 MB (38324849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:latest`

```console
$ docker pull buildpack-deps@sha256:39d6d1b626103d5d8daecf321abe9d8a1ce5cc8cbff2cd3195b4fdb04af654f3
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
$ docker pull buildpack-deps@sha256:067329836a99c56bd087b255c70cf2e7bb7f0c1965d8a12be769c86a062c12a4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.0 MB (322022992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48a4688637227faef31aa5134c34ca2ec85dd07beebcf327c38566eb3eb8ef79`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:15:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66b7f31b095b7fa01d8ba10e600a192bab43a1311f50216cf6fa9a45d0f435e`  
		Last Modified: Wed, 17 Nov 2021 03:24:18 GMT  
		Size: 196.5 MB (196498701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:095b3e58e31205572ba70b19cefdc7ec5de99683e74c0c8f095e3d564b2e1f0b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.1 MB (295100343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc59e839989efbe22d3c9e21e3cefb3c810799f569486d4f5493b98c454a3bb1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 00:49:54 GMT
ADD file:b9969604315238de271e1769a4b8dd85cdf0d33f9fac387e940d5195ac3030a1 in / 
# Tue, 12 Oct 2021 00:49:55 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:40:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:41:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 05:42:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:44:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a97c782f2538791984ce12c859cada96e395e3950d4cb7d1238e08acd2eb74ec`  
		Last Modified: Tue, 12 Oct 2021 01:05:12 GMT  
		Size: 52.5 MB (52452198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34dc529b005dbeff70906cd4baf2310c918ae6379fdf53ef632c3cd1203aa38`  
		Last Modified: Tue, 12 Oct 2021 06:01:18 GMT  
		Size: 5.1 MB (5063794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2876b7f933f68a5b4f35f854cc8c651bf3d21476fe2bb0a786e6376f389b44b`  
		Last Modified: Tue, 12 Oct 2021 06:01:20 GMT  
		Size: 10.6 MB (10571017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c918a5faa65bffd689b9869a942e77a3fbc7d89566be880da188d6050f4f627`  
		Last Modified: Tue, 12 Oct 2021 06:02:11 GMT  
		Size: 52.3 MB (52322898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3127725d64ae6922801ff988a903c7db9c780283ffb0ed82afa5763076b47be7`  
		Last Modified: Tue, 12 Oct 2021 06:04:12 GMT  
		Size: 174.7 MB (174690436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:d56f41aa9c8faf2f038f7d533362e91ee583358bc719176d20f3c17daad0fb9f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.5 MB (282546908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7d3fb1baab35afcb64347548d5cecdba2a8cd3c4299b815347de10b18e7fa29`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 01:59:07 GMT
ADD file:43b45f65ff4ba720f6f9a107b5f80818d5ea6ebc4835840b11e9a506351da32f in / 
# Wed, 17 Nov 2021 01:59:08 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:41:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:42:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 02:43:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:45:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dbbf55137aab3c7acd1e012a70f1ea1adeaef8d39b474829965d3480a02bf572`  
		Last Modified: Wed, 17 Nov 2021 02:14:27 GMT  
		Size: 50.1 MB (50134152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb1ae7a04cee77523f9e09a62b28632c56a700d0c481be7cddc566c835e7a71d`  
		Last Modified: Wed, 17 Nov 2021 03:04:13 GMT  
		Size: 4.9 MB (4922782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66894dfea839186e94448f6c25a37c6b3b1b42cece6332cc9d36336917e18a4`  
		Last Modified: Wed, 17 Nov 2021 03:04:14 GMT  
		Size: 10.2 MB (10216965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4502933ba6aa2071501257e094faa363699dc23995f798a124d688c2523240af`  
		Last Modified: Wed, 17 Nov 2021 03:05:05 GMT  
		Size: 50.3 MB (50327664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b521106771559ec34e350caa7c1220e7d91669cfdd392f09bf61b4de0ffbfed6`  
		Last Modified: Wed, 17 Nov 2021 03:06:54 GMT  
		Size: 166.9 MB (166945345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:53545965440c95434bfc95e564fd274f086892b89a42ff4ff145f60ef5ba02df
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.3 MB (313267051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:455c971696419e341265a976576201f36454718c107fcd51d4c07ecf67d23d13`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:59 GMT
ADD file:eb667e18226da8a1ca5a41beacddc65cd1efec01c3d01e50845c5e89e91ea17c in / 
# Wed, 17 Nov 2021 02:40:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:26:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:26:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:27:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:27:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce18cd0ba11c2dfa8c1a2d2b325e1e019b14d4ae25ffdeffb0f9686c5496bf5c`  
		Last Modified: Wed, 17 Nov 2021 02:46:45 GMT  
		Size: 53.6 MB (53619024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f138a340a2373acc72dcc4ea9ef08bdf5648aabc5fe08f7e8d25222ca63b7ee`  
		Last Modified: Wed, 17 Nov 2021 13:36:26 GMT  
		Size: 4.9 MB (4937639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34c030205ccb8656e30a58f96bb1edbe7c59bf17f3329ae3c442ec897f2b270`  
		Last Modified: Wed, 17 Nov 2021 13:36:27 GMT  
		Size: 10.7 MB (10655878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7a1cfcc2070fbe1e702751d85f7074b93d142f6beb03ef66e9ba1c58bcc3e3`  
		Last Modified: Wed, 17 Nov 2021 13:36:49 GMT  
		Size: 54.7 MB (54669696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3503a35f6e45ec76f6c25673ef4934feb88c3c35ee30ffc8bf7437a0ade8e15`  
		Last Modified: Wed, 17 Nov 2021 13:37:28 GMT  
		Size: 189.4 MB (189384814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; 386

```console
$ docker pull buildpack-deps@sha256:22b4c7d5f90e61044a709672c2f9f4172afc8d87432cb5e8ec6165670064022b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.8 MB (327786933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd6b36232cd4509daee36d1370c035efee46f839cd7eca26d55136f8274a2db8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:39:30 GMT
ADD file:e007d6eff02dbc696e1166db315b97a77ae8aa65f2e66ca8074765dde9c70a59 in / 
# Tue, 12 Oct 2021 01:39:31 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:35:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:36:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 04:36:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:37:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6911c8f66691266d86e2cafa67ca005d919f357436fac971c694d37625b5ba90`  
		Last Modified: Tue, 12 Oct 2021 01:47:06 GMT  
		Size: 55.9 MB (55923419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a0f31369a20c178b1d5c84f192412ed962068e8932d5821eefb00bc7d1cbc1a`  
		Last Modified: Tue, 12 Oct 2021 04:47:26 GMT  
		Size: 5.3 MB (5283102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97aa3d222d7e8d6e0b06e57e5bd03168c422475942f92d09a487bd98d09bb742`  
		Last Modified: Tue, 12 Oct 2021 04:47:27 GMT  
		Size: 11.3 MB (11250699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae99d06bab5fc31ba3db9436a22c452db74a7b5e559a451de2d971a493abe52`  
		Last Modified: Tue, 12 Oct 2021 04:48:03 GMT  
		Size: 55.9 MB (55917451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ceaeace1516b23dd6c26014f977ec910629b0f1e818efcba72285c444c745dc`  
		Last Modified: Tue, 12 Oct 2021 04:49:16 GMT  
		Size: 199.4 MB (199412262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:a2b66ff7f5602d629f435424734849d38a6e15416a23b64b2d23e13178660e84
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.1 MB (301083355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a25bde1d7937a6f6dd29e4c251d24e4a821689a59f57bb28e96e734a349c0faa`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:09:46 GMT
ADD file:2971df49f24648b8d5166d87e392e2547d5b03469356f20d112ce6feb3c329fc in / 
# Wed, 17 Nov 2021 02:09:47 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:29:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:30:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 08:31:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:33:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b095a0b63d99a4c4cd9c1c353f381a69ef041e6f80798d807ae51a34b04920a0`  
		Last Modified: Wed, 17 Nov 2021 02:18:22 GMT  
		Size: 53.2 MB (53183806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2e37aff1692726b1ea3dd0b4eeb684072527295f8e981d3c45825327daea19`  
		Last Modified: Wed, 17 Nov 2021 08:45:38 GMT  
		Size: 5.1 MB (5114925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d4c0302ddd7a6cb573a156076dba9c593e09a0c321b32ae0f1da2bd36bc754`  
		Last Modified: Wed, 17 Nov 2021 08:45:41 GMT  
		Size: 10.9 MB (10873360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cde5eca075420fcfc6498f454dc040f1e236dea180a82a0d27d7a739ffd41c1`  
		Last Modified: Wed, 17 Nov 2021 08:46:32 GMT  
		Size: 53.3 MB (53296603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b326e913cf09f7b591a15250a21e659e1a1490c8db287698247813607f511be`  
		Last Modified: Wed, 17 Nov 2021 08:48:42 GMT  
		Size: 178.6 MB (178614661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3ad89b390c0582bf3f9073da22edc33da00fa72294f690312f20c8670974f6ae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.6 MB (330552911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c32d3a8d6d884cd659ea67e7f174cd8ba989c9582a46828d4a63585aeaf8c56f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 03:27:04 GMT
ADD file:85375acb19da58f9eabaa67f8cb425cd1ff2dadb2888bbd9dbfa6223d16fef23 in / 
# Wed, 17 Nov 2021 03:27:20 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 07:40:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 07:40:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 07:42:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 07:51:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ede9cd7c8f1d380c971a130fb3d8a3914bf3a9106702164c23b2cce536fa618c`  
		Last Modified: Wed, 17 Nov 2021 03:52:39 GMT  
		Size: 58.8 MB (58819505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743814bfd79326104da0238d8edced6b14f63b95734b6dc0e2b7a9d83356b0cb`  
		Last Modified: Wed, 17 Nov 2021 08:25:58 GMT  
		Size: 5.4 MB (5402000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca978d94a6543bbd1c60026602b64e810b4bf65e052dcf19adf2b4d6b518bf8`  
		Last Modified: Wed, 17 Nov 2021 08:25:59 GMT  
		Size: 11.6 MB (11626016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d785f1d8909cb3a3e46844611c28e15781da809be0073e40af017d6e5631d0`  
		Last Modified: Wed, 17 Nov 2021 08:26:57 GMT  
		Size: 58.9 MB (58851458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18fadd6314eacb7e881a9590b8566952a97cc84d87002b2f80c125e36f166f91`  
		Last Modified: Wed, 17 Nov 2021 08:28:32 GMT  
		Size: 195.9 MB (195853932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b771ceede0a02f3c3e45fbf245a79af43a82d8a5a89e280847ac77f34783db7f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.6 MB (295637108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:424bab9df7f41f34456e281a4d38395352c0b8a719a123e6e3da820dad5b62e2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:07 GMT
ADD file:b7524e775a2033d246d1096765a0eb6eaa5ba6ed6c8b395522579d2c4e7a2e38 in / 
# Wed, 17 Nov 2021 02:42:09 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:07:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:07:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:08:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:09:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ffa47acd07831fbc96680a705da20704bac0016c20dc3c454ecd45cda44b368d`  
		Last Modified: Wed, 17 Nov 2021 02:48:05 GMT  
		Size: 53.2 MB (53207179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c950336719691da019c99e4ff78fe559ab0308ea145757994bdb7be34c6d224`  
		Last Modified: Wed, 17 Nov 2021 03:17:18 GMT  
		Size: 5.1 MB (5137199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d769af2ca44d1c7c206e7190cd71df7cb5ff3df2dd45e1dd52ea447ffb547b1a`  
		Last Modified: Wed, 17 Nov 2021 03:17:19 GMT  
		Size: 10.8 MB (10761499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3bbc68017b41a8cc07b10d715e2a23108c5addefa80b01cac1a2ef075bb1acd`  
		Last Modified: Wed, 17 Nov 2021 03:17:36 GMT  
		Size: 54.0 MB (54041155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5890dc05b0932fa2fcd5ebf331e2dbb96bf6af4989173b3745e7228388fc8f0a`  
		Last Modified: Wed, 17 Nov 2021 03:18:03 GMT  
		Size: 172.5 MB (172490076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldoldstable`

```console
$ docker pull buildpack-deps@sha256:b83d6f9f3e784ab663beeddb4f9b15ec04f5ef9996f9fa9c28cb7ba7027aa558
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
$ docker pull buildpack-deps@sha256:1f84211ee3ff7baac91f583b97571f0abe60c11e1f29e0ebf5fa332b9d8981e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.2 MB (325233927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21c35b5593f396fdaa3497088189c39f7524d01ff424cd5f42eafc81bb0db7c1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:22:28 GMT
ADD file:d7365dd9cf34b10ca189f85c95c21a0c33e44092f85ffb5884d5e737fb0b9be1 in / 
# Wed, 17 Nov 2021 02:22:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:19:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:19:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:20:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:200cae5c9d88bb9cf1dd3fcfb831d671403f078d2310416fa3b304337d8279c0`  
		Last Modified: Wed, 17 Nov 2021 02:29:09 GMT  
		Size: 45.4 MB (45380444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047156b8adafd241846cd5539cebd45e6e28fe1bd818cd654a0124cef61d4cb2`  
		Last Modified: Wed, 17 Nov 2021 03:27:27 GMT  
		Size: 11.3 MB (11301447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cbf304dd51feb48b321b93ae5b8a5a6ca55c23b51a8dc0d9642c3c3b5081a7`  
		Last Modified: Wed, 17 Nov 2021 03:27:26 GMT  
		Size: 4.3 MB (4342326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6e9db633dd66ac91ed2df32c5900c5a1ae82b58cc9261fd240913743d283ca`  
		Last Modified: Wed, 17 Nov 2021 03:27:45 GMT  
		Size: 49.8 MB (49762330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16c1fa47fbffbf5d3d0c694fb480235a6ba765befaef57b62680514af6c2d0b8`  
		Last Modified: Wed, 17 Nov 2021 03:28:26 GMT  
		Size: 214.4 MB (214447380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:f1b619365d5dce8c961a51631354d01e66aadc6b82191aea0fde832ea20a8edc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.1 MB (309147959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8519ad77bacec454b6c51f92bdb6396c985f1edb4fc29146cadf27502ffe697e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 00:55:37 GMT
ADD file:eb65cc31f82e76c4ea5a8f21e4cad1372399517ee41a759740ff91d1d23b9e44 in / 
# Tue, 12 Oct 2021 00:55:38 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:54:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:54:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 05:55:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:58:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d2f67fd5897d122073fc9ad347c1fb9faec31555c47b3ee6ff64ca2b553034ed`  
		Last Modified: Tue, 12 Oct 2021 01:13:31 GMT  
		Size: 44.1 MB (44091932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b4f8f4eb65e840d4778dd2e77e7cc6d546cbd55ed717e53e017c853e7c07d1`  
		Last Modified: Tue, 12 Oct 2021 06:12:15 GMT  
		Size: 10.4 MB (10351740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec0c01cd7d7e35fbb8d775a4bca6166749569cbf3c1bc4b9a5aee530bff8978`  
		Last Modified: Tue, 12 Oct 2021 06:12:12 GMT  
		Size: 4.2 MB (4161429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb3ac8456e186fb75e7aaf1c21260430344e8cf1d6cd6fdaec9bfb9ab5a0741`  
		Last Modified: Tue, 12 Oct 2021 06:12:58 GMT  
		Size: 48.0 MB (47984451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e836375083dc2ab922dd843b4cf24c13682693e3391b6c1429c233240bafa36b`  
		Last Modified: Tue, 12 Oct 2021 06:15:09 GMT  
		Size: 202.6 MB (202558407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:34e043644f0b3472348ca1922c817cfead39d47718cd0bf195b133b74594853d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.2 MB (297172929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:629cf466cec2a9b62004e6fabb013a03aaa948260188a7536d7039dd7d23f63e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:04:57 GMT
ADD file:61da3fcef3aea99b4927189cfcb823a65b0e911a3f4436e44ea84a57a7919ff3 in / 
# Wed, 17 Nov 2021 02:04:58 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:54:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:54:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 02:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:57:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e4d54b576c2fcdd259e57bac14c4e1a2623f6e5dc9a0b1facaed7fe59d891e86`  
		Last Modified: Wed, 17 Nov 2021 02:22:03 GMT  
		Size: 42.1 MB (42116868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf04dd2447fcded30a4c9a8d7a054ccb2e4c4db4118989ea05bf2e56d60a8924`  
		Last Modified: Wed, 17 Nov 2021 03:14:24 GMT  
		Size: 10.0 MB (9956153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b37c8e78d6ca4f8e5467e0ec7ef61eef6101e99c8154472df98aa34159f5974`  
		Last Modified: Wed, 17 Nov 2021 03:14:21 GMT  
		Size: 3.9 MB (3921214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fcf28009119cc468ce87b98d583e8c51d3703937d10d502a704f1032bc2b26`  
		Last Modified: Wed, 17 Nov 2021 03:15:08 GMT  
		Size: 46.1 MB (46126162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b8b79b0de7febe2c3b866e2f14fe48bca033ef5ee3eda5193c147f47eb3f55`  
		Last Modified: Wed, 17 Nov 2021 03:17:08 GMT  
		Size: 195.1 MB (195052532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:eb62a7fc0d18f0f9cde800bdbec22f5baf0e77c4d4be12290a6dfe5dd5dff258
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.8 MB (306765224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef6ac97bc2ecd37279a6f1b4e04c10b22609eeabb9496051c80999f502d8d752`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:33 GMT
ADD file:3225671be4edc3599e29ebd06516b95573246e68bf29649c402ed87c03c109b5 in / 
# Wed, 17 Nov 2021 02:42:34 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:32:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:32:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:32:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:33:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c64a4bafe4ad6fc05fcc6d76d2a06f168f331ffbc87e518fb4ca4ea22e75527e`  
		Last Modified: Wed, 17 Nov 2021 02:51:11 GMT  
		Size: 43.2 MB (43174478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deaddc7c2a37cd151a9001bbe7816f06f5f36ac6d53cc0d02fe2b327f85a2c7e`  
		Last Modified: Wed, 17 Nov 2021 13:40:24 GMT  
		Size: 10.2 MB (10216788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61401ffc70123532d1f4886b9ebd00e11d1155a2363117bf5aab10353c373dc9`  
		Last Modified: Wed, 17 Nov 2021 13:40:23 GMT  
		Size: 3.9 MB (3873891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185eee4daee1ed1fa34e853c2332cc4253415d7e015143b2432a96047c88d828`  
		Last Modified: Wed, 17 Nov 2021 13:40:43 GMT  
		Size: 47.7 MB (47734854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc999035e89072506c3f538d25644144fcabf1babfd2b71bfdd62c2ac570b8d0`  
		Last Modified: Wed, 17 Nov 2021 13:41:25 GMT  
		Size: 201.8 MB (201765213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:d51e19c8a7f30a56580661332d964aa73ab70b00fc602feeb7c96051a8d3794d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.7 MB (332749925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e1c89142617e6ea716a487a28ff686e7b1826f983f94e53ab383bb6677f224c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:42:19 GMT
ADD file:5a6f08cc731f24357c3702231256fb05eb0a97733779b2ace406ba3c9bf64baa in / 
# Tue, 12 Oct 2021 01:42:19 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:42:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:42:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 04:43:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:44:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d2ef4e90cca7406b4907a34e3571153fc56e3ecc9b2b5fdbb7787f22877cfec5`  
		Last Modified: Tue, 12 Oct 2021 01:51:58 GMT  
		Size: 46.1 MB (46097164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9020db84c7cf31b7929c21a2b6fe2123900e91c7391ad6f4ee5560a934f382`  
		Last Modified: Tue, 12 Oct 2021 04:52:49 GMT  
		Size: 11.4 MB (11358857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8cbe9196a8b6bd3825445c718bc5a248b7c295b4d9f45756819e8bf27cb72b`  
		Last Modified: Tue, 12 Oct 2021 04:52:47 GMT  
		Size: 4.6 MB (4565012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7454f0fe0ebf5d024897d682d46181ab978a980f7f40caa2492a83cc39f75ec`  
		Last Modified: Tue, 12 Oct 2021 04:53:20 GMT  
		Size: 51.3 MB (51264783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d689f4cc817a5dea61b3cd4ed2680f093caa75b7c811cee4392ea0effff4f5c`  
		Last Modified: Tue, 12 Oct 2021 04:54:33 GMT  
		Size: 219.5 MB (219464109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldoldstable-curl`

```console
$ docker pull buildpack-deps@sha256:e2c7c02aeaae59464b9bf9a1315c291bcaef9b2b840b0750e6c242d20a1714b0
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
$ docker pull buildpack-deps@sha256:cf8274ff3f94d52058249c3fa2a3fa6f58da3f51f5bbaa18d26d451a11e55190
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.0 MB (61024217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0886d8702caa5ba4caa2911a9a70b0d489f272aa850952a75f880b9f4664d388`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:22:28 GMT
ADD file:d7365dd9cf34b10ca189f85c95c21a0c33e44092f85ffb5884d5e737fb0b9be1 in / 
# Wed, 17 Nov 2021 02:22:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:19:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:200cae5c9d88bb9cf1dd3fcfb831d671403f078d2310416fa3b304337d8279c0`  
		Last Modified: Wed, 17 Nov 2021 02:29:09 GMT  
		Size: 45.4 MB (45380444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047156b8adafd241846cd5539cebd45e6e28fe1bd818cd654a0124cef61d4cb2`  
		Last Modified: Wed, 17 Nov 2021 03:27:27 GMT  
		Size: 11.3 MB (11301447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cbf304dd51feb48b321b93ae5b8a5a6ca55c23b51a8dc0d9642c3c3b5081a7`  
		Last Modified: Wed, 17 Nov 2021 03:27:26 GMT  
		Size: 4.3 MB (4342326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:d22384305baafb9cd36935a9bdefcf829118d3d1458b5d353798b97b3f6e83d3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.6 MB (58605101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddb7b424b63a5db211ff320d4629b66d91f09ff2fff4d2236cdc7316f3201f9c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 00:55:37 GMT
ADD file:eb65cc31f82e76c4ea5a8f21e4cad1372399517ee41a759740ff91d1d23b9e44 in / 
# Tue, 12 Oct 2021 00:55:38 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:54:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:54:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d2f67fd5897d122073fc9ad347c1fb9faec31555c47b3ee6ff64ca2b553034ed`  
		Last Modified: Tue, 12 Oct 2021 01:13:31 GMT  
		Size: 44.1 MB (44091932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b4f8f4eb65e840d4778dd2e77e7cc6d546cbd55ed717e53e017c853e7c07d1`  
		Last Modified: Tue, 12 Oct 2021 06:12:15 GMT  
		Size: 10.4 MB (10351740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec0c01cd7d7e35fbb8d775a4bca6166749569cbf3c1bc4b9a5aee530bff8978`  
		Last Modified: Tue, 12 Oct 2021 06:12:12 GMT  
		Size: 4.2 MB (4161429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:2e294312a129ae76beed8f6db683fefb2075deea7406f388f37b2aa606cebb30
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (55994235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ac3b5ed742906ac82c169d00412d6043ee6e55561442421ef66c7d392c8506d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:04:57 GMT
ADD file:61da3fcef3aea99b4927189cfcb823a65b0e911a3f4436e44ea84a57a7919ff3 in / 
# Wed, 17 Nov 2021 02:04:58 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:54:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:54:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e4d54b576c2fcdd259e57bac14c4e1a2623f6e5dc9a0b1facaed7fe59d891e86`  
		Last Modified: Wed, 17 Nov 2021 02:22:03 GMT  
		Size: 42.1 MB (42116868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf04dd2447fcded30a4c9a8d7a054ccb2e4c4db4118989ea05bf2e56d60a8924`  
		Last Modified: Wed, 17 Nov 2021 03:14:24 GMT  
		Size: 10.0 MB (9956153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b37c8e78d6ca4f8e5467e0ec7ef61eef6101e99c8154472df98aa34159f5974`  
		Last Modified: Wed, 17 Nov 2021 03:14:21 GMT  
		Size: 3.9 MB (3921214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f8c63f2967bc872468d5e51917554a8ea360b461f6c6b1461b826a6442d19490
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.3 MB (57265157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:014f4bdee0c150fb8cf8cdfff5d193c2eaced3df30b883271791d6a840b6567b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:33 GMT
ADD file:3225671be4edc3599e29ebd06516b95573246e68bf29649c402ed87c03c109b5 in / 
# Wed, 17 Nov 2021 02:42:34 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:32:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:32:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c64a4bafe4ad6fc05fcc6d76d2a06f168f331ffbc87e518fb4ca4ea22e75527e`  
		Last Modified: Wed, 17 Nov 2021 02:51:11 GMT  
		Size: 43.2 MB (43174478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deaddc7c2a37cd151a9001bbe7816f06f5f36ac6d53cc0d02fe2b327f85a2c7e`  
		Last Modified: Wed, 17 Nov 2021 13:40:24 GMT  
		Size: 10.2 MB (10216788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61401ffc70123532d1f4886b9ebd00e11d1155a2363117bf5aab10353c373dc9`  
		Last Modified: Wed, 17 Nov 2021 13:40:23 GMT  
		Size: 3.9 MB (3873891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:27a549af269a461e6896cf3b3a7199e34e7417ff4f572c30ff2815b85cf0d5b5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (62021033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0aa60dbddb29720e51a7ec1ada2bba0a56158d345ab8caed4a5537a267eb8957`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:42:19 GMT
ADD file:5a6f08cc731f24357c3702231256fb05eb0a97733779b2ace406ba3c9bf64baa in / 
# Tue, 12 Oct 2021 01:42:19 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:42:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:42:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d2ef4e90cca7406b4907a34e3571153fc56e3ecc9b2b5fdbb7787f22877cfec5`  
		Last Modified: Tue, 12 Oct 2021 01:51:58 GMT  
		Size: 46.1 MB (46097164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9020db84c7cf31b7929c21a2b6fe2123900e91c7391ad6f4ee5560a934f382`  
		Last Modified: Tue, 12 Oct 2021 04:52:49 GMT  
		Size: 11.4 MB (11358857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8cbe9196a8b6bd3825445c718bc5a248b7c295b4d9f45756819e8bf27cb72b`  
		Last Modified: Tue, 12 Oct 2021 04:52:47 GMT  
		Size: 4.6 MB (4565012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldoldstable-scm`

```console
$ docker pull buildpack-deps@sha256:671522708995c6015365c1ffbf4ec04af96a02b3cd6b4fe799ae946fc7dab362
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
$ docker pull buildpack-deps@sha256:b0f76319830edb0ebac43cd1e76a4c2a5d34e847b9bb3f7371bbfebe57eb205f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.8 MB (110786547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cea98b6e932cedec41f17989129c68a1bd3d343c834ab1c992efb3bc8544888`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:22:28 GMT
ADD file:d7365dd9cf34b10ca189f85c95c21a0c33e44092f85ffb5884d5e737fb0b9be1 in / 
# Wed, 17 Nov 2021 02:22:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:19:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:19:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:200cae5c9d88bb9cf1dd3fcfb831d671403f078d2310416fa3b304337d8279c0`  
		Last Modified: Wed, 17 Nov 2021 02:29:09 GMT  
		Size: 45.4 MB (45380444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047156b8adafd241846cd5539cebd45e6e28fe1bd818cd654a0124cef61d4cb2`  
		Last Modified: Wed, 17 Nov 2021 03:27:27 GMT  
		Size: 11.3 MB (11301447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cbf304dd51feb48b321b93ae5b8a5a6ca55c23b51a8dc0d9642c3c3b5081a7`  
		Last Modified: Wed, 17 Nov 2021 03:27:26 GMT  
		Size: 4.3 MB (4342326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6e9db633dd66ac91ed2df32c5900c5a1ae82b58cc9261fd240913743d283ca`  
		Last Modified: Wed, 17 Nov 2021 03:27:45 GMT  
		Size: 49.8 MB (49762330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:3b6dcef1865cc1d9df51cfcede2b22a42810d59e1ed7f2dd6f1a2afdab2da382
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.6 MB (106589552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f1b47c4fc7cd09da1eadb373e1b3639dd3ea6f0d0a7f277a6f9a3a1badf1916`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 00:55:37 GMT
ADD file:eb65cc31f82e76c4ea5a8f21e4cad1372399517ee41a759740ff91d1d23b9e44 in / 
# Tue, 12 Oct 2021 00:55:38 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:54:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:54:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 05:55:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d2f67fd5897d122073fc9ad347c1fb9faec31555c47b3ee6ff64ca2b553034ed`  
		Last Modified: Tue, 12 Oct 2021 01:13:31 GMT  
		Size: 44.1 MB (44091932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b4f8f4eb65e840d4778dd2e77e7cc6d546cbd55ed717e53e017c853e7c07d1`  
		Last Modified: Tue, 12 Oct 2021 06:12:15 GMT  
		Size: 10.4 MB (10351740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec0c01cd7d7e35fbb8d775a4bca6166749569cbf3c1bc4b9a5aee530bff8978`  
		Last Modified: Tue, 12 Oct 2021 06:12:12 GMT  
		Size: 4.2 MB (4161429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb3ac8456e186fb75e7aaf1c21260430344e8cf1d6cd6fdaec9bfb9ab5a0741`  
		Last Modified: Tue, 12 Oct 2021 06:12:58 GMT  
		Size: 48.0 MB (47984451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:06b12ba3a191d0ec83b7588cd9cb7e94e5206746fe70cef1b57974f1c21f5097
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102120397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c01627a3706745a8b4f9600a77ff4453ce771391c424dff9199dbdfbec858c24`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:04:57 GMT
ADD file:61da3fcef3aea99b4927189cfcb823a65b0e911a3f4436e44ea84a57a7919ff3 in / 
# Wed, 17 Nov 2021 02:04:58 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:54:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:54:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 02:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e4d54b576c2fcdd259e57bac14c4e1a2623f6e5dc9a0b1facaed7fe59d891e86`  
		Last Modified: Wed, 17 Nov 2021 02:22:03 GMT  
		Size: 42.1 MB (42116868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf04dd2447fcded30a4c9a8d7a054ccb2e4c4db4118989ea05bf2e56d60a8924`  
		Last Modified: Wed, 17 Nov 2021 03:14:24 GMT  
		Size: 10.0 MB (9956153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b37c8e78d6ca4f8e5467e0ec7ef61eef6101e99c8154472df98aa34159f5974`  
		Last Modified: Wed, 17 Nov 2021 03:14:21 GMT  
		Size: 3.9 MB (3921214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fcf28009119cc468ce87b98d583e8c51d3703937d10d502a704f1032bc2b26`  
		Last Modified: Wed, 17 Nov 2021 03:15:08 GMT  
		Size: 46.1 MB (46126162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:eee3dd1c4660b65af7e8f4b3b200e6b89d3b7f43fa955fcb1678a602aef8a32e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105000011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52b744ede03418aaf0da398c56b90d7f07486c457d319e40f083d7ed41ea3639`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:33 GMT
ADD file:3225671be4edc3599e29ebd06516b95573246e68bf29649c402ed87c03c109b5 in / 
# Wed, 17 Nov 2021 02:42:34 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:32:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:32:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:32:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c64a4bafe4ad6fc05fcc6d76d2a06f168f331ffbc87e518fb4ca4ea22e75527e`  
		Last Modified: Wed, 17 Nov 2021 02:51:11 GMT  
		Size: 43.2 MB (43174478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deaddc7c2a37cd151a9001bbe7816f06f5f36ac6d53cc0d02fe2b327f85a2c7e`  
		Last Modified: Wed, 17 Nov 2021 13:40:24 GMT  
		Size: 10.2 MB (10216788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61401ffc70123532d1f4886b9ebd00e11d1155a2363117bf5aab10353c373dc9`  
		Last Modified: Wed, 17 Nov 2021 13:40:23 GMT  
		Size: 3.9 MB (3873891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185eee4daee1ed1fa34e853c2332cc4253415d7e015143b2432a96047c88d828`  
		Last Modified: Wed, 17 Nov 2021 13:40:43 GMT  
		Size: 47.7 MB (47734854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:3dd7dfec75397dae002735d04557b86aaaf641dbf609cd11f267f7740392d841
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.3 MB (113285816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10424f2f9fa56c237f5a1cb67f32e5286a03841b408bf07e8c6d4f87b5757030`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:42:19 GMT
ADD file:5a6f08cc731f24357c3702231256fb05eb0a97733779b2ace406ba3c9bf64baa in / 
# Tue, 12 Oct 2021 01:42:19 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:42:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:42:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 04:43:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d2ef4e90cca7406b4907a34e3571153fc56e3ecc9b2b5fdbb7787f22877cfec5`  
		Last Modified: Tue, 12 Oct 2021 01:51:58 GMT  
		Size: 46.1 MB (46097164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9020db84c7cf31b7929c21a2b6fe2123900e91c7391ad6f4ee5560a934f382`  
		Last Modified: Tue, 12 Oct 2021 04:52:49 GMT  
		Size: 11.4 MB (11358857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8cbe9196a8b6bd3825445c718bc5a248b7c295b4d9f45756819e8bf27cb72b`  
		Last Modified: Tue, 12 Oct 2021 04:52:47 GMT  
		Size: 4.6 MB (4565012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7454f0fe0ebf5d024897d682d46181ab978a980f7f40caa2492a83cc39f75ec`  
		Last Modified: Tue, 12 Oct 2021 04:53:20 GMT  
		Size: 51.3 MB (51264783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldstable`

```console
$ docker pull buildpack-deps@sha256:33cb41bdc60ac651ee2fb97714dc86af89bf1cf52fb8827f350aff333ddcd490
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
$ docker pull buildpack-deps@sha256:40214612fb01ceeb7860226a8a782a8d50a4850847f78981cf364d8084d147de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.5 MB (312533991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0413fe230a75e8ed7ab2771c02492189116b86729fd184bba5339a1bac348050`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:51 GMT
ADD file:cb5ed7070880d4c0177fbe6dd278adb7926e38cd73e6abd582fd8d67e4bbf06c in / 
# Wed, 17 Nov 2021 02:20:51 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:15:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:15:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:16:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:17:16 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1230f17f526cb07307d41462355b10488b994e8bdafe0d8f275a405fa3b33831`  
		Last Modified: Wed, 17 Nov 2021 02:26:06 GMT  
		Size: 50.4 MB (50437098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17d0de332ca1b34d53ca41c2b39ea52ce72f8c1e81c5200e27a8bade3e6ecbb`  
		Last Modified: Wed, 17 Nov 2021 03:24:34 GMT  
		Size: 7.8 MB (7833787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7474d56348f5333567750c1e5f06f899477fd437330627341eafa71bfa1a36ab`  
		Last Modified: Wed, 17 Nov 2021 03:24:34 GMT  
		Size: 10.0 MB (9997183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211c565de40518c5dac4498ccebbf3833fcfaa5db17d4bf94e6bef466136278b`  
		Last Modified: Wed, 17 Nov 2021 03:24:55 GMT  
		Size: 51.8 MB (51840474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71337a3dfc6f79fe42b06f2f3872667ca6d9ebac8029afcf6df3b0ee321f509f`  
		Last Modified: Wed, 17 Nov 2021 03:25:36 GMT  
		Size: 192.4 MB (192425449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:992531625663e82ea52458ff2a822637f40c4e415c9b30c62882cc47da243925
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.1 MB (286144717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea6ba2c3224423f294f623719618096fa1d795d97560237193e8196cb8ab8d61`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 00:50:58 GMT
ADD file:f9432d6da0faddeaa117c57c0c007cd56738ef01549baf71e5c59939b7e69b6c in / 
# Tue, 12 Oct 2021 00:50:59 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:45:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:45:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 05:46:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:48:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ae00de77d9c27fe3ba9ea06833b273e4fc0aa128a3a61d3992632e6e3941a78c`  
		Last Modified: Tue, 12 Oct 2021 01:07:01 GMT  
		Size: 48.2 MB (48154085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52282bf2103fc337ab7cc23ebfae979096e6f901b62960b03952c2d52e9978db`  
		Last Modified: Tue, 12 Oct 2021 06:04:31 GMT  
		Size: 7.4 MB (7377193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b1aa5c1e770fff74bdcd066b443f1e1e49f677ae77ec80d22c50e20be8c3b3`  
		Last Modified: Tue, 12 Oct 2021 06:04:32 GMT  
		Size: 9.7 MB (9687494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b03f47e60dacc119379be5c6a6d690ee9ebe00c3a3f7755e295b572e9d4817aa`  
		Last Modified: Tue, 12 Oct 2021 06:05:19 GMT  
		Size: 49.6 MB (49574809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f680c95108ec6b108b9dcd987cc473d268506328d38866d5b6aa0e44ff73c8dd`  
		Last Modified: Tue, 12 Oct 2021 06:07:13 GMT  
		Size: 171.4 MB (171351136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:b7df7895ed903ba0d50d3c0b59280a0b329ac98b9b89a1997c0a1db9cdba9b31
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.4 MB (278351711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3172590d3c7dc0fb07cd01d18ebc7811c421c9409f6f8624ff870b62a5a0351e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:00:12 GMT
ADD file:d71807613acdf86685f6d640a90e27b7b63cfe0f13d88668ee943aca089d8876 in / 
# Wed, 17 Nov 2021 02:00:13 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:45:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:45:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 02:46:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:48:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10acd81022d17f452439d0385615fa066b8f0ddcf3c1a803872eec5bdc6acf64`  
		Last Modified: Wed, 17 Nov 2021 02:16:00 GMT  
		Size: 45.9 MB (45918099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a9604eb6c465f658d6422593d504030155029fe0c4302451d4369030c29144`  
		Last Modified: Wed, 17 Nov 2021 03:07:14 GMT  
		Size: 7.1 MB (7125194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b043b954c4f0757e89df96897cea2cf1f93c6275466008e4ba7a4b1089c7dd3d`  
		Last Modified: Wed, 17 Nov 2021 03:07:15 GMT  
		Size: 9.3 MB (9343839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf41461745fd89900c4b7cc794c93de081420bd83223b46e1495ff96748685c`  
		Last Modified: Wed, 17 Nov 2021 03:07:59 GMT  
		Size: 47.4 MB (47356485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4cebe2126c416f6186078f6b19742a166f0d535016a910ed5bd1bed73ab5ab`  
		Last Modified: Wed, 17 Nov 2021 03:09:46 GMT  
		Size: 168.6 MB (168608094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a781bc03f60fd23b4f3bc527115eae336c4406da469a32b05e5a8cb879285c0c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.8 MB (302842791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d89bb85d03bfdc93c6f242b95047eda9fd8a32f57973d9615c0bf809eb00c27f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:27 GMT
ADD file:c7e9e884b1494f96e33e9d9a892b51367af8943edb282c4101cc99ea78a7753f in / 
# Wed, 17 Nov 2021 02:40:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:28:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:28:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:28:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:29:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:626979e62c56e192812e818d52b82f063d9f9514b1b7bae14e534e4a7c98117a`  
		Last Modified: Wed, 17 Nov 2021 02:47:40 GMT  
		Size: 49.2 MB (49222990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134a528370d5dcbf5b6ba2d8c20f576504448e8f2d1debb5d2a4950a38a3ff2d`  
		Last Modified: Wed, 17 Nov 2021 13:37:44 GMT  
		Size: 7.7 MB (7695161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e12e3364b52ad043d8e79f750863ed4ca2878c4fdf45ded974508febc55fdd`  
		Last Modified: Wed, 17 Nov 2021 13:37:44 GMT  
		Size: 9.8 MB (9767133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a7f2500f9574b0a495bfb031c2d52e83c96dd545ef2185737f8032567e70677`  
		Last Modified: Wed, 17 Nov 2021 13:38:03 GMT  
		Size: 52.2 MB (52165947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16922d4fa4f2c649c56a586e06135309b0cc7e160a17c909e5eb349988df61aa`  
		Last Modified: Wed, 17 Nov 2021 13:38:38 GMT  
		Size: 184.0 MB (183991560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:07a84d8bf937d4befea7f1d2878f2f7b46a31fdc00d5d6891072304ae83b4d06
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.9 MB (321944968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00f2f20bac236128ca2d426c71e0fc49ae840c119b299d797809f4c224bc7948`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:40:01 GMT
ADD file:1461fa0362c70b5b7a677c57dd48633827fd9635a9cb136730aa7581cc523b46 in / 
# Tue, 12 Oct 2021 01:40:02 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:37:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:38:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 04:38:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:39:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f4b233498baa64e956a5f70979351e206bd085bd547a3cf25c08b154348df726`  
		Last Modified: Tue, 12 Oct 2021 01:48:07 GMT  
		Size: 51.2 MB (51207606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece122ff48522de249e81ee22f617bf84d59b003d3c79f44331163046a937e4c`  
		Last Modified: Tue, 12 Oct 2021 04:49:37 GMT  
		Size: 8.0 MB (8000221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:378307f52e8eeddb964324804377cd9fd65b1bf7b848c5b690e63ef92f1fe3d5`  
		Last Modified: Tue, 12 Oct 2021 04:49:37 GMT  
		Size: 10.3 MB (10339916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559cdd7287c6a9a0f142216d3645f886b4a777073daae85c51de968330bb9f9d`  
		Last Modified: Tue, 12 Oct 2021 04:50:08 GMT  
		Size: 53.4 MB (53437801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:325db7f1d3dd664f85cad29c0867f78c550d2b5c426ed460bf5283c008942bb6`  
		Last Modified: Tue, 12 Oct 2021 04:50:59 GMT  
		Size: 199.0 MB (198959424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:30c758f087fd5312ed4d5cfbda2905fd550e0d3738afdeb1030499c4f12a1ccc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.1 MB (297128262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c90dc68a1536bdf0771a84535d0ccf2a3e57ae0ac87df32c471fe9265da620b0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:10:39 GMT
ADD file:4769a173ec92e69a1b5cd79af0ed018bf150d1ee278de07f4bdab45f55f3c818 in / 
# Wed, 17 Nov 2021 02:10:40 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:34:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:34:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 08:36:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:39:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8c028c43f55209ca75650433b923c8952e16d106529242daad16c3be3efd66a3`  
		Last Modified: Wed, 17 Nov 2021 02:19:53 GMT  
		Size: 49.1 MB (49079535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:762a68d988b283d25c4ea122ea03a45caa2b4174b9d1df992298cef4bc15678f`  
		Last Modified: Wed, 17 Nov 2021 08:48:59 GMT  
		Size: 7.3 MB (7253673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a792c079b6714bc5d104fd824622583cd79ee86bf0cd4bd3930290e5bea3a81`  
		Last Modified: Wed, 17 Nov 2021 08:48:59 GMT  
		Size: 10.0 MB (10016437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0c1cd6c6ead61c438a2c08e4c9cc9d3c5ff225d437de4052cd5b03699bdae3`  
		Last Modified: Wed, 17 Nov 2021 08:49:46 GMT  
		Size: 50.8 MB (50844942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4347eaf923b6e261b09fec9e7c6e3e06fee0595ef1609e0e9f25be6a2b8428`  
		Last Modified: Wed, 17 Nov 2021 08:51:52 GMT  
		Size: 179.9 MB (179933675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:b87c8fcad8f67a37fdb8dd3764fdcc849043fe943f3f5ac261f37c0aed85d80e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.9 MB (333943769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30105f5450a73d27a5f54e7976ea986d267e0f70bccf47c138963ac685d08dc2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 03:29:10 GMT
ADD file:fc0d43ba74311deef20b2131cca3a8e86b083624d63560251191adca21417f2f in / 
# Wed, 17 Nov 2021 03:29:20 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 07:52:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 07:53:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 07:55:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:06:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:aad6e1fe6f7c56b0e1b5850f40e4fec91ffaed4b6235e730f5c7ff43db397d3d`  
		Last Modified: Wed, 17 Nov 2021 03:56:39 GMT  
		Size: 54.2 MB (54183702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38c773e3945e9939b7299519ac8a7f3ad909af69c2d7291d8dfb6e7fa6eccfe`  
		Last Modified: Wed, 17 Nov 2021 08:28:50 GMT  
		Size: 8.3 MB (8272985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65e0d54cc06e26d154b6f6e9746c8de2af93d9f635c280336663372f382fcd46`  
		Last Modified: Wed, 17 Nov 2021 08:28:49 GMT  
		Size: 10.7 MB (10727776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3239f513a520f7d81f241b123128d80a0c91d3ef8697270ffae67898934cb4f9`  
		Last Modified: Wed, 17 Nov 2021 08:29:36 GMT  
		Size: 57.5 MB (57457385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f80735649ead4029d67b9d28dac87b66bb06e2548f5c0d68c5f9877855d41c`  
		Last Modified: Wed, 17 Nov 2021 08:31:23 GMT  
		Size: 203.3 MB (203301921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:2a549a62e97fa58428a04001462c87f88b3fa92be5fcce03ca6280f6de3c9e46
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.6 MB (294582808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a55feeaee694c81b717cd5fcae296288c5700416bf32d57d56cc2249119570da`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:40 GMT
ADD file:dc4ee96f81059accdc88a686f80f1714bc9d2f383af71c0d130c08560cea115e in / 
# Wed, 17 Nov 2021 02:42:42 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:10:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:10:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:10:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:11:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c12eae84d2674466d924a139a276e361afa9f63de21cf77eae19bd94eaac2629`  
		Last Modified: Wed, 17 Nov 2021 02:48:42 GMT  
		Size: 49.0 MB (49005439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564a8b4bf4cf08933f04084cd556e9c716474b9801854ea7c4473c9804894516`  
		Last Modified: Wed, 17 Nov 2021 03:18:14 GMT  
		Size: 7.4 MB (7401273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ffdc4b0bb501f5f5214892baa1a5d53d44ce92b645995a43fe2cfeb2ffec6d1`  
		Last Modified: Wed, 17 Nov 2021 03:18:14 GMT  
		Size: 9.9 MB (9883156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb48942b4b14ee80905b23bc6babae28a961847a914becfe41686d368d8693d`  
		Last Modified: Wed, 17 Nov 2021 03:18:28 GMT  
		Size: 51.4 MB (51380227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3deaef082aa42f5164fd0beb9cf445ba4867c9ad41c784080a427bc615a02df9`  
		Last Modified: Wed, 17 Nov 2021 03:18:54 GMT  
		Size: 176.9 MB (176912713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldstable-curl`

```console
$ docker pull buildpack-deps@sha256:d58c6560d64100478b91c5a36db1baa7299fd98f69cba651c222abd37b5b6396
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
$ docker pull buildpack-deps@sha256:a0bba8f1fd79022a347c88c8ba94f43b7b9a85b2a241a977a2d15ff65f3b9974
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68268068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae7b4dd26afae147336976cacba2d6de091e5f31ce99148eadb745564c75cdf8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:51 GMT
ADD file:cb5ed7070880d4c0177fbe6dd278adb7926e38cd73e6abd582fd8d67e4bbf06c in / 
# Wed, 17 Nov 2021 02:20:51 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:15:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:15:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1230f17f526cb07307d41462355b10488b994e8bdafe0d8f275a405fa3b33831`  
		Last Modified: Wed, 17 Nov 2021 02:26:06 GMT  
		Size: 50.4 MB (50437098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17d0de332ca1b34d53ca41c2b39ea52ce72f8c1e81c5200e27a8bade3e6ecbb`  
		Last Modified: Wed, 17 Nov 2021 03:24:34 GMT  
		Size: 7.8 MB (7833787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7474d56348f5333567750c1e5f06f899477fd437330627341eafa71bfa1a36ab`  
		Last Modified: Wed, 17 Nov 2021 03:24:34 GMT  
		Size: 10.0 MB (9997183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:b140abc457f97daff918385b366ef37a61f11bd24028a0f05be0fd904723f38c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65218772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ca71e57b57c8f55f460a4ef80141da4552e2dd1317eccfae4a8f32e70126712`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 00:50:58 GMT
ADD file:f9432d6da0faddeaa117c57c0c007cd56738ef01549baf71e5c59939b7e69b6c in / 
# Tue, 12 Oct 2021 00:50:59 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:45:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:45:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ae00de77d9c27fe3ba9ea06833b273e4fc0aa128a3a61d3992632e6e3941a78c`  
		Last Modified: Tue, 12 Oct 2021 01:07:01 GMT  
		Size: 48.2 MB (48154085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52282bf2103fc337ab7cc23ebfae979096e6f901b62960b03952c2d52e9978db`  
		Last Modified: Tue, 12 Oct 2021 06:04:31 GMT  
		Size: 7.4 MB (7377193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b1aa5c1e770fff74bdcd066b443f1e1e49f677ae77ec80d22c50e20be8c3b3`  
		Last Modified: Tue, 12 Oct 2021 06:04:32 GMT  
		Size: 9.7 MB (9687494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:e724e938ae162d22679aa13688acc32788d5193b4f552dfd33702ad1843e3bc7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62387132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b37d37a14a96bf4731ecee8b62e9002e52f378b5a25d0f6668dbc7a96554394a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:00:12 GMT
ADD file:d71807613acdf86685f6d640a90e27b7b63cfe0f13d88668ee943aca089d8876 in / 
# Wed, 17 Nov 2021 02:00:13 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:45:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:45:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:10acd81022d17f452439d0385615fa066b8f0ddcf3c1a803872eec5bdc6acf64`  
		Last Modified: Wed, 17 Nov 2021 02:16:00 GMT  
		Size: 45.9 MB (45918099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a9604eb6c465f658d6422593d504030155029fe0c4302451d4369030c29144`  
		Last Modified: Wed, 17 Nov 2021 03:07:14 GMT  
		Size: 7.1 MB (7125194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b043b954c4f0757e89df96897cea2cf1f93c6275466008e4ba7a4b1089c7dd3d`  
		Last Modified: Wed, 17 Nov 2021 03:07:15 GMT  
		Size: 9.3 MB (9343839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:10f1a26aec27e58769c26f86b48604d74076ae1af479444ae540e2b73260466b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66685284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af10d3fa6817ac70b7abf7cf182c08ca8c2e382178327e9aaf6bf86ea8ebccf5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:27 GMT
ADD file:c7e9e884b1494f96e33e9d9a892b51367af8943edb282c4101cc99ea78a7753f in / 
# Wed, 17 Nov 2021 02:40:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:28:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:28:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:626979e62c56e192812e818d52b82f063d9f9514b1b7bae14e534e4a7c98117a`  
		Last Modified: Wed, 17 Nov 2021 02:47:40 GMT  
		Size: 49.2 MB (49222990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134a528370d5dcbf5b6ba2d8c20f576504448e8f2d1debb5d2a4950a38a3ff2d`  
		Last Modified: Wed, 17 Nov 2021 13:37:44 GMT  
		Size: 7.7 MB (7695161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e12e3364b52ad043d8e79f750863ed4ca2878c4fdf45ded974508febc55fdd`  
		Last Modified: Wed, 17 Nov 2021 13:37:44 GMT  
		Size: 9.8 MB (9767133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:2486e26715fffc0103cff821dabfb04a4065f77b779ab7740ee9ef68bf6628bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69547743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eddce9da46d7c9304a8b60a2eea1e90ec1647b65c857487a9d68b7bb1635d413`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:40:01 GMT
ADD file:1461fa0362c70b5b7a677c57dd48633827fd9635a9cb136730aa7581cc523b46 in / 
# Tue, 12 Oct 2021 01:40:02 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:37:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:38:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f4b233498baa64e956a5f70979351e206bd085bd547a3cf25c08b154348df726`  
		Last Modified: Tue, 12 Oct 2021 01:48:07 GMT  
		Size: 51.2 MB (51207606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece122ff48522de249e81ee22f617bf84d59b003d3c79f44331163046a937e4c`  
		Last Modified: Tue, 12 Oct 2021 04:49:37 GMT  
		Size: 8.0 MB (8000221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:378307f52e8eeddb964324804377cd9fd65b1bf7b848c5b690e63ef92f1fe3d5`  
		Last Modified: Tue, 12 Oct 2021 04:49:37 GMT  
		Size: 10.3 MB (10339916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:7c61cd32ed32b3b639ddb2468350c4b45a105bc0f5c2e23daa4aa97ded77e997
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66349645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9969b21b9718be805e11858a4a3a51a6bfb015e4b3d34d1c36cd3b7571ec5119`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:10:39 GMT
ADD file:4769a173ec92e69a1b5cd79af0ed018bf150d1ee278de07f4bdab45f55f3c818 in / 
# Wed, 17 Nov 2021 02:10:40 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:34:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:34:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8c028c43f55209ca75650433b923c8952e16d106529242daad16c3be3efd66a3`  
		Last Modified: Wed, 17 Nov 2021 02:19:53 GMT  
		Size: 49.1 MB (49079535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:762a68d988b283d25c4ea122ea03a45caa2b4174b9d1df992298cef4bc15678f`  
		Last Modified: Wed, 17 Nov 2021 08:48:59 GMT  
		Size: 7.3 MB (7253673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a792c079b6714bc5d104fd824622583cd79ee86bf0cd4bd3930290e5bea3a81`  
		Last Modified: Wed, 17 Nov 2021 08:48:59 GMT  
		Size: 10.0 MB (10016437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:93ced9b6d18e78790cbd7fda169627b5233452d7cc6896e6d819d3fb0662f4c4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73184463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:804b950ad439852a9015c271a4046743a5293839cf6d652ded639eceefbc214c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 03:29:10 GMT
ADD file:fc0d43ba74311deef20b2131cca3a8e86b083624d63560251191adca21417f2f in / 
# Wed, 17 Nov 2021 03:29:20 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 07:52:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 07:53:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:aad6e1fe6f7c56b0e1b5850f40e4fec91ffaed4b6235e730f5c7ff43db397d3d`  
		Last Modified: Wed, 17 Nov 2021 03:56:39 GMT  
		Size: 54.2 MB (54183702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38c773e3945e9939b7299519ac8a7f3ad909af69c2d7291d8dfb6e7fa6eccfe`  
		Last Modified: Wed, 17 Nov 2021 08:28:50 GMT  
		Size: 8.3 MB (8272985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65e0d54cc06e26d154b6f6e9746c8de2af93d9f635c280336663372f382fcd46`  
		Last Modified: Wed, 17 Nov 2021 08:28:49 GMT  
		Size: 10.7 MB (10727776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:2f148905d6fe03767f7cb6e8c4fcbd6b5a200f0a6b8a9907394dc5154a203300
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66289868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65862f040a1b0973ae86d1e0f56a13ec80e7c12e566a3f87dab7af1ec5238448`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:40 GMT
ADD file:dc4ee96f81059accdc88a686f80f1714bc9d2f383af71c0d130c08560cea115e in / 
# Wed, 17 Nov 2021 02:42:42 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:10:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:10:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c12eae84d2674466d924a139a276e361afa9f63de21cf77eae19bd94eaac2629`  
		Last Modified: Wed, 17 Nov 2021 02:48:42 GMT  
		Size: 49.0 MB (49005439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564a8b4bf4cf08933f04084cd556e9c716474b9801854ea7c4473c9804894516`  
		Last Modified: Wed, 17 Nov 2021 03:18:14 GMT  
		Size: 7.4 MB (7401273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ffdc4b0bb501f5f5214892baa1a5d53d44ce92b645995a43fe2cfeb2ffec6d1`  
		Last Modified: Wed, 17 Nov 2021 03:18:14 GMT  
		Size: 9.9 MB (9883156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldstable-scm`

```console
$ docker pull buildpack-deps@sha256:b50bfcdde34728e1f8ba9ac0c1d1fcd44c4959a97b1577ae54a856fc2295f917
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
$ docker pull buildpack-deps@sha256:b024630c704ae32d7b5d99d3665a0a8e2d56001e59cfa84c36e9e2228c358dbe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120108542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c6e8b3f9456db8dd890d42a41fcb77c190b0d283f8ca01f471e275d1c209d6b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:51 GMT
ADD file:cb5ed7070880d4c0177fbe6dd278adb7926e38cd73e6abd582fd8d67e4bbf06c in / 
# Wed, 17 Nov 2021 02:20:51 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:15:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:15:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:16:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1230f17f526cb07307d41462355b10488b994e8bdafe0d8f275a405fa3b33831`  
		Last Modified: Wed, 17 Nov 2021 02:26:06 GMT  
		Size: 50.4 MB (50437098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17d0de332ca1b34d53ca41c2b39ea52ce72f8c1e81c5200e27a8bade3e6ecbb`  
		Last Modified: Wed, 17 Nov 2021 03:24:34 GMT  
		Size: 7.8 MB (7833787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7474d56348f5333567750c1e5f06f899477fd437330627341eafa71bfa1a36ab`  
		Last Modified: Wed, 17 Nov 2021 03:24:34 GMT  
		Size: 10.0 MB (9997183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211c565de40518c5dac4498ccebbf3833fcfaa5db17d4bf94e6bef466136278b`  
		Last Modified: Wed, 17 Nov 2021 03:24:55 GMT  
		Size: 51.8 MB (51840474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:80937d7a95e48544fa440d8ff13fc0b9d30ec833fad447077c9e608976313fe0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114793581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ba5c3d966befcbb226c6a48c41f0915d5314c95ec5b05b6da617cbe79855c80`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 00:50:58 GMT
ADD file:f9432d6da0faddeaa117c57c0c007cd56738ef01549baf71e5c59939b7e69b6c in / 
# Tue, 12 Oct 2021 00:50:59 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:45:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:45:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 05:46:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ae00de77d9c27fe3ba9ea06833b273e4fc0aa128a3a61d3992632e6e3941a78c`  
		Last Modified: Tue, 12 Oct 2021 01:07:01 GMT  
		Size: 48.2 MB (48154085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52282bf2103fc337ab7cc23ebfae979096e6f901b62960b03952c2d52e9978db`  
		Last Modified: Tue, 12 Oct 2021 06:04:31 GMT  
		Size: 7.4 MB (7377193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b1aa5c1e770fff74bdcd066b443f1e1e49f677ae77ec80d22c50e20be8c3b3`  
		Last Modified: Tue, 12 Oct 2021 06:04:32 GMT  
		Size: 9.7 MB (9687494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b03f47e60dacc119379be5c6a6d690ee9ebe00c3a3f7755e295b572e9d4817aa`  
		Last Modified: Tue, 12 Oct 2021 06:05:19 GMT  
		Size: 49.6 MB (49574809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:38e7ee8c93b1073e32b5e8444018fdf2fed12d6f0e0162718b120b70f00725bf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109743617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c99199676eacaf17a961d89b17bcf60f3ba4bcaa4bad06ab06550ed01003e885`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:00:12 GMT
ADD file:d71807613acdf86685f6d640a90e27b7b63cfe0f13d88668ee943aca089d8876 in / 
# Wed, 17 Nov 2021 02:00:13 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:45:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:45:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 02:46:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10acd81022d17f452439d0385615fa066b8f0ddcf3c1a803872eec5bdc6acf64`  
		Last Modified: Wed, 17 Nov 2021 02:16:00 GMT  
		Size: 45.9 MB (45918099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a9604eb6c465f658d6422593d504030155029fe0c4302451d4369030c29144`  
		Last Modified: Wed, 17 Nov 2021 03:07:14 GMT  
		Size: 7.1 MB (7125194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b043b954c4f0757e89df96897cea2cf1f93c6275466008e4ba7a4b1089c7dd3d`  
		Last Modified: Wed, 17 Nov 2021 03:07:15 GMT  
		Size: 9.3 MB (9343839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf41461745fd89900c4b7cc794c93de081420bd83223b46e1495ff96748685c`  
		Last Modified: Wed, 17 Nov 2021 03:07:59 GMT  
		Size: 47.4 MB (47356485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ae9e47c84e1cb304d5585a7cabe72277e995c683344e652437eae69be73404f4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.9 MB (118851231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16caaa63c991b5d1a70fd8dfded47c4d0a820cc1ec1de6dd0877379c7d244150`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:27 GMT
ADD file:c7e9e884b1494f96e33e9d9a892b51367af8943edb282c4101cc99ea78a7753f in / 
# Wed, 17 Nov 2021 02:40:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:28:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:28:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:28:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:626979e62c56e192812e818d52b82f063d9f9514b1b7bae14e534e4a7c98117a`  
		Last Modified: Wed, 17 Nov 2021 02:47:40 GMT  
		Size: 49.2 MB (49222990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134a528370d5dcbf5b6ba2d8c20f576504448e8f2d1debb5d2a4950a38a3ff2d`  
		Last Modified: Wed, 17 Nov 2021 13:37:44 GMT  
		Size: 7.7 MB (7695161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e12e3364b52ad043d8e79f750863ed4ca2878c4fdf45ded974508febc55fdd`  
		Last Modified: Wed, 17 Nov 2021 13:37:44 GMT  
		Size: 9.8 MB (9767133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a7f2500f9574b0a495bfb031c2d52e83c96dd545ef2185737f8032567e70677`  
		Last Modified: Wed, 17 Nov 2021 13:38:03 GMT  
		Size: 52.2 MB (52165947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:0d0d9bd21ec4cf4c15da749cd2dace32bc7a91f60d2e70dea7636c686c0c197f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (122985544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b468e2beeabc6c15ba9fdf021ec223e3ba84fc3ea63cceb1a4d97d4c4553232a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:40:01 GMT
ADD file:1461fa0362c70b5b7a677c57dd48633827fd9635a9cb136730aa7581cc523b46 in / 
# Tue, 12 Oct 2021 01:40:02 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:37:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:38:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 04:38:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f4b233498baa64e956a5f70979351e206bd085bd547a3cf25c08b154348df726`  
		Last Modified: Tue, 12 Oct 2021 01:48:07 GMT  
		Size: 51.2 MB (51207606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece122ff48522de249e81ee22f617bf84d59b003d3c79f44331163046a937e4c`  
		Last Modified: Tue, 12 Oct 2021 04:49:37 GMT  
		Size: 8.0 MB (8000221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:378307f52e8eeddb964324804377cd9fd65b1bf7b848c5b690e63ef92f1fe3d5`  
		Last Modified: Tue, 12 Oct 2021 04:49:37 GMT  
		Size: 10.3 MB (10339916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559cdd7287c6a9a0f142216d3645f886b4a777073daae85c51de968330bb9f9d`  
		Last Modified: Tue, 12 Oct 2021 04:50:08 GMT  
		Size: 53.4 MB (53437801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:2bce12967fadf2de5d6317e7098ce12b55856bf06a7037fb2fd24422a4e81e88
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.2 MB (117194587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c9da7943e7aefd994faf5843414c15b9bec44d6c353d37797bd5a778b9cb19b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:10:39 GMT
ADD file:4769a173ec92e69a1b5cd79af0ed018bf150d1ee278de07f4bdab45f55f3c818 in / 
# Wed, 17 Nov 2021 02:10:40 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:34:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:34:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 08:36:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8c028c43f55209ca75650433b923c8952e16d106529242daad16c3be3efd66a3`  
		Last Modified: Wed, 17 Nov 2021 02:19:53 GMT  
		Size: 49.1 MB (49079535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:762a68d988b283d25c4ea122ea03a45caa2b4174b9d1df992298cef4bc15678f`  
		Last Modified: Wed, 17 Nov 2021 08:48:59 GMT  
		Size: 7.3 MB (7253673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a792c079b6714bc5d104fd824622583cd79ee86bf0cd4bd3930290e5bea3a81`  
		Last Modified: Wed, 17 Nov 2021 08:48:59 GMT  
		Size: 10.0 MB (10016437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0c1cd6c6ead61c438a2c08e4c9cc9d3c5ff225d437de4052cd5b03699bdae3`  
		Last Modified: Wed, 17 Nov 2021 08:49:46 GMT  
		Size: 50.8 MB (50844942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:369458b8d3ff683d522860c70940db01c7723d2d956ad0ec28cd3401b6db7c0c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.6 MB (130641848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60323d251a71f8deeea46542dac34070eb1f8f93ba89d8953ee518ea2ef6f9ae`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 03:29:10 GMT
ADD file:fc0d43ba74311deef20b2131cca3a8e86b083624d63560251191adca21417f2f in / 
# Wed, 17 Nov 2021 03:29:20 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 07:52:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 07:53:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 07:55:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:aad6e1fe6f7c56b0e1b5850f40e4fec91ffaed4b6235e730f5c7ff43db397d3d`  
		Last Modified: Wed, 17 Nov 2021 03:56:39 GMT  
		Size: 54.2 MB (54183702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38c773e3945e9939b7299519ac8a7f3ad909af69c2d7291d8dfb6e7fa6eccfe`  
		Last Modified: Wed, 17 Nov 2021 08:28:50 GMT  
		Size: 8.3 MB (8272985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65e0d54cc06e26d154b6f6e9746c8de2af93d9f635c280336663372f382fcd46`  
		Last Modified: Wed, 17 Nov 2021 08:28:49 GMT  
		Size: 10.7 MB (10727776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3239f513a520f7d81f241b123128d80a0c91d3ef8697270ffae67898934cb4f9`  
		Last Modified: Wed, 17 Nov 2021 08:29:36 GMT  
		Size: 57.5 MB (57457385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:f5e9778f889dea21e925be77a1a076e7f0c4589927b4612209c4db9b2bef5331
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117670095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fd015a72e8350a3bbb306e91dd17a1d82b36ee73f2c0b7348bda5ac13840988`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:40 GMT
ADD file:dc4ee96f81059accdc88a686f80f1714bc9d2f383af71c0d130c08560cea115e in / 
# Wed, 17 Nov 2021 02:42:42 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:10:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:10:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:10:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c12eae84d2674466d924a139a276e361afa9f63de21cf77eae19bd94eaac2629`  
		Last Modified: Wed, 17 Nov 2021 02:48:42 GMT  
		Size: 49.0 MB (49005439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564a8b4bf4cf08933f04084cd556e9c716474b9801854ea7c4473c9804894516`  
		Last Modified: Wed, 17 Nov 2021 03:18:14 GMT  
		Size: 7.4 MB (7401273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ffdc4b0bb501f5f5214892baa1a5d53d44ce92b645995a43fe2cfeb2ffec6d1`  
		Last Modified: Wed, 17 Nov 2021 03:18:14 GMT  
		Size: 9.9 MB (9883156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb48942b4b14ee80905b23bc6babae28a961847a914becfe41686d368d8693d`  
		Last Modified: Wed, 17 Nov 2021 03:18:28 GMT  
		Size: 51.4 MB (51380227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:scm`

```console
$ docker pull buildpack-deps@sha256:993f6b93af203b5057bca0bf5858d22798c837de81f63c65326cf4bd25734d20
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
$ docker pull buildpack-deps@sha256:705b87b1c31cbc5283ea312fb0af16deeda2d00a9121f33d1779813dff4dd55b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.5 MB (125524291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e81de6f42b69f2697b8b01a08799441414abcedf96ec293b306eddb6d0d6c8ba`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:ab1b571f15dc9620590ae51b9e2a70cfb75b6438013b7a3599f47e39f6c7d600
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.4 MB (120409907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e962133851ffbc9d390eb7b46532392de0c1e19443d48ed2c7a52c4ca877cc2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 00:49:54 GMT
ADD file:b9969604315238de271e1769a4b8dd85cdf0d33f9fac387e940d5195ac3030a1 in / 
# Tue, 12 Oct 2021 00:49:55 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:40:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:41:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 05:42:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a97c782f2538791984ce12c859cada96e395e3950d4cb7d1238e08acd2eb74ec`  
		Last Modified: Tue, 12 Oct 2021 01:05:12 GMT  
		Size: 52.5 MB (52452198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34dc529b005dbeff70906cd4baf2310c918ae6379fdf53ef632c3cd1203aa38`  
		Last Modified: Tue, 12 Oct 2021 06:01:18 GMT  
		Size: 5.1 MB (5063794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2876b7f933f68a5b4f35f854cc8c651bf3d21476fe2bb0a786e6376f389b44b`  
		Last Modified: Tue, 12 Oct 2021 06:01:20 GMT  
		Size: 10.6 MB (10571017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c918a5faa65bffd689b9869a942e77a3fbc7d89566be880da188d6050f4f627`  
		Last Modified: Tue, 12 Oct 2021 06:02:11 GMT  
		Size: 52.3 MB (52322898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:19565c156eedbb4210675b27d3f633814a7f585b53d58729e1fe465da7904001
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.6 MB (115601563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31f5dfdc32269a08b775b7b18972781651a1103e34bb2eb596fda4bcd843f1af`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 01:59:07 GMT
ADD file:43b45f65ff4ba720f6f9a107b5f80818d5ea6ebc4835840b11e9a506351da32f in / 
# Wed, 17 Nov 2021 01:59:08 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:41:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:42:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 02:43:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dbbf55137aab3c7acd1e012a70f1ea1adeaef8d39b474829965d3480a02bf572`  
		Last Modified: Wed, 17 Nov 2021 02:14:27 GMT  
		Size: 50.1 MB (50134152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb1ae7a04cee77523f9e09a62b28632c56a700d0c481be7cddc566c835e7a71d`  
		Last Modified: Wed, 17 Nov 2021 03:04:13 GMT  
		Size: 4.9 MB (4922782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66894dfea839186e94448f6c25a37c6b3b1b42cece6332cc9d36336917e18a4`  
		Last Modified: Wed, 17 Nov 2021 03:04:14 GMT  
		Size: 10.2 MB (10216965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4502933ba6aa2071501257e094faa363699dc23995f798a124d688c2523240af`  
		Last Modified: Wed, 17 Nov 2021 03:05:05 GMT  
		Size: 50.3 MB (50327664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d98321260829308a2348a158000abedf1fcd03e58d44ac414c3d077d1c110c70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.9 MB (123882237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32fa5708561ca81a99850197b076caf6f432ccb91bee5a5df1a4e6a478d3ec3f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:59 GMT
ADD file:eb667e18226da8a1ca5a41beacddc65cd1efec01c3d01e50845c5e89e91ea17c in / 
# Wed, 17 Nov 2021 02:40:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:26:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:26:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:27:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce18cd0ba11c2dfa8c1a2d2b325e1e019b14d4ae25ffdeffb0f9686c5496bf5c`  
		Last Modified: Wed, 17 Nov 2021 02:46:45 GMT  
		Size: 53.6 MB (53619024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f138a340a2373acc72dcc4ea9ef08bdf5648aabc5fe08f7e8d25222ca63b7ee`  
		Last Modified: Wed, 17 Nov 2021 13:36:26 GMT  
		Size: 4.9 MB (4937639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34c030205ccb8656e30a58f96bb1edbe7c59bf17f3329ae3c442ec897f2b270`  
		Last Modified: Wed, 17 Nov 2021 13:36:27 GMT  
		Size: 10.7 MB (10655878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7a1cfcc2070fbe1e702751d85f7074b93d142f6beb03ef66e9ba1c58bcc3e3`  
		Last Modified: Wed, 17 Nov 2021 13:36:49 GMT  
		Size: 54.7 MB (54669696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:16abe77eeca3b6e96cff6cf2bbff639647cf581d03efc6c7dcb8ab3fb5fa8bd2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128374671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:363c0a8d58ad2bab650032b97601a821766dc54ba78827525e9e45381d993d08`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:39:30 GMT
ADD file:e007d6eff02dbc696e1166db315b97a77ae8aa65f2e66ca8074765dde9c70a59 in / 
# Tue, 12 Oct 2021 01:39:31 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:35:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:36:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 04:36:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6911c8f66691266d86e2cafa67ca005d919f357436fac971c694d37625b5ba90`  
		Last Modified: Tue, 12 Oct 2021 01:47:06 GMT  
		Size: 55.9 MB (55923419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a0f31369a20c178b1d5c84f192412ed962068e8932d5821eefb00bc7d1cbc1a`  
		Last Modified: Tue, 12 Oct 2021 04:47:26 GMT  
		Size: 5.3 MB (5283102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97aa3d222d7e8d6e0b06e57e5bd03168c422475942f92d09a487bd98d09bb742`  
		Last Modified: Tue, 12 Oct 2021 04:47:27 GMT  
		Size: 11.3 MB (11250699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae99d06bab5fc31ba3db9436a22c452db74a7b5e559a451de2d971a493abe52`  
		Last Modified: Tue, 12 Oct 2021 04:48:03 GMT  
		Size: 55.9 MB (55917451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:a5be5277770524bd35dd921bc7f03adf64d8bf76eeee88ba1a6fb10f62aa65a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.5 MB (122468694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afe05d4524b16661e35a811e3b2f3a1ea3e0fc1ca56eb4306839c755f24c34ef`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:09:46 GMT
ADD file:2971df49f24648b8d5166d87e392e2547d5b03469356f20d112ce6feb3c329fc in / 
# Wed, 17 Nov 2021 02:09:47 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:29:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:30:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 08:31:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b095a0b63d99a4c4cd9c1c353f381a69ef041e6f80798d807ae51a34b04920a0`  
		Last Modified: Wed, 17 Nov 2021 02:18:22 GMT  
		Size: 53.2 MB (53183806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2e37aff1692726b1ea3dd0b4eeb684072527295f8e981d3c45825327daea19`  
		Last Modified: Wed, 17 Nov 2021 08:45:38 GMT  
		Size: 5.1 MB (5114925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d4c0302ddd7a6cb573a156076dba9c593e09a0c321b32ae0f1da2bd36bc754`  
		Last Modified: Wed, 17 Nov 2021 08:45:41 GMT  
		Size: 10.9 MB (10873360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cde5eca075420fcfc6498f454dc040f1e236dea180a82a0d27d7a739ffd41c1`  
		Last Modified: Wed, 17 Nov 2021 08:46:32 GMT  
		Size: 53.3 MB (53296603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:faf4c1b1a0373960c09ef3f862d4fcd8e9c6bc9b842a86cdf1ab3405f45a9f3c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134698979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b960badc27a250634b2e76a6871d276d149dcd0fe0fe615bbf2f54db9efc221b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 03:27:04 GMT
ADD file:85375acb19da58f9eabaa67f8cb425cd1ff2dadb2888bbd9dbfa6223d16fef23 in / 
# Wed, 17 Nov 2021 03:27:20 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 07:40:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 07:40:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 07:42:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ede9cd7c8f1d380c971a130fb3d8a3914bf3a9106702164c23b2cce536fa618c`  
		Last Modified: Wed, 17 Nov 2021 03:52:39 GMT  
		Size: 58.8 MB (58819505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743814bfd79326104da0238d8edced6b14f63b95734b6dc0e2b7a9d83356b0cb`  
		Last Modified: Wed, 17 Nov 2021 08:25:58 GMT  
		Size: 5.4 MB (5402000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca978d94a6543bbd1c60026602b64e810b4bf65e052dcf19adf2b4d6b518bf8`  
		Last Modified: Wed, 17 Nov 2021 08:25:59 GMT  
		Size: 11.6 MB (11626016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d785f1d8909cb3a3e46844611c28e15781da809be0073e40af017d6e5631d0`  
		Last Modified: Wed, 17 Nov 2021 08:26:57 GMT  
		Size: 58.9 MB (58851458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:673b0a54f0e03e540c534b0dfc3525d90049ec556ed645e24d83e7eaa1dd159f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123147032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ec10947074405be072d3cee591cea9230aa7dd19dafc623039d1644d6083ca4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:07 GMT
ADD file:b7524e775a2033d246d1096765a0eb6eaa5ba6ed6c8b395522579d2c4e7a2e38 in / 
# Wed, 17 Nov 2021 02:42:09 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:07:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:07:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:08:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ffa47acd07831fbc96680a705da20704bac0016c20dc3c454ecd45cda44b368d`  
		Last Modified: Wed, 17 Nov 2021 02:48:05 GMT  
		Size: 53.2 MB (53207179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c950336719691da019c99e4ff78fe559ab0308ea145757994bdb7be34c6d224`  
		Last Modified: Wed, 17 Nov 2021 03:17:18 GMT  
		Size: 5.1 MB (5137199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d769af2ca44d1c7c206e7190cd71df7cb5ff3df2dd45e1dd52ea447ffb547b1a`  
		Last Modified: Wed, 17 Nov 2021 03:17:19 GMT  
		Size: 10.8 MB (10761499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3bbc68017b41a8cc07b10d715e2a23108c5addefa80b01cac1a2ef075bb1acd`  
		Last Modified: Wed, 17 Nov 2021 03:17:36 GMT  
		Size: 54.0 MB (54041155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:sid`

```console
$ docker pull buildpack-deps@sha256:b11103e6002f002f86e02cb10b9cef8b4a2cf90715e61d7cf395454bb089662e
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
$ docker pull buildpack-deps@sha256:de2c4024f4b15d8d4c980231c950776d5a75d15255ac95ebf4d7fc164fd26cc5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **492.2 MB (492225831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54138805f9191923bd18fae65421f211dad9ebf7d18c4e55fc9f640874f0b585`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:21:50 GMT
ADD file:1f62518cec36eb3320e38344c0d36779557214cfce8bc32eda000183a34a0ffa in / 
# Wed, 17 Nov 2021 02:21:51 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:17:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:17:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:18:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fef5443775fe054990b02e8f72c4c5bc7792c6a5bf6ef8df110873a81676a87`  
		Last Modified: Wed, 17 Nov 2021 02:28:03 GMT  
		Size: 55.8 MB (55758091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b63aa91be04004e56a4d31d70c789eadabfebe392e2f76a862eaa2fdd70dcfd`  
		Last Modified: Wed, 17 Nov 2021 03:25:48 GMT  
		Size: 5.3 MB (5269763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f625d605a0450d800b57ca6e2e0662fba5094348ccbf581c053a485802ebe1`  
		Last Modified: Wed, 17 Nov 2021 03:25:49 GMT  
		Size: 11.8 MB (11756478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f0dd71d7f2f690f062de61d743dd487108ccd38089c95218a295206a6c68c3`  
		Last Modified: Wed, 17 Nov 2021 03:26:09 GMT  
		Size: 55.9 MB (55936130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3929219b522d034efb90c4bdfcc3dc832476eea68565e8fdd758c5302b0766c2`  
		Last Modified: Wed, 17 Nov 2021 03:27:15 GMT  
		Size: 363.5 MB (363505369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:215a46aa6f638cf9e220fab73f63e86e8bfab8c61cfd70685dbda87356f34fa8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **474.9 MB (474871327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd2a73342dfad8a3515950c7aab1d759d8165ed5f42f656523b75f8e7b6ef43a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 00:53:53 GMT
ADD file:2918872df07d47b9a7862abf3b22f39600ab45587fcd02466bdefa775a3fc2dd in / 
# Tue, 12 Oct 2021 00:53:54 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:49:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:49:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 05:50:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:53:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8f73c109c91bd2f18faab4d6862ba33d940956d6457aaaaeeda5e8f72281edcc`  
		Last Modified: Tue, 12 Oct 2021 01:11:00 GMT  
		Size: 53.2 MB (53186352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd99c7b364b1329f3fc27bcb8d50810c30d8a7928b7518c93f2d538a1124daa0`  
		Last Modified: Tue, 12 Oct 2021 06:07:28 GMT  
		Size: 5.1 MB (5122384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8779df359e844ab400aaeab5d2001cf6d805ff10af17660fd4577296ecbf7f9`  
		Last Modified: Tue, 12 Oct 2021 06:07:30 GMT  
		Size: 10.6 MB (10606788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83014d4ab58f54e38e974b2de48f1a41a6bee268a7b6ebb1050582b1d782db1b`  
		Last Modified: Tue, 12 Oct 2021 06:08:20 GMT  
		Size: 53.4 MB (53442505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af54fd52817c8dff8e7fb1fb4b62845da3ed7da902c46ad93c9210945460647`  
		Last Modified: Tue, 12 Oct 2021 06:11:57 GMT  
		Size: 352.5 MB (352513298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:0e27ca88aaec10d98a1a69d635898d0de8d28f06ef64c3e111940e973d556ea0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **447.4 MB (447442275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2068124a06286aeecf9bb8a71ec407a13f888636b5b5030a394286b666e0f17d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:03:10 GMT
ADD file:df29fec66c741f67158d8ed2094810758d4a7cfb2c7cba3dbe60e5bc11ed824a in / 
# Wed, 17 Nov 2021 02:03:11 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:49:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:49:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 02:50:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:53:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:339de498e0e3324e5657ae3bd0868b26e4518664b7405a1fb321434233c56211`  
		Last Modified: Wed, 17 Nov 2021 02:19:45 GMT  
		Size: 50.9 MB (50860308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b9096006210de2acfc2854bd14870e0046c7c41610d75f402e14c7fa186a10`  
		Last Modified: Wed, 17 Nov 2021 03:10:01 GMT  
		Size: 5.0 MB (5029921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8864516b2a87655fdd355f203892d84f29fb0f553f371f37e7027ceb5017ec34`  
		Last Modified: Wed, 17 Nov 2021 03:10:03 GMT  
		Size: 11.1 MB (11067071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e207fc56e058029a1aa1e0cae4ac127bfa621c4e822edde8fdad43037978ac`  
		Last Modified: Wed, 17 Nov 2021 03:10:51 GMT  
		Size: 51.6 MB (51586431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31acdea0339066b9fdb9e8d5b74ff20f7ec64f9c62a7bf2ae54f21f2d6f1dcdb`  
		Last Modified: Wed, 17 Nov 2021 03:14:06 GMT  
		Size: 328.9 MB (328898544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c5e577cbb626d2867b19ce7ce967421f0665abf3c9cdb76e1574bff2ae26e9f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.7 MB (484718199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cb63aed3f12bbd933a07cf611eb991b7dec3ec3d9008ec829ec5ec30aa40b74`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:41:46 GMT
ADD file:6547698ce9c0dce5d390e739342bd015a0c3266dba4ef5828dc1b1a9eb46e826 in / 
# Wed, 17 Nov 2021 02:41:47 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:29:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:29:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:30:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:31:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:67eeb578521bba47ceed6d5c2de23409a33ec3c1c6fda03d83e22d74dc1cdb76`  
		Last Modified: Wed, 17 Nov 2021 02:49:53 GMT  
		Size: 54.8 MB (54767045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f777f34bfc0463ddee51fc9ba3a1f668f6072f8431123ab0571266c60fb89c`  
		Last Modified: Wed, 17 Nov 2021 13:38:51 GMT  
		Size: 5.3 MB (5253448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e720a8fffb7aadf0b926dc4c5b3d7cb21c21c6ec5e507ddcdb546f5483b5a44e`  
		Last Modified: Wed, 17 Nov 2021 13:38:52 GMT  
		Size: 11.5 MB (11525452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cab4dc0eb95cf2e9a2e2a5f77eca7d76108730f09e1e205c09465b4fa35934`  
		Last Modified: Wed, 17 Nov 2021 13:39:12 GMT  
		Size: 56.0 MB (55987448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c004de456b5e733bd6cf254df397e043de9b362c370460e313ed02fe89d4de81`  
		Last Modified: Wed, 17 Nov 2021 13:40:11 GMT  
		Size: 357.2 MB (357184806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; 386

```console
$ docker pull buildpack-deps@sha256:4ea2edd31669732d12dce321d6928127ffbe9073c24d96085b9ca44c2933bfab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.4 MB (332367435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea23a81b9c83e610134b648dd92aba29502de7ae1aa419876e7ab76976e253a2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:27 GMT
ADD file:9ab0c16547aac0a32292246b35737ca5260c5942d5e26ca1381be39c9e321ee5 in / 
# Tue, 12 Oct 2021 01:41:27 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:40:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:40:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 04:40:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:42:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c36fe1aa4217cf0326227a0bdcadc16e85d2670bd6485518167903dfc6934c65`  
		Last Modified: Tue, 12 Oct 2021 01:50:33 GMT  
		Size: 56.7 MB (56716103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1cefa3abf3c8d9687bfe164fbd73be6245f1e0c523603077cfcffd5881a3778`  
		Last Modified: Tue, 12 Oct 2021 04:51:12 GMT  
		Size: 5.3 MB (5346244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902f94685b9ef6228bbe2d7c552fb6d02ea5e723469df5c9e980d102fd9c6aa2`  
		Last Modified: Tue, 12 Oct 2021 04:51:13 GMT  
		Size: 11.3 MB (11281973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802e1fd067f1198f877ff5bc97afd5870c21a28609a1919a09063ff8aacf5fd4`  
		Last Modified: Tue, 12 Oct 2021 04:51:37 GMT  
		Size: 57.2 MB (57159249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ecb28b33acfca8e5784c5c3b85c0efb3eeb8d08971fe4e1e1dee2cc768ee8d`  
		Last Modified: Tue, 12 Oct 2021 04:52:26 GMT  
		Size: 201.9 MB (201863866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:d85ae18394cee324adf13254d7ec82ba0f2b66e532a1b07e1bf9ce1bade8da76
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **549.8 MB (549780160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a665b5eab25ab4ed0aaf7891e0b735ee8cabe629675356cb418ecd9a7771755c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:12:23 GMT
ADD file:9e3985f5064204cf4c74f2d464977349398f8e0325083d223b22ace99f5dfa3a in / 
# Wed, 17 Nov 2021 02:12:24 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:39:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:39:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 08:41:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:45:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b79f1dde26df3dbfdaf094cc43f4dc602b492e9dd707f7a7874e1366808028c5`  
		Last Modified: Wed, 17 Nov 2021 02:22:36 GMT  
		Size: 54.4 MB (54365459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c0e1963482abb9ea5592b86c11c6528aebf6fe675fd25fdeb440cd4f999043`  
		Last Modified: Wed, 17 Nov 2021 08:52:05 GMT  
		Size: 5.2 MB (5227764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0761e303fe4f33cd92c7d2d5ce49857285721fb135e5bf569abf4ec59745f3d`  
		Last Modified: Wed, 17 Nov 2021 08:52:07 GMT  
		Size: 11.8 MB (11755031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c476b323dda6fd93fbb86e98139e76c07bff3f2d7a4b07b087d8e2c114b346f2`  
		Last Modified: Wed, 17 Nov 2021 08:52:57 GMT  
		Size: 54.7 MB (54724326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea5b4a56a5596c25bbe127b531db840714709450c79dc686fb6cadb3ca56d6b`  
		Last Modified: Wed, 17 Nov 2021 08:57:22 GMT  
		Size: 423.7 MB (423707580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:a36f7bd93877cf70c960b650bc009777ba9a4e1a8a4c54e2a062ea7543d6e6e3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **490.1 MB (490107816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c48763889dcaa835be669cbc061b277dce92e01b77549cf143c08d77b60c8d15`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 03:32:54 GMT
ADD file:33bc17dd3e3b6cd8c5ac37c8382a5d2b8e3ee8384b598b69b0d17b813dcfc767 in / 
# Wed, 17 Nov 2021 03:33:15 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:07:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:08:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 08:11:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:23:09 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:60fa303f933c621481dd7a32f72de0e35b85a3567ff116516725c45089e1cb88`  
		Last Modified: Wed, 17 Nov 2021 04:05:01 GMT  
		Size: 60.0 MB (60045015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a3dd48191daf1a5544d8a3146aececcefc7d4f8fe8e7e64e723022de0e5bae`  
		Last Modified: Wed, 17 Nov 2021 08:31:39 GMT  
		Size: 5.5 MB (5531621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147c14b8f9e107cd759a99e83c419ee5c8c99e500d16d4bbbfdb94cf6126b724`  
		Last Modified: Wed, 17 Nov 2021 08:31:39 GMT  
		Size: 12.6 MB (12551297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16114ff6b100453ae456bca4961ed144a5cd72589c05128a5b44f063feab7bb`  
		Last Modified: Wed, 17 Nov 2021 08:32:21 GMT  
		Size: 60.4 MB (60400057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e03566f3ff76ccaf4843d621b4de9ff1a4ee9e74293314b7c986934b6be759d`  
		Last Modified: Wed, 17 Nov 2021 08:33:58 GMT  
		Size: 351.6 MB (351579826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:7ab7d4a74146b5374310fdaf408c2b278bcc7b29f972af025baebb48315f3c0b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343151630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70b618750b60d86f44a77d1d23690393cf206bada324151d86c6a22e64af1c7c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:14:24 GMT
ADD file:9ce8adafd95fc1e31db924edf473abf22a68101cad20cd078c35db5fa719b34b in / 
# Wed, 17 Nov 2021 02:14:27 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:56:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:58:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:02:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:11:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a35675c997377ee8bf94b0a94460a6d2fd72a26b5c7fc6194b13ae99da869125`  
		Last Modified: Wed, 17 Nov 2021 02:30:42 GMT  
		Size: 51.5 MB (51522304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6561ec3264f30875424c0937b41795ce70f58306ddfe766af2fcb7d266b6a6`  
		Last Modified: Wed, 17 Nov 2021 03:35:29 GMT  
		Size: 5.1 MB (5080232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f12be064689662dab642f65c8e821186c7247cf7ea84901a22b9e2584d51ee`  
		Last Modified: Wed, 17 Nov 2021 03:35:32 GMT  
		Size: 11.1 MB (11140508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077cd6f4305eeccad12d3a65baeff88b63dd35ab2735a8b6ca9d8f523e0b6a0a`  
		Last Modified: Wed, 17 Nov 2021 03:37:41 GMT  
		Size: 52.0 MB (52047230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3022710ce0174de31ed5f93fad3d58e7093927e84afdebfe2ee1e4a0bf48a54`  
		Last Modified: Wed, 17 Nov 2021 03:43:51 GMT  
		Size: 223.4 MB (223361356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:01443347d94c5d12c4c092d73f4e8954a0534604ba46a76e51e266d41e1adee0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **445.9 MB (445921270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef208aa2298803038eb573bf20ffc382beb5cb388e6ce838fd0cb92765f14a07`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:43:42 GMT
ADD file:ba3a56dbd46c1324142a33ad1eefa66c34fda8c9c635140debf01131cb259e63 in / 
# Wed, 17 Nov 2021 02:43:45 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:11:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:12:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:12:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:13:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3595b50e30d7d0d412c142596638dbf5abfc27f196fe5d138ded04b66fd2b50e`  
		Last Modified: Wed, 17 Nov 2021 02:49:48 GMT  
		Size: 54.0 MB (53965664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634664d8b893813a04761069646d85aea7164717481b8c7e3f500e4260fc39ee`  
		Last Modified: Wed, 17 Nov 2021 03:19:03 GMT  
		Size: 5.2 MB (5248300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1780c6b7bcc6484f6ae6602c37ffd3bb2c9aad27b1b2587b796a5824e8b6575`  
		Last Modified: Wed, 17 Nov 2021 03:19:03 GMT  
		Size: 11.6 MB (11647079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a6bd04c7a7df4cb7de2e064bcfa156db3e89664ab5448cf33cf12043705f4f5`  
		Last Modified: Wed, 17 Nov 2021 03:19:17 GMT  
		Size: 55.3 MB (55308755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d56ccdfeb3f75ba623e571ad85ef9c45f32b1e527abc14d9e5164dca7dbd76`  
		Last Modified: Wed, 17 Nov 2021 03:19:59 GMT  
		Size: 319.8 MB (319751472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:bfffe4a3acc134d001cdcf237d588a1e9caebafd5707bd0b9d392800a322b926
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
$ docker pull buildpack-deps@sha256:19dfc5e7628b593c8056b31cbe197a24fffbe1d35a9b17adfd2f59a34641a4d8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.8 MB (72784332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07490f1b8ba2320e2026f3266933346b545ee1a5e75319a686e3575bac5b7f55`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:21:50 GMT
ADD file:1f62518cec36eb3320e38344c0d36779557214cfce8bc32eda000183a34a0ffa in / 
# Wed, 17 Nov 2021 02:21:51 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:17:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:17:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0fef5443775fe054990b02e8f72c4c5bc7792c6a5bf6ef8df110873a81676a87`  
		Last Modified: Wed, 17 Nov 2021 02:28:03 GMT  
		Size: 55.8 MB (55758091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b63aa91be04004e56a4d31d70c789eadabfebe392e2f76a862eaa2fdd70dcfd`  
		Last Modified: Wed, 17 Nov 2021 03:25:48 GMT  
		Size: 5.3 MB (5269763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f625d605a0450d800b57ca6e2e0662fba5094348ccbf581c053a485802ebe1`  
		Last Modified: Wed, 17 Nov 2021 03:25:49 GMT  
		Size: 11.8 MB (11756478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:93a96196f940f2470a5f63e45ed1eea93d39f49454b3461ce4f86003f32e88b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68915524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0426cef40090f80992e6f69498065959d6e618dd140a8a21341a317c7ce7f274`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 00:53:53 GMT
ADD file:2918872df07d47b9a7862abf3b22f39600ab45587fcd02466bdefa775a3fc2dd in / 
# Tue, 12 Oct 2021 00:53:54 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:49:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:49:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8f73c109c91bd2f18faab4d6862ba33d940956d6457aaaaeeda5e8f72281edcc`  
		Last Modified: Tue, 12 Oct 2021 01:11:00 GMT  
		Size: 53.2 MB (53186352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd99c7b364b1329f3fc27bcb8d50810c30d8a7928b7518c93f2d538a1124daa0`  
		Last Modified: Tue, 12 Oct 2021 06:07:28 GMT  
		Size: 5.1 MB (5122384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8779df359e844ab400aaeab5d2001cf6d805ff10af17660fd4577296ecbf7f9`  
		Last Modified: Tue, 12 Oct 2021 06:07:30 GMT  
		Size: 10.6 MB (10606788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:67b214acbcd9f9a68874338a7751ff7c36fbfaf55bf4c8085992ae1d47249822
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (66957300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17a529394265f7fd2fbce68d31a42a78128feabb2a05da15f6db6613f9a9f76d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:03:10 GMT
ADD file:df29fec66c741f67158d8ed2094810758d4a7cfb2c7cba3dbe60e5bc11ed824a in / 
# Wed, 17 Nov 2021 02:03:11 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:49:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:49:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:339de498e0e3324e5657ae3bd0868b26e4518664b7405a1fb321434233c56211`  
		Last Modified: Wed, 17 Nov 2021 02:19:45 GMT  
		Size: 50.9 MB (50860308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b9096006210de2acfc2854bd14870e0046c7c41610d75f402e14c7fa186a10`  
		Last Modified: Wed, 17 Nov 2021 03:10:01 GMT  
		Size: 5.0 MB (5029921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8864516b2a87655fdd355f203892d84f29fb0f553f371f37e7027ceb5017ec34`  
		Last Modified: Wed, 17 Nov 2021 03:10:03 GMT  
		Size: 11.1 MB (11067071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:739c39731b3c78675e5b07d31cfd783cbcaa98f52bcd3e90fcd44c9a307e6676
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.5 MB (71545945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a03eacbbae2823342ae5c042212eaa4d8a7fd2b691788aca661c794de4be92dd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:41:46 GMT
ADD file:6547698ce9c0dce5d390e739342bd015a0c3266dba4ef5828dc1b1a9eb46e826 in / 
# Wed, 17 Nov 2021 02:41:47 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:29:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:29:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:67eeb578521bba47ceed6d5c2de23409a33ec3c1c6fda03d83e22d74dc1cdb76`  
		Last Modified: Wed, 17 Nov 2021 02:49:53 GMT  
		Size: 54.8 MB (54767045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f777f34bfc0463ddee51fc9ba3a1f668f6072f8431123ab0571266c60fb89c`  
		Last Modified: Wed, 17 Nov 2021 13:38:51 GMT  
		Size: 5.3 MB (5253448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e720a8fffb7aadf0b926dc4c5b3d7cb21c21c6ec5e507ddcdb546f5483b5a44e`  
		Last Modified: Wed, 17 Nov 2021 13:38:52 GMT  
		Size: 11.5 MB (11525452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:4dd56a29db23efb893ab16850832733df3813b7a11f292dee71fd5094fd58a3c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.3 MB (73344320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:962d74b000a7400b45ea570dcd0f3351f2de7987db6d7cbd3225992e396a156d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:27 GMT
ADD file:9ab0c16547aac0a32292246b35737ca5260c5942d5e26ca1381be39c9e321ee5 in / 
# Tue, 12 Oct 2021 01:41:27 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:40:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:40:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c36fe1aa4217cf0326227a0bdcadc16e85d2670bd6485518167903dfc6934c65`  
		Last Modified: Tue, 12 Oct 2021 01:50:33 GMT  
		Size: 56.7 MB (56716103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1cefa3abf3c8d9687bfe164fbd73be6245f1e0c523603077cfcffd5881a3778`  
		Last Modified: Tue, 12 Oct 2021 04:51:12 GMT  
		Size: 5.3 MB (5346244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902f94685b9ef6228bbe2d7c552fb6d02ea5e723469df5c9e980d102fd9c6aa2`  
		Last Modified: Tue, 12 Oct 2021 04:51:13 GMT  
		Size: 11.3 MB (11281973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:7cb7cefc9fa6132910698c9133093c1f9b92416218f2ee05824d1bd3c04bf7af
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71348254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c188c28686d73282c6cc150448e2c28b123c0faf48b12f0c6ba204562bd511d0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:12:23 GMT
ADD file:9e3985f5064204cf4c74f2d464977349398f8e0325083d223b22ace99f5dfa3a in / 
# Wed, 17 Nov 2021 02:12:24 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:39:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:39:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b79f1dde26df3dbfdaf094cc43f4dc602b492e9dd707f7a7874e1366808028c5`  
		Last Modified: Wed, 17 Nov 2021 02:22:36 GMT  
		Size: 54.4 MB (54365459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c0e1963482abb9ea5592b86c11c6528aebf6fe675fd25fdeb440cd4f999043`  
		Last Modified: Wed, 17 Nov 2021 08:52:05 GMT  
		Size: 5.2 MB (5227764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0761e303fe4f33cd92c7d2d5ce49857285721fb135e5bf569abf4ec59745f3d`  
		Last Modified: Wed, 17 Nov 2021 08:52:07 GMT  
		Size: 11.8 MB (11755031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:b66398bb06582e08079239ae0b55efcdaa4a6ce35f62aef40ad59f2066a751a1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.1 MB (78127933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4909eb043acba9dfc8f6ced1c81d8f31d080bf218205bcff6428112c4bbfecd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 03:32:54 GMT
ADD file:33bc17dd3e3b6cd8c5ac37c8382a5d2b8e3ee8384b598b69b0d17b813dcfc767 in / 
# Wed, 17 Nov 2021 03:33:15 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:07:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:08:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:60fa303f933c621481dd7a32f72de0e35b85a3567ff116516725c45089e1cb88`  
		Last Modified: Wed, 17 Nov 2021 04:05:01 GMT  
		Size: 60.0 MB (60045015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a3dd48191daf1a5544d8a3146aececcefc7d4f8fe8e7e64e723022de0e5bae`  
		Last Modified: Wed, 17 Nov 2021 08:31:39 GMT  
		Size: 5.5 MB (5531621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147c14b8f9e107cd759a99e83c419ee5c8c99e500d16d4bbbfdb94cf6126b724`  
		Last Modified: Wed, 17 Nov 2021 08:31:39 GMT  
		Size: 12.6 MB (12551297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:c56a5966672afb0d47c167ad7358e0979cd24aef6efa756a7d6814b137b647df
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67743044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c2ef8905089a0b83a3817c763b00709bc4c9c53504e843a8e09c10005a148e6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:14:24 GMT
ADD file:9ce8adafd95fc1e31db924edf473abf22a68101cad20cd078c35db5fa719b34b in / 
# Wed, 17 Nov 2021 02:14:27 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:56:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:58:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a35675c997377ee8bf94b0a94460a6d2fd72a26b5c7fc6194b13ae99da869125`  
		Last Modified: Wed, 17 Nov 2021 02:30:42 GMT  
		Size: 51.5 MB (51522304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6561ec3264f30875424c0937b41795ce70f58306ddfe766af2fcb7d266b6a6`  
		Last Modified: Wed, 17 Nov 2021 03:35:29 GMT  
		Size: 5.1 MB (5080232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f12be064689662dab642f65c8e821186c7247cf7ea84901a22b9e2584d51ee`  
		Last Modified: Wed, 17 Nov 2021 03:35:32 GMT  
		Size: 11.1 MB (11140508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:40088f08cf065fbc90807be108a7a28a69ba5cf9a42b702be39a8c7e51925ab5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.9 MB (70861043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab27d0591464195b772d890535dec1c22fe3a85b97d9aff1dbb6f656574b113c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:43:42 GMT
ADD file:ba3a56dbd46c1324142a33ad1eefa66c34fda8c9c635140debf01131cb259e63 in / 
# Wed, 17 Nov 2021 02:43:45 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:11:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:12:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3595b50e30d7d0d412c142596638dbf5abfc27f196fe5d138ded04b66fd2b50e`  
		Last Modified: Wed, 17 Nov 2021 02:49:48 GMT  
		Size: 54.0 MB (53965664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634664d8b893813a04761069646d85aea7164717481b8c7e3f500e4260fc39ee`  
		Last Modified: Wed, 17 Nov 2021 03:19:03 GMT  
		Size: 5.2 MB (5248300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1780c6b7bcc6484f6ae6602c37ffd3bb2c9aad27b1b2587b796a5824e8b6575`  
		Last Modified: Wed, 17 Nov 2021 03:19:03 GMT  
		Size: 11.6 MB (11647079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:sid-scm`

```console
$ docker pull buildpack-deps@sha256:df709a87f131d005c85caf81955466cc7b0448e415eddbf201b4afadb88dce0f
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
$ docker pull buildpack-deps@sha256:62c202ce5cf8cf05bcb2ba5a873e1590fb65fadeeb82a6c0909b7dc0585d74f8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128720462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c577bace026f3ec0ecea3874f32bad4f5b02436f6da5fe8a140ca47b896691f4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:21:50 GMT
ADD file:1f62518cec36eb3320e38344c0d36779557214cfce8bc32eda000183a34a0ffa in / 
# Wed, 17 Nov 2021 02:21:51 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:17:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:17:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:18:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fef5443775fe054990b02e8f72c4c5bc7792c6a5bf6ef8df110873a81676a87`  
		Last Modified: Wed, 17 Nov 2021 02:28:03 GMT  
		Size: 55.8 MB (55758091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b63aa91be04004e56a4d31d70c789eadabfebe392e2f76a862eaa2fdd70dcfd`  
		Last Modified: Wed, 17 Nov 2021 03:25:48 GMT  
		Size: 5.3 MB (5269763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f625d605a0450d800b57ca6e2e0662fba5094348ccbf581c053a485802ebe1`  
		Last Modified: Wed, 17 Nov 2021 03:25:49 GMT  
		Size: 11.8 MB (11756478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f0dd71d7f2f690f062de61d743dd487108ccd38089c95218a295206a6c68c3`  
		Last Modified: Wed, 17 Nov 2021 03:26:09 GMT  
		Size: 55.9 MB (55936130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:a6fd6b6ff59a9e3a097d8125f6ca8b78882f804f0ca5bec557784676e4d379a3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.4 MB (122358029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33b4f3e109e84ef325b2927539c9c569367e50198086ed8d72be40ef36742c34`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 00:53:53 GMT
ADD file:2918872df07d47b9a7862abf3b22f39600ab45587fcd02466bdefa775a3fc2dd in / 
# Tue, 12 Oct 2021 00:53:54 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:49:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:49:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 05:50:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8f73c109c91bd2f18faab4d6862ba33d940956d6457aaaaeeda5e8f72281edcc`  
		Last Modified: Tue, 12 Oct 2021 01:11:00 GMT  
		Size: 53.2 MB (53186352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd99c7b364b1329f3fc27bcb8d50810c30d8a7928b7518c93f2d538a1124daa0`  
		Last Modified: Tue, 12 Oct 2021 06:07:28 GMT  
		Size: 5.1 MB (5122384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8779df359e844ab400aaeab5d2001cf6d805ff10af17660fd4577296ecbf7f9`  
		Last Modified: Tue, 12 Oct 2021 06:07:30 GMT  
		Size: 10.6 MB (10606788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83014d4ab58f54e38e974b2de48f1a41a6bee268a7b6ebb1050582b1d782db1b`  
		Last Modified: Tue, 12 Oct 2021 06:08:20 GMT  
		Size: 53.4 MB (53442505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:e25517d9e4d5c71b0fd71f8672be17b1407629cf364b7b4c875a48dd1572d1d9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.5 MB (118543731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b22e7df05fd0bffeca4c0755b5570159b2a6f9ae77bca4317c40c4257b7e6e1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:03:10 GMT
ADD file:df29fec66c741f67158d8ed2094810758d4a7cfb2c7cba3dbe60e5bc11ed824a in / 
# Wed, 17 Nov 2021 02:03:11 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:49:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:49:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 02:50:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:339de498e0e3324e5657ae3bd0868b26e4518664b7405a1fb321434233c56211`  
		Last Modified: Wed, 17 Nov 2021 02:19:45 GMT  
		Size: 50.9 MB (50860308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b9096006210de2acfc2854bd14870e0046c7c41610d75f402e14c7fa186a10`  
		Last Modified: Wed, 17 Nov 2021 03:10:01 GMT  
		Size: 5.0 MB (5029921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8864516b2a87655fdd355f203892d84f29fb0f553f371f37e7027ceb5017ec34`  
		Last Modified: Wed, 17 Nov 2021 03:10:03 GMT  
		Size: 11.1 MB (11067071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e207fc56e058029a1aa1e0cae4ac127bfa621c4e822edde8fdad43037978ac`  
		Last Modified: Wed, 17 Nov 2021 03:10:51 GMT  
		Size: 51.6 MB (51586431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3057f63e28cc1fe4f0dd11039577f14ac057f713e42e2b2e13000b37b8b86967
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127533393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4bbe255f47709b63ebef085398bae156c616dc66fa9f1980c105e345911141a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:41:46 GMT
ADD file:6547698ce9c0dce5d390e739342bd015a0c3266dba4ef5828dc1b1a9eb46e826 in / 
# Wed, 17 Nov 2021 02:41:47 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:29:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:29:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:30:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:67eeb578521bba47ceed6d5c2de23409a33ec3c1c6fda03d83e22d74dc1cdb76`  
		Last Modified: Wed, 17 Nov 2021 02:49:53 GMT  
		Size: 54.8 MB (54767045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f777f34bfc0463ddee51fc9ba3a1f668f6072f8431123ab0571266c60fb89c`  
		Last Modified: Wed, 17 Nov 2021 13:38:51 GMT  
		Size: 5.3 MB (5253448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e720a8fffb7aadf0b926dc4c5b3d7cb21c21c6ec5e507ddcdb546f5483b5a44e`  
		Last Modified: Wed, 17 Nov 2021 13:38:52 GMT  
		Size: 11.5 MB (11525452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cab4dc0eb95cf2e9a2e2a5f77eca7d76108730f09e1e205c09465b4fa35934`  
		Last Modified: Wed, 17 Nov 2021 13:39:12 GMT  
		Size: 56.0 MB (55987448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:733772bac49de30e8a05b0ad0e7d0340e5b5089313a4dfdb7f57a6d60552b79c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.5 MB (130503569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41174274a4fa2d6806ed55fabbfd91e97b22e8a8178e2412b0e819bceda895d8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:27 GMT
ADD file:9ab0c16547aac0a32292246b35737ca5260c5942d5e26ca1381be39c9e321ee5 in / 
# Tue, 12 Oct 2021 01:41:27 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:40:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:40:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 04:40:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c36fe1aa4217cf0326227a0bdcadc16e85d2670bd6485518167903dfc6934c65`  
		Last Modified: Tue, 12 Oct 2021 01:50:33 GMT  
		Size: 56.7 MB (56716103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1cefa3abf3c8d9687bfe164fbd73be6245f1e0c523603077cfcffd5881a3778`  
		Last Modified: Tue, 12 Oct 2021 04:51:12 GMT  
		Size: 5.3 MB (5346244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902f94685b9ef6228bbe2d7c552fb6d02ea5e723469df5c9e980d102fd9c6aa2`  
		Last Modified: Tue, 12 Oct 2021 04:51:13 GMT  
		Size: 11.3 MB (11281973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802e1fd067f1198f877ff5bc97afd5870c21a28609a1919a09063ff8aacf5fd4`  
		Last Modified: Tue, 12 Oct 2021 04:51:37 GMT  
		Size: 57.2 MB (57159249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:277451baec3ac7c41ff286c5d4bf89c602eb089f8ec4b24e96281dac4cea121f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.1 MB (126072580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48b49a0d880ec3185395fff15df7416540f343c3c377be897de3965fb23c1cfd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:12:23 GMT
ADD file:9e3985f5064204cf4c74f2d464977349398f8e0325083d223b22ace99f5dfa3a in / 
# Wed, 17 Nov 2021 02:12:24 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:39:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:39:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 08:41:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b79f1dde26df3dbfdaf094cc43f4dc602b492e9dd707f7a7874e1366808028c5`  
		Last Modified: Wed, 17 Nov 2021 02:22:36 GMT  
		Size: 54.4 MB (54365459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c0e1963482abb9ea5592b86c11c6528aebf6fe675fd25fdeb440cd4f999043`  
		Last Modified: Wed, 17 Nov 2021 08:52:05 GMT  
		Size: 5.2 MB (5227764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0761e303fe4f33cd92c7d2d5ce49857285721fb135e5bf569abf4ec59745f3d`  
		Last Modified: Wed, 17 Nov 2021 08:52:07 GMT  
		Size: 11.8 MB (11755031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c476b323dda6fd93fbb86e98139e76c07bff3f2d7a4b07b087d8e2c114b346f2`  
		Last Modified: Wed, 17 Nov 2021 08:52:57 GMT  
		Size: 54.7 MB (54724326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:8262acfa4cec540a727499b029781e6d9a768c80567ef0a550cc50eb38db0b5e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.5 MB (138527990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70616a1063b2854769c53da57f912b1b4adb02a65b34be74ac6b6749e1606f88`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 03:32:54 GMT
ADD file:33bc17dd3e3b6cd8c5ac37c8382a5d2b8e3ee8384b598b69b0d17b813dcfc767 in / 
# Wed, 17 Nov 2021 03:33:15 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:07:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:08:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 08:11:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:60fa303f933c621481dd7a32f72de0e35b85a3567ff116516725c45089e1cb88`  
		Last Modified: Wed, 17 Nov 2021 04:05:01 GMT  
		Size: 60.0 MB (60045015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a3dd48191daf1a5544d8a3146aececcefc7d4f8fe8e7e64e723022de0e5bae`  
		Last Modified: Wed, 17 Nov 2021 08:31:39 GMT  
		Size: 5.5 MB (5531621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147c14b8f9e107cd759a99e83c419ee5c8c99e500d16d4bbbfdb94cf6126b724`  
		Last Modified: Wed, 17 Nov 2021 08:31:39 GMT  
		Size: 12.6 MB (12551297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16114ff6b100453ae456bca4961ed144a5cd72589c05128a5b44f063feab7bb`  
		Last Modified: Wed, 17 Nov 2021 08:32:21 GMT  
		Size: 60.4 MB (60400057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:8486f624b42b956b1401a5bd240b03ad282ea1e54edb5242ea846893478a20ab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.8 MB (119790274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b441fc86b4e2662aeadd8e308872b18de076f1c73c976e045a69988dcff041e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:14:24 GMT
ADD file:9ce8adafd95fc1e31db924edf473abf22a68101cad20cd078c35db5fa719b34b in / 
# Wed, 17 Nov 2021 02:14:27 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:56:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:58:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:02:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a35675c997377ee8bf94b0a94460a6d2fd72a26b5c7fc6194b13ae99da869125`  
		Last Modified: Wed, 17 Nov 2021 02:30:42 GMT  
		Size: 51.5 MB (51522304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6561ec3264f30875424c0937b41795ce70f58306ddfe766af2fcb7d266b6a6`  
		Last Modified: Wed, 17 Nov 2021 03:35:29 GMT  
		Size: 5.1 MB (5080232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f12be064689662dab642f65c8e821186c7247cf7ea84901a22b9e2584d51ee`  
		Last Modified: Wed, 17 Nov 2021 03:35:32 GMT  
		Size: 11.1 MB (11140508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077cd6f4305eeccad12d3a65baeff88b63dd35ab2735a8b6ca9d8f523e0b6a0a`  
		Last Modified: Wed, 17 Nov 2021 03:37:41 GMT  
		Size: 52.0 MB (52047230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:8e5535d8b76c576ccc669d4f642fe2ed78be80df9778331222b1c87425845db7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.2 MB (126169798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6223c90d2c69ea15d0c2c6ca6033b860ee5f424c5d543919e86bc305d827047e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:43:42 GMT
ADD file:ba3a56dbd46c1324142a33ad1eefa66c34fda8c9c635140debf01131cb259e63 in / 
# Wed, 17 Nov 2021 02:43:45 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:11:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:12:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:12:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3595b50e30d7d0d412c142596638dbf5abfc27f196fe5d138ded04b66fd2b50e`  
		Last Modified: Wed, 17 Nov 2021 02:49:48 GMT  
		Size: 54.0 MB (53965664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634664d8b893813a04761069646d85aea7164717481b8c7e3f500e4260fc39ee`  
		Last Modified: Wed, 17 Nov 2021 03:19:03 GMT  
		Size: 5.2 MB (5248300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1780c6b7bcc6484f6ae6602c37ffd3bb2c9aad27b1b2587b796a5824e8b6575`  
		Last Modified: Wed, 17 Nov 2021 03:19:03 GMT  
		Size: 11.6 MB (11647079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a6bd04c7a7df4cb7de2e064bcfa156db3e89664ab5448cf33cf12043705f4f5`  
		Last Modified: Wed, 17 Nov 2021 03:19:17 GMT  
		Size: 55.3 MB (55308755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stable`

```console
$ docker pull buildpack-deps@sha256:39d6d1b626103d5d8daecf321abe9d8a1ce5cc8cbff2cd3195b4fdb04af654f3
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
$ docker pull buildpack-deps@sha256:067329836a99c56bd087b255c70cf2e7bb7f0c1965d8a12be769c86a062c12a4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.0 MB (322022992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48a4688637227faef31aa5134c34ca2ec85dd07beebcf327c38566eb3eb8ef79`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:15:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66b7f31b095b7fa01d8ba10e600a192bab43a1311f50216cf6fa9a45d0f435e`  
		Last Modified: Wed, 17 Nov 2021 03:24:18 GMT  
		Size: 196.5 MB (196498701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:095b3e58e31205572ba70b19cefdc7ec5de99683e74c0c8f095e3d564b2e1f0b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.1 MB (295100343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc59e839989efbe22d3c9e21e3cefb3c810799f569486d4f5493b98c454a3bb1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 00:49:54 GMT
ADD file:b9969604315238de271e1769a4b8dd85cdf0d33f9fac387e940d5195ac3030a1 in / 
# Tue, 12 Oct 2021 00:49:55 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:40:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:41:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 05:42:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:44:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a97c782f2538791984ce12c859cada96e395e3950d4cb7d1238e08acd2eb74ec`  
		Last Modified: Tue, 12 Oct 2021 01:05:12 GMT  
		Size: 52.5 MB (52452198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34dc529b005dbeff70906cd4baf2310c918ae6379fdf53ef632c3cd1203aa38`  
		Last Modified: Tue, 12 Oct 2021 06:01:18 GMT  
		Size: 5.1 MB (5063794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2876b7f933f68a5b4f35f854cc8c651bf3d21476fe2bb0a786e6376f389b44b`  
		Last Modified: Tue, 12 Oct 2021 06:01:20 GMT  
		Size: 10.6 MB (10571017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c918a5faa65bffd689b9869a942e77a3fbc7d89566be880da188d6050f4f627`  
		Last Modified: Tue, 12 Oct 2021 06:02:11 GMT  
		Size: 52.3 MB (52322898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3127725d64ae6922801ff988a903c7db9c780283ffb0ed82afa5763076b47be7`  
		Last Modified: Tue, 12 Oct 2021 06:04:12 GMT  
		Size: 174.7 MB (174690436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:d56f41aa9c8faf2f038f7d533362e91ee583358bc719176d20f3c17daad0fb9f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.5 MB (282546908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7d3fb1baab35afcb64347548d5cecdba2a8cd3c4299b815347de10b18e7fa29`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 01:59:07 GMT
ADD file:43b45f65ff4ba720f6f9a107b5f80818d5ea6ebc4835840b11e9a506351da32f in / 
# Wed, 17 Nov 2021 01:59:08 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:41:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:42:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 02:43:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:45:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dbbf55137aab3c7acd1e012a70f1ea1adeaef8d39b474829965d3480a02bf572`  
		Last Modified: Wed, 17 Nov 2021 02:14:27 GMT  
		Size: 50.1 MB (50134152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb1ae7a04cee77523f9e09a62b28632c56a700d0c481be7cddc566c835e7a71d`  
		Last Modified: Wed, 17 Nov 2021 03:04:13 GMT  
		Size: 4.9 MB (4922782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66894dfea839186e94448f6c25a37c6b3b1b42cece6332cc9d36336917e18a4`  
		Last Modified: Wed, 17 Nov 2021 03:04:14 GMT  
		Size: 10.2 MB (10216965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4502933ba6aa2071501257e094faa363699dc23995f798a124d688c2523240af`  
		Last Modified: Wed, 17 Nov 2021 03:05:05 GMT  
		Size: 50.3 MB (50327664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b521106771559ec34e350caa7c1220e7d91669cfdd392f09bf61b4de0ffbfed6`  
		Last Modified: Wed, 17 Nov 2021 03:06:54 GMT  
		Size: 166.9 MB (166945345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:53545965440c95434bfc95e564fd274f086892b89a42ff4ff145f60ef5ba02df
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.3 MB (313267051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:455c971696419e341265a976576201f36454718c107fcd51d4c07ecf67d23d13`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:59 GMT
ADD file:eb667e18226da8a1ca5a41beacddc65cd1efec01c3d01e50845c5e89e91ea17c in / 
# Wed, 17 Nov 2021 02:40:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:26:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:26:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:27:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:27:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce18cd0ba11c2dfa8c1a2d2b325e1e019b14d4ae25ffdeffb0f9686c5496bf5c`  
		Last Modified: Wed, 17 Nov 2021 02:46:45 GMT  
		Size: 53.6 MB (53619024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f138a340a2373acc72dcc4ea9ef08bdf5648aabc5fe08f7e8d25222ca63b7ee`  
		Last Modified: Wed, 17 Nov 2021 13:36:26 GMT  
		Size: 4.9 MB (4937639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34c030205ccb8656e30a58f96bb1edbe7c59bf17f3329ae3c442ec897f2b270`  
		Last Modified: Wed, 17 Nov 2021 13:36:27 GMT  
		Size: 10.7 MB (10655878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7a1cfcc2070fbe1e702751d85f7074b93d142f6beb03ef66e9ba1c58bcc3e3`  
		Last Modified: Wed, 17 Nov 2021 13:36:49 GMT  
		Size: 54.7 MB (54669696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3503a35f6e45ec76f6c25673ef4934feb88c3c35ee30ffc8bf7437a0ade8e15`  
		Last Modified: Wed, 17 Nov 2021 13:37:28 GMT  
		Size: 189.4 MB (189384814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:22b4c7d5f90e61044a709672c2f9f4172afc8d87432cb5e8ec6165670064022b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.8 MB (327786933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd6b36232cd4509daee36d1370c035efee46f839cd7eca26d55136f8274a2db8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:39:30 GMT
ADD file:e007d6eff02dbc696e1166db315b97a77ae8aa65f2e66ca8074765dde9c70a59 in / 
# Tue, 12 Oct 2021 01:39:31 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:35:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:36:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 04:36:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:37:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6911c8f66691266d86e2cafa67ca005d919f357436fac971c694d37625b5ba90`  
		Last Modified: Tue, 12 Oct 2021 01:47:06 GMT  
		Size: 55.9 MB (55923419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a0f31369a20c178b1d5c84f192412ed962068e8932d5821eefb00bc7d1cbc1a`  
		Last Modified: Tue, 12 Oct 2021 04:47:26 GMT  
		Size: 5.3 MB (5283102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97aa3d222d7e8d6e0b06e57e5bd03168c422475942f92d09a487bd98d09bb742`  
		Last Modified: Tue, 12 Oct 2021 04:47:27 GMT  
		Size: 11.3 MB (11250699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae99d06bab5fc31ba3db9436a22c452db74a7b5e559a451de2d971a493abe52`  
		Last Modified: Tue, 12 Oct 2021 04:48:03 GMT  
		Size: 55.9 MB (55917451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ceaeace1516b23dd6c26014f977ec910629b0f1e818efcba72285c444c745dc`  
		Last Modified: Tue, 12 Oct 2021 04:49:16 GMT  
		Size: 199.4 MB (199412262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:a2b66ff7f5602d629f435424734849d38a6e15416a23b64b2d23e13178660e84
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.1 MB (301083355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a25bde1d7937a6f6dd29e4c251d24e4a821689a59f57bb28e96e734a349c0faa`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:09:46 GMT
ADD file:2971df49f24648b8d5166d87e392e2547d5b03469356f20d112ce6feb3c329fc in / 
# Wed, 17 Nov 2021 02:09:47 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:29:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:30:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 08:31:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:33:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b095a0b63d99a4c4cd9c1c353f381a69ef041e6f80798d807ae51a34b04920a0`  
		Last Modified: Wed, 17 Nov 2021 02:18:22 GMT  
		Size: 53.2 MB (53183806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2e37aff1692726b1ea3dd0b4eeb684072527295f8e981d3c45825327daea19`  
		Last Modified: Wed, 17 Nov 2021 08:45:38 GMT  
		Size: 5.1 MB (5114925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d4c0302ddd7a6cb573a156076dba9c593e09a0c321b32ae0f1da2bd36bc754`  
		Last Modified: Wed, 17 Nov 2021 08:45:41 GMT  
		Size: 10.9 MB (10873360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cde5eca075420fcfc6498f454dc040f1e236dea180a82a0d27d7a739ffd41c1`  
		Last Modified: Wed, 17 Nov 2021 08:46:32 GMT  
		Size: 53.3 MB (53296603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b326e913cf09f7b591a15250a21e659e1a1490c8db287698247813607f511be`  
		Last Modified: Wed, 17 Nov 2021 08:48:42 GMT  
		Size: 178.6 MB (178614661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3ad89b390c0582bf3f9073da22edc33da00fa72294f690312f20c8670974f6ae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.6 MB (330552911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c32d3a8d6d884cd659ea67e7f174cd8ba989c9582a46828d4a63585aeaf8c56f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 03:27:04 GMT
ADD file:85375acb19da58f9eabaa67f8cb425cd1ff2dadb2888bbd9dbfa6223d16fef23 in / 
# Wed, 17 Nov 2021 03:27:20 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 07:40:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 07:40:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 07:42:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 07:51:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ede9cd7c8f1d380c971a130fb3d8a3914bf3a9106702164c23b2cce536fa618c`  
		Last Modified: Wed, 17 Nov 2021 03:52:39 GMT  
		Size: 58.8 MB (58819505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743814bfd79326104da0238d8edced6b14f63b95734b6dc0e2b7a9d83356b0cb`  
		Last Modified: Wed, 17 Nov 2021 08:25:58 GMT  
		Size: 5.4 MB (5402000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca978d94a6543bbd1c60026602b64e810b4bf65e052dcf19adf2b4d6b518bf8`  
		Last Modified: Wed, 17 Nov 2021 08:25:59 GMT  
		Size: 11.6 MB (11626016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d785f1d8909cb3a3e46844611c28e15781da809be0073e40af017d6e5631d0`  
		Last Modified: Wed, 17 Nov 2021 08:26:57 GMT  
		Size: 58.9 MB (58851458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18fadd6314eacb7e881a9590b8566952a97cc84d87002b2f80c125e36f166f91`  
		Last Modified: Wed, 17 Nov 2021 08:28:32 GMT  
		Size: 195.9 MB (195853932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b771ceede0a02f3c3e45fbf245a79af43a82d8a5a89e280847ac77f34783db7f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.6 MB (295637108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:424bab9df7f41f34456e281a4d38395352c0b8a719a123e6e3da820dad5b62e2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:07 GMT
ADD file:b7524e775a2033d246d1096765a0eb6eaa5ba6ed6c8b395522579d2c4e7a2e38 in / 
# Wed, 17 Nov 2021 02:42:09 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:07:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:07:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:08:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:09:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ffa47acd07831fbc96680a705da20704bac0016c20dc3c454ecd45cda44b368d`  
		Last Modified: Wed, 17 Nov 2021 02:48:05 GMT  
		Size: 53.2 MB (53207179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c950336719691da019c99e4ff78fe559ab0308ea145757994bdb7be34c6d224`  
		Last Modified: Wed, 17 Nov 2021 03:17:18 GMT  
		Size: 5.1 MB (5137199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d769af2ca44d1c7c206e7190cd71df7cb5ff3df2dd45e1dd52ea447ffb547b1a`  
		Last Modified: Wed, 17 Nov 2021 03:17:19 GMT  
		Size: 10.8 MB (10761499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3bbc68017b41a8cc07b10d715e2a23108c5addefa80b01cac1a2ef075bb1acd`  
		Last Modified: Wed, 17 Nov 2021 03:17:36 GMT  
		Size: 54.0 MB (54041155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5890dc05b0932fa2fcd5ebf331e2dbb96bf6af4989173b3745e7228388fc8f0a`  
		Last Modified: Wed, 17 Nov 2021 03:18:03 GMT  
		Size: 172.5 MB (172490076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stable-curl`

```console
$ docker pull buildpack-deps@sha256:55e8b08399933366af5bf7339d286a42b69484a144be7a9505b9652bb3abc9d4
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
$ docker pull buildpack-deps@sha256:0edf02c125a1738634b314fe74509188fe8ec80d4fe0e5dcb6a8e2c69b752eda
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.0 MB (70957967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4210c06ad2290080f1e15b81fcab4884d6d092607663ed35830d2cb7f05d88df`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:8f64ae6a92bbcdf3bd87aa336ab8cfbe025c94f2871fb30c7c869ddf5b398637
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68087009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:452c0670207bd3308452b37f769e1991141d3955fb9c449d6651538516664d78`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 00:49:54 GMT
ADD file:b9969604315238de271e1769a4b8dd85cdf0d33f9fac387e940d5195ac3030a1 in / 
# Tue, 12 Oct 2021 00:49:55 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:40:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:41:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a97c782f2538791984ce12c859cada96e395e3950d4cb7d1238e08acd2eb74ec`  
		Last Modified: Tue, 12 Oct 2021 01:05:12 GMT  
		Size: 52.5 MB (52452198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34dc529b005dbeff70906cd4baf2310c918ae6379fdf53ef632c3cd1203aa38`  
		Last Modified: Tue, 12 Oct 2021 06:01:18 GMT  
		Size: 5.1 MB (5063794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2876b7f933f68a5b4f35f854cc8c651bf3d21476fe2bb0a786e6376f389b44b`  
		Last Modified: Tue, 12 Oct 2021 06:01:20 GMT  
		Size: 10.6 MB (10571017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:e0db5a4c0ddaf3021a476cd83cb48a47baae27cafc02c61fd6151c2b113034fd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65273899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a096ebca0a1dcf6c812935690d2f1ceba23cdc7565b5dedf1b01adb266c3296a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 01:59:07 GMT
ADD file:43b45f65ff4ba720f6f9a107b5f80818d5ea6ebc4835840b11e9a506351da32f in / 
# Wed, 17 Nov 2021 01:59:08 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:41:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:42:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:dbbf55137aab3c7acd1e012a70f1ea1adeaef8d39b474829965d3480a02bf572`  
		Last Modified: Wed, 17 Nov 2021 02:14:27 GMT  
		Size: 50.1 MB (50134152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb1ae7a04cee77523f9e09a62b28632c56a700d0c481be7cddc566c835e7a71d`  
		Last Modified: Wed, 17 Nov 2021 03:04:13 GMT  
		Size: 4.9 MB (4922782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66894dfea839186e94448f6c25a37c6b3b1b42cece6332cc9d36336917e18a4`  
		Last Modified: Wed, 17 Nov 2021 03:04:14 GMT  
		Size: 10.2 MB (10216965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c52337b05fa1f275820e562dc39597db3ec027dbc6930cd6c1424233776c385c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69212541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:638dd156261f84c328de4551fcff54679fa0628f7b63b62344e169cb0cfdf82c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:59 GMT
ADD file:eb667e18226da8a1ca5a41beacddc65cd1efec01c3d01e50845c5e89e91ea17c in / 
# Wed, 17 Nov 2021 02:40:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:26:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:26:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ce18cd0ba11c2dfa8c1a2d2b325e1e019b14d4ae25ffdeffb0f9686c5496bf5c`  
		Last Modified: Wed, 17 Nov 2021 02:46:45 GMT  
		Size: 53.6 MB (53619024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f138a340a2373acc72dcc4ea9ef08bdf5648aabc5fe08f7e8d25222ca63b7ee`  
		Last Modified: Wed, 17 Nov 2021 13:36:26 GMT  
		Size: 4.9 MB (4937639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34c030205ccb8656e30a58f96bb1edbe7c59bf17f3329ae3c442ec897f2b270`  
		Last Modified: Wed, 17 Nov 2021 13:36:27 GMT  
		Size: 10.7 MB (10655878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:307bd4c6b80d221cc5ffaa51a6561a19f142cbe2349df40cd823c45df8a66d0c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72457220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1fe930770d8d6583e5406717d0128e6efa4aa9438733ab028c7df182c036184`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:39:30 GMT
ADD file:e007d6eff02dbc696e1166db315b97a77ae8aa65f2e66ca8074765dde9c70a59 in / 
# Tue, 12 Oct 2021 01:39:31 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:35:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:36:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6911c8f66691266d86e2cafa67ca005d919f357436fac971c694d37625b5ba90`  
		Last Modified: Tue, 12 Oct 2021 01:47:06 GMT  
		Size: 55.9 MB (55923419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a0f31369a20c178b1d5c84f192412ed962068e8932d5821eefb00bc7d1cbc1a`  
		Last Modified: Tue, 12 Oct 2021 04:47:26 GMT  
		Size: 5.3 MB (5283102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97aa3d222d7e8d6e0b06e57e5bd03168c422475942f92d09a487bd98d09bb742`  
		Last Modified: Tue, 12 Oct 2021 04:47:27 GMT  
		Size: 11.3 MB (11250699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:c8e1c20d487b63fa0111dd8c6dbb3e8cad660d4ad92dfedcc288dbcf88b52ae1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69172091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e01b4e0250266355d14651090fbb68f4b5950f1e1e3e93ad45e1d024d3e8db78`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:09:46 GMT
ADD file:2971df49f24648b8d5166d87e392e2547d5b03469356f20d112ce6feb3c329fc in / 
# Wed, 17 Nov 2021 02:09:47 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:29:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:30:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b095a0b63d99a4c4cd9c1c353f381a69ef041e6f80798d807ae51a34b04920a0`  
		Last Modified: Wed, 17 Nov 2021 02:18:22 GMT  
		Size: 53.2 MB (53183806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2e37aff1692726b1ea3dd0b4eeb684072527295f8e981d3c45825327daea19`  
		Last Modified: Wed, 17 Nov 2021 08:45:38 GMT  
		Size: 5.1 MB (5114925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d4c0302ddd7a6cb573a156076dba9c593e09a0c321b32ae0f1da2bd36bc754`  
		Last Modified: Wed, 17 Nov 2021 08:45:41 GMT  
		Size: 10.9 MB (10873360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:ffc112a46cd4cb66176c5d7b815903b1652b33a26fb9f38d3233e1892293d496
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.8 MB (75847521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17cfe935fd31679e71de8a6756361a413d64351be692488a2fd6c0de16648ada`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 03:27:04 GMT
ADD file:85375acb19da58f9eabaa67f8cb425cd1ff2dadb2888bbd9dbfa6223d16fef23 in / 
# Wed, 17 Nov 2021 03:27:20 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 07:40:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 07:40:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ede9cd7c8f1d380c971a130fb3d8a3914bf3a9106702164c23b2cce536fa618c`  
		Last Modified: Wed, 17 Nov 2021 03:52:39 GMT  
		Size: 58.8 MB (58819505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743814bfd79326104da0238d8edced6b14f63b95734b6dc0e2b7a9d83356b0cb`  
		Last Modified: Wed, 17 Nov 2021 08:25:58 GMT  
		Size: 5.4 MB (5402000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca978d94a6543bbd1c60026602b64e810b4bf65e052dcf19adf2b4d6b518bf8`  
		Last Modified: Wed, 17 Nov 2021 08:25:59 GMT  
		Size: 11.6 MB (11626016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:864eebbaafc1154c0017d16100182a15ea13c7dd81a1e2474b581c03a8e4d27c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69105877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d1c13a820b2c0e693a7fcd87c7888df8a0f95367ff8e2381ec07faf8e711307`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:07 GMT
ADD file:b7524e775a2033d246d1096765a0eb6eaa5ba6ed6c8b395522579d2c4e7a2e38 in / 
# Wed, 17 Nov 2021 02:42:09 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:07:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:07:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ffa47acd07831fbc96680a705da20704bac0016c20dc3c454ecd45cda44b368d`  
		Last Modified: Wed, 17 Nov 2021 02:48:05 GMT  
		Size: 53.2 MB (53207179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c950336719691da019c99e4ff78fe559ab0308ea145757994bdb7be34c6d224`  
		Last Modified: Wed, 17 Nov 2021 03:17:18 GMT  
		Size: 5.1 MB (5137199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d769af2ca44d1c7c206e7190cd71df7cb5ff3df2dd45e1dd52ea447ffb547b1a`  
		Last Modified: Wed, 17 Nov 2021 03:17:19 GMT  
		Size: 10.8 MB (10761499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stable-scm`

```console
$ docker pull buildpack-deps@sha256:993f6b93af203b5057bca0bf5858d22798c837de81f63c65326cf4bd25734d20
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
$ docker pull buildpack-deps@sha256:705b87b1c31cbc5283ea312fb0af16deeda2d00a9121f33d1779813dff4dd55b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.5 MB (125524291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e81de6f42b69f2697b8b01a08799441414abcedf96ec293b306eddb6d0d6c8ba`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:ab1b571f15dc9620590ae51b9e2a70cfb75b6438013b7a3599f47e39f6c7d600
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.4 MB (120409907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e962133851ffbc9d390eb7b46532392de0c1e19443d48ed2c7a52c4ca877cc2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 00:49:54 GMT
ADD file:b9969604315238de271e1769a4b8dd85cdf0d33f9fac387e940d5195ac3030a1 in / 
# Tue, 12 Oct 2021 00:49:55 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:40:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:41:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 05:42:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a97c782f2538791984ce12c859cada96e395e3950d4cb7d1238e08acd2eb74ec`  
		Last Modified: Tue, 12 Oct 2021 01:05:12 GMT  
		Size: 52.5 MB (52452198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34dc529b005dbeff70906cd4baf2310c918ae6379fdf53ef632c3cd1203aa38`  
		Last Modified: Tue, 12 Oct 2021 06:01:18 GMT  
		Size: 5.1 MB (5063794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2876b7f933f68a5b4f35f854cc8c651bf3d21476fe2bb0a786e6376f389b44b`  
		Last Modified: Tue, 12 Oct 2021 06:01:20 GMT  
		Size: 10.6 MB (10571017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c918a5faa65bffd689b9869a942e77a3fbc7d89566be880da188d6050f4f627`  
		Last Modified: Tue, 12 Oct 2021 06:02:11 GMT  
		Size: 52.3 MB (52322898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:19565c156eedbb4210675b27d3f633814a7f585b53d58729e1fe465da7904001
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.6 MB (115601563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31f5dfdc32269a08b775b7b18972781651a1103e34bb2eb596fda4bcd843f1af`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 01:59:07 GMT
ADD file:43b45f65ff4ba720f6f9a107b5f80818d5ea6ebc4835840b11e9a506351da32f in / 
# Wed, 17 Nov 2021 01:59:08 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:41:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:42:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 02:43:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dbbf55137aab3c7acd1e012a70f1ea1adeaef8d39b474829965d3480a02bf572`  
		Last Modified: Wed, 17 Nov 2021 02:14:27 GMT  
		Size: 50.1 MB (50134152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb1ae7a04cee77523f9e09a62b28632c56a700d0c481be7cddc566c835e7a71d`  
		Last Modified: Wed, 17 Nov 2021 03:04:13 GMT  
		Size: 4.9 MB (4922782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66894dfea839186e94448f6c25a37c6b3b1b42cece6332cc9d36336917e18a4`  
		Last Modified: Wed, 17 Nov 2021 03:04:14 GMT  
		Size: 10.2 MB (10216965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4502933ba6aa2071501257e094faa363699dc23995f798a124d688c2523240af`  
		Last Modified: Wed, 17 Nov 2021 03:05:05 GMT  
		Size: 50.3 MB (50327664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d98321260829308a2348a158000abedf1fcd03e58d44ac414c3d077d1c110c70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.9 MB (123882237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32fa5708561ca81a99850197b076caf6f432ccb91bee5a5df1a4e6a478d3ec3f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:59 GMT
ADD file:eb667e18226da8a1ca5a41beacddc65cd1efec01c3d01e50845c5e89e91ea17c in / 
# Wed, 17 Nov 2021 02:40:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:26:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:26:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:27:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce18cd0ba11c2dfa8c1a2d2b325e1e019b14d4ae25ffdeffb0f9686c5496bf5c`  
		Last Modified: Wed, 17 Nov 2021 02:46:45 GMT  
		Size: 53.6 MB (53619024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f138a340a2373acc72dcc4ea9ef08bdf5648aabc5fe08f7e8d25222ca63b7ee`  
		Last Modified: Wed, 17 Nov 2021 13:36:26 GMT  
		Size: 4.9 MB (4937639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34c030205ccb8656e30a58f96bb1edbe7c59bf17f3329ae3c442ec897f2b270`  
		Last Modified: Wed, 17 Nov 2021 13:36:27 GMT  
		Size: 10.7 MB (10655878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7a1cfcc2070fbe1e702751d85f7074b93d142f6beb03ef66e9ba1c58bcc3e3`  
		Last Modified: Wed, 17 Nov 2021 13:36:49 GMT  
		Size: 54.7 MB (54669696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:16abe77eeca3b6e96cff6cf2bbff639647cf581d03efc6c7dcb8ab3fb5fa8bd2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128374671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:363c0a8d58ad2bab650032b97601a821766dc54ba78827525e9e45381d993d08`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:39:30 GMT
ADD file:e007d6eff02dbc696e1166db315b97a77ae8aa65f2e66ca8074765dde9c70a59 in / 
# Tue, 12 Oct 2021 01:39:31 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:35:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:36:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 04:36:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6911c8f66691266d86e2cafa67ca005d919f357436fac971c694d37625b5ba90`  
		Last Modified: Tue, 12 Oct 2021 01:47:06 GMT  
		Size: 55.9 MB (55923419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a0f31369a20c178b1d5c84f192412ed962068e8932d5821eefb00bc7d1cbc1a`  
		Last Modified: Tue, 12 Oct 2021 04:47:26 GMT  
		Size: 5.3 MB (5283102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97aa3d222d7e8d6e0b06e57e5bd03168c422475942f92d09a487bd98d09bb742`  
		Last Modified: Tue, 12 Oct 2021 04:47:27 GMT  
		Size: 11.3 MB (11250699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae99d06bab5fc31ba3db9436a22c452db74a7b5e559a451de2d971a493abe52`  
		Last Modified: Tue, 12 Oct 2021 04:48:03 GMT  
		Size: 55.9 MB (55917451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:a5be5277770524bd35dd921bc7f03adf64d8bf76eeee88ba1a6fb10f62aa65a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.5 MB (122468694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afe05d4524b16661e35a811e3b2f3a1ea3e0fc1ca56eb4306839c755f24c34ef`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:09:46 GMT
ADD file:2971df49f24648b8d5166d87e392e2547d5b03469356f20d112ce6feb3c329fc in / 
# Wed, 17 Nov 2021 02:09:47 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:29:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:30:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 08:31:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b095a0b63d99a4c4cd9c1c353f381a69ef041e6f80798d807ae51a34b04920a0`  
		Last Modified: Wed, 17 Nov 2021 02:18:22 GMT  
		Size: 53.2 MB (53183806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2e37aff1692726b1ea3dd0b4eeb684072527295f8e981d3c45825327daea19`  
		Last Modified: Wed, 17 Nov 2021 08:45:38 GMT  
		Size: 5.1 MB (5114925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d4c0302ddd7a6cb573a156076dba9c593e09a0c321b32ae0f1da2bd36bc754`  
		Last Modified: Wed, 17 Nov 2021 08:45:41 GMT  
		Size: 10.9 MB (10873360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cde5eca075420fcfc6498f454dc040f1e236dea180a82a0d27d7a739ffd41c1`  
		Last Modified: Wed, 17 Nov 2021 08:46:32 GMT  
		Size: 53.3 MB (53296603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:faf4c1b1a0373960c09ef3f862d4fcd8e9c6bc9b842a86cdf1ab3405f45a9f3c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134698979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b960badc27a250634b2e76a6871d276d149dcd0fe0fe615bbf2f54db9efc221b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 03:27:04 GMT
ADD file:85375acb19da58f9eabaa67f8cb425cd1ff2dadb2888bbd9dbfa6223d16fef23 in / 
# Wed, 17 Nov 2021 03:27:20 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 07:40:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 07:40:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 07:42:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ede9cd7c8f1d380c971a130fb3d8a3914bf3a9106702164c23b2cce536fa618c`  
		Last Modified: Wed, 17 Nov 2021 03:52:39 GMT  
		Size: 58.8 MB (58819505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743814bfd79326104da0238d8edced6b14f63b95734b6dc0e2b7a9d83356b0cb`  
		Last Modified: Wed, 17 Nov 2021 08:25:58 GMT  
		Size: 5.4 MB (5402000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca978d94a6543bbd1c60026602b64e810b4bf65e052dcf19adf2b4d6b518bf8`  
		Last Modified: Wed, 17 Nov 2021 08:25:59 GMT  
		Size: 11.6 MB (11626016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d785f1d8909cb3a3e46844611c28e15781da809be0073e40af017d6e5631d0`  
		Last Modified: Wed, 17 Nov 2021 08:26:57 GMT  
		Size: 58.9 MB (58851458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:673b0a54f0e03e540c534b0dfc3525d90049ec556ed645e24d83e7eaa1dd159f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123147032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ec10947074405be072d3cee591cea9230aa7dd19dafc623039d1644d6083ca4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:07 GMT
ADD file:b7524e775a2033d246d1096765a0eb6eaa5ba6ed6c8b395522579d2c4e7a2e38 in / 
# Wed, 17 Nov 2021 02:42:09 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:07:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:07:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:08:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ffa47acd07831fbc96680a705da20704bac0016c20dc3c454ecd45cda44b368d`  
		Last Modified: Wed, 17 Nov 2021 02:48:05 GMT  
		Size: 53.2 MB (53207179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c950336719691da019c99e4ff78fe559ab0308ea145757994bdb7be34c6d224`  
		Last Modified: Wed, 17 Nov 2021 03:17:18 GMT  
		Size: 5.1 MB (5137199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d769af2ca44d1c7c206e7190cd71df7cb5ff3df2dd45e1dd52ea447ffb547b1a`  
		Last Modified: Wed, 17 Nov 2021 03:17:19 GMT  
		Size: 10.8 MB (10761499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3bbc68017b41a8cc07b10d715e2a23108c5addefa80b01cac1a2ef075bb1acd`  
		Last Modified: Wed, 17 Nov 2021 03:17:36 GMT  
		Size: 54.0 MB (54041155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stretch`

```console
$ docker pull buildpack-deps@sha256:b83d6f9f3e784ab663beeddb4f9b15ec04f5ef9996f9fa9c28cb7ba7027aa558
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
$ docker pull buildpack-deps@sha256:1f84211ee3ff7baac91f583b97571f0abe60c11e1f29e0ebf5fa332b9d8981e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.2 MB (325233927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21c35b5593f396fdaa3497088189c39f7524d01ff424cd5f42eafc81bb0db7c1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:22:28 GMT
ADD file:d7365dd9cf34b10ca189f85c95c21a0c33e44092f85ffb5884d5e737fb0b9be1 in / 
# Wed, 17 Nov 2021 02:22:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:19:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:19:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:20:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:200cae5c9d88bb9cf1dd3fcfb831d671403f078d2310416fa3b304337d8279c0`  
		Last Modified: Wed, 17 Nov 2021 02:29:09 GMT  
		Size: 45.4 MB (45380444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047156b8adafd241846cd5539cebd45e6e28fe1bd818cd654a0124cef61d4cb2`  
		Last Modified: Wed, 17 Nov 2021 03:27:27 GMT  
		Size: 11.3 MB (11301447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cbf304dd51feb48b321b93ae5b8a5a6ca55c23b51a8dc0d9642c3c3b5081a7`  
		Last Modified: Wed, 17 Nov 2021 03:27:26 GMT  
		Size: 4.3 MB (4342326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6e9db633dd66ac91ed2df32c5900c5a1ae82b58cc9261fd240913743d283ca`  
		Last Modified: Wed, 17 Nov 2021 03:27:45 GMT  
		Size: 49.8 MB (49762330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16c1fa47fbffbf5d3d0c694fb480235a6ba765befaef57b62680514af6c2d0b8`  
		Last Modified: Wed, 17 Nov 2021 03:28:26 GMT  
		Size: 214.4 MB (214447380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:f1b619365d5dce8c961a51631354d01e66aadc6b82191aea0fde832ea20a8edc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.1 MB (309147959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8519ad77bacec454b6c51f92bdb6396c985f1edb4fc29146cadf27502ffe697e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 00:55:37 GMT
ADD file:eb65cc31f82e76c4ea5a8f21e4cad1372399517ee41a759740ff91d1d23b9e44 in / 
# Tue, 12 Oct 2021 00:55:38 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:54:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:54:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 05:55:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:58:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d2f67fd5897d122073fc9ad347c1fb9faec31555c47b3ee6ff64ca2b553034ed`  
		Last Modified: Tue, 12 Oct 2021 01:13:31 GMT  
		Size: 44.1 MB (44091932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b4f8f4eb65e840d4778dd2e77e7cc6d546cbd55ed717e53e017c853e7c07d1`  
		Last Modified: Tue, 12 Oct 2021 06:12:15 GMT  
		Size: 10.4 MB (10351740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec0c01cd7d7e35fbb8d775a4bca6166749569cbf3c1bc4b9a5aee530bff8978`  
		Last Modified: Tue, 12 Oct 2021 06:12:12 GMT  
		Size: 4.2 MB (4161429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb3ac8456e186fb75e7aaf1c21260430344e8cf1d6cd6fdaec9bfb9ab5a0741`  
		Last Modified: Tue, 12 Oct 2021 06:12:58 GMT  
		Size: 48.0 MB (47984451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e836375083dc2ab922dd843b4cf24c13682693e3391b6c1429c233240bafa36b`  
		Last Modified: Tue, 12 Oct 2021 06:15:09 GMT  
		Size: 202.6 MB (202558407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:34e043644f0b3472348ca1922c817cfead39d47718cd0bf195b133b74594853d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.2 MB (297172929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:629cf466cec2a9b62004e6fabb013a03aaa948260188a7536d7039dd7d23f63e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:04:57 GMT
ADD file:61da3fcef3aea99b4927189cfcb823a65b0e911a3f4436e44ea84a57a7919ff3 in / 
# Wed, 17 Nov 2021 02:04:58 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:54:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:54:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 02:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:57:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e4d54b576c2fcdd259e57bac14c4e1a2623f6e5dc9a0b1facaed7fe59d891e86`  
		Last Modified: Wed, 17 Nov 2021 02:22:03 GMT  
		Size: 42.1 MB (42116868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf04dd2447fcded30a4c9a8d7a054ccb2e4c4db4118989ea05bf2e56d60a8924`  
		Last Modified: Wed, 17 Nov 2021 03:14:24 GMT  
		Size: 10.0 MB (9956153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b37c8e78d6ca4f8e5467e0ec7ef61eef6101e99c8154472df98aa34159f5974`  
		Last Modified: Wed, 17 Nov 2021 03:14:21 GMT  
		Size: 3.9 MB (3921214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fcf28009119cc468ce87b98d583e8c51d3703937d10d502a704f1032bc2b26`  
		Last Modified: Wed, 17 Nov 2021 03:15:08 GMT  
		Size: 46.1 MB (46126162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b8b79b0de7febe2c3b866e2f14fe48bca033ef5ee3eda5193c147f47eb3f55`  
		Last Modified: Wed, 17 Nov 2021 03:17:08 GMT  
		Size: 195.1 MB (195052532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:eb62a7fc0d18f0f9cde800bdbec22f5baf0e77c4d4be12290a6dfe5dd5dff258
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.8 MB (306765224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef6ac97bc2ecd37279a6f1b4e04c10b22609eeabb9496051c80999f502d8d752`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:33 GMT
ADD file:3225671be4edc3599e29ebd06516b95573246e68bf29649c402ed87c03c109b5 in / 
# Wed, 17 Nov 2021 02:42:34 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:32:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:32:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:32:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:33:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c64a4bafe4ad6fc05fcc6d76d2a06f168f331ffbc87e518fb4ca4ea22e75527e`  
		Last Modified: Wed, 17 Nov 2021 02:51:11 GMT  
		Size: 43.2 MB (43174478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deaddc7c2a37cd151a9001bbe7816f06f5f36ac6d53cc0d02fe2b327f85a2c7e`  
		Last Modified: Wed, 17 Nov 2021 13:40:24 GMT  
		Size: 10.2 MB (10216788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61401ffc70123532d1f4886b9ebd00e11d1155a2363117bf5aab10353c373dc9`  
		Last Modified: Wed, 17 Nov 2021 13:40:23 GMT  
		Size: 3.9 MB (3873891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185eee4daee1ed1fa34e853c2332cc4253415d7e015143b2432a96047c88d828`  
		Last Modified: Wed, 17 Nov 2021 13:40:43 GMT  
		Size: 47.7 MB (47734854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc999035e89072506c3f538d25644144fcabf1babfd2b71bfdd62c2ac570b8d0`  
		Last Modified: Wed, 17 Nov 2021 13:41:25 GMT  
		Size: 201.8 MB (201765213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch` - linux; 386

```console
$ docker pull buildpack-deps@sha256:d51e19c8a7f30a56580661332d964aa73ab70b00fc602feeb7c96051a8d3794d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.7 MB (332749925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e1c89142617e6ea716a487a28ff686e7b1826f983f94e53ab383bb6677f224c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:42:19 GMT
ADD file:5a6f08cc731f24357c3702231256fb05eb0a97733779b2ace406ba3c9bf64baa in / 
# Tue, 12 Oct 2021 01:42:19 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:42:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:42:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 04:43:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:44:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d2ef4e90cca7406b4907a34e3571153fc56e3ecc9b2b5fdbb7787f22877cfec5`  
		Last Modified: Tue, 12 Oct 2021 01:51:58 GMT  
		Size: 46.1 MB (46097164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9020db84c7cf31b7929c21a2b6fe2123900e91c7391ad6f4ee5560a934f382`  
		Last Modified: Tue, 12 Oct 2021 04:52:49 GMT  
		Size: 11.4 MB (11358857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8cbe9196a8b6bd3825445c718bc5a248b7c295b4d9f45756819e8bf27cb72b`  
		Last Modified: Tue, 12 Oct 2021 04:52:47 GMT  
		Size: 4.6 MB (4565012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7454f0fe0ebf5d024897d682d46181ab978a980f7f40caa2492a83cc39f75ec`  
		Last Modified: Tue, 12 Oct 2021 04:53:20 GMT  
		Size: 51.3 MB (51264783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d689f4cc817a5dea61b3cd4ed2680f093caa75b7c811cee4392ea0effff4f5c`  
		Last Modified: Tue, 12 Oct 2021 04:54:33 GMT  
		Size: 219.5 MB (219464109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stretch-curl`

```console
$ docker pull buildpack-deps@sha256:e2c7c02aeaae59464b9bf9a1315c291bcaef9b2b840b0750e6c242d20a1714b0
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
$ docker pull buildpack-deps@sha256:cf8274ff3f94d52058249c3fa2a3fa6f58da3f51f5bbaa18d26d451a11e55190
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.0 MB (61024217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0886d8702caa5ba4caa2911a9a70b0d489f272aa850952a75f880b9f4664d388`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:22:28 GMT
ADD file:d7365dd9cf34b10ca189f85c95c21a0c33e44092f85ffb5884d5e737fb0b9be1 in / 
# Wed, 17 Nov 2021 02:22:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:19:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:200cae5c9d88bb9cf1dd3fcfb831d671403f078d2310416fa3b304337d8279c0`  
		Last Modified: Wed, 17 Nov 2021 02:29:09 GMT  
		Size: 45.4 MB (45380444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047156b8adafd241846cd5539cebd45e6e28fe1bd818cd654a0124cef61d4cb2`  
		Last Modified: Wed, 17 Nov 2021 03:27:27 GMT  
		Size: 11.3 MB (11301447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cbf304dd51feb48b321b93ae5b8a5a6ca55c23b51a8dc0d9642c3c3b5081a7`  
		Last Modified: Wed, 17 Nov 2021 03:27:26 GMT  
		Size: 4.3 MB (4342326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:d22384305baafb9cd36935a9bdefcf829118d3d1458b5d353798b97b3f6e83d3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.6 MB (58605101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddb7b424b63a5db211ff320d4629b66d91f09ff2fff4d2236cdc7316f3201f9c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 00:55:37 GMT
ADD file:eb65cc31f82e76c4ea5a8f21e4cad1372399517ee41a759740ff91d1d23b9e44 in / 
# Tue, 12 Oct 2021 00:55:38 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:54:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:54:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d2f67fd5897d122073fc9ad347c1fb9faec31555c47b3ee6ff64ca2b553034ed`  
		Last Modified: Tue, 12 Oct 2021 01:13:31 GMT  
		Size: 44.1 MB (44091932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b4f8f4eb65e840d4778dd2e77e7cc6d546cbd55ed717e53e017c853e7c07d1`  
		Last Modified: Tue, 12 Oct 2021 06:12:15 GMT  
		Size: 10.4 MB (10351740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec0c01cd7d7e35fbb8d775a4bca6166749569cbf3c1bc4b9a5aee530bff8978`  
		Last Modified: Tue, 12 Oct 2021 06:12:12 GMT  
		Size: 4.2 MB (4161429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:2e294312a129ae76beed8f6db683fefb2075deea7406f388f37b2aa606cebb30
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (55994235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ac3b5ed742906ac82c169d00412d6043ee6e55561442421ef66c7d392c8506d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:04:57 GMT
ADD file:61da3fcef3aea99b4927189cfcb823a65b0e911a3f4436e44ea84a57a7919ff3 in / 
# Wed, 17 Nov 2021 02:04:58 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:54:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:54:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e4d54b576c2fcdd259e57bac14c4e1a2623f6e5dc9a0b1facaed7fe59d891e86`  
		Last Modified: Wed, 17 Nov 2021 02:22:03 GMT  
		Size: 42.1 MB (42116868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf04dd2447fcded30a4c9a8d7a054ccb2e4c4db4118989ea05bf2e56d60a8924`  
		Last Modified: Wed, 17 Nov 2021 03:14:24 GMT  
		Size: 10.0 MB (9956153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b37c8e78d6ca4f8e5467e0ec7ef61eef6101e99c8154472df98aa34159f5974`  
		Last Modified: Wed, 17 Nov 2021 03:14:21 GMT  
		Size: 3.9 MB (3921214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f8c63f2967bc872468d5e51917554a8ea360b461f6c6b1461b826a6442d19490
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.3 MB (57265157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:014f4bdee0c150fb8cf8cdfff5d193c2eaced3df30b883271791d6a840b6567b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:33 GMT
ADD file:3225671be4edc3599e29ebd06516b95573246e68bf29649c402ed87c03c109b5 in / 
# Wed, 17 Nov 2021 02:42:34 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:32:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:32:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c64a4bafe4ad6fc05fcc6d76d2a06f168f331ffbc87e518fb4ca4ea22e75527e`  
		Last Modified: Wed, 17 Nov 2021 02:51:11 GMT  
		Size: 43.2 MB (43174478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deaddc7c2a37cd151a9001bbe7816f06f5f36ac6d53cc0d02fe2b327f85a2c7e`  
		Last Modified: Wed, 17 Nov 2021 13:40:24 GMT  
		Size: 10.2 MB (10216788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61401ffc70123532d1f4886b9ebd00e11d1155a2363117bf5aab10353c373dc9`  
		Last Modified: Wed, 17 Nov 2021 13:40:23 GMT  
		Size: 3.9 MB (3873891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:27a549af269a461e6896cf3b3a7199e34e7417ff4f572c30ff2815b85cf0d5b5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (62021033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0aa60dbddb29720e51a7ec1ada2bba0a56158d345ab8caed4a5537a267eb8957`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:42:19 GMT
ADD file:5a6f08cc731f24357c3702231256fb05eb0a97733779b2ace406ba3c9bf64baa in / 
# Tue, 12 Oct 2021 01:42:19 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:42:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:42:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d2ef4e90cca7406b4907a34e3571153fc56e3ecc9b2b5fdbb7787f22877cfec5`  
		Last Modified: Tue, 12 Oct 2021 01:51:58 GMT  
		Size: 46.1 MB (46097164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9020db84c7cf31b7929c21a2b6fe2123900e91c7391ad6f4ee5560a934f382`  
		Last Modified: Tue, 12 Oct 2021 04:52:49 GMT  
		Size: 11.4 MB (11358857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8cbe9196a8b6bd3825445c718bc5a248b7c295b4d9f45756819e8bf27cb72b`  
		Last Modified: Tue, 12 Oct 2021 04:52:47 GMT  
		Size: 4.6 MB (4565012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stretch-scm`

```console
$ docker pull buildpack-deps@sha256:671522708995c6015365c1ffbf4ec04af96a02b3cd6b4fe799ae946fc7dab362
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
$ docker pull buildpack-deps@sha256:b0f76319830edb0ebac43cd1e76a4c2a5d34e847b9bb3f7371bbfebe57eb205f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.8 MB (110786547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cea98b6e932cedec41f17989129c68a1bd3d343c834ab1c992efb3bc8544888`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:22:28 GMT
ADD file:d7365dd9cf34b10ca189f85c95c21a0c33e44092f85ffb5884d5e737fb0b9be1 in / 
# Wed, 17 Nov 2021 02:22:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:19:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:19:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:200cae5c9d88bb9cf1dd3fcfb831d671403f078d2310416fa3b304337d8279c0`  
		Last Modified: Wed, 17 Nov 2021 02:29:09 GMT  
		Size: 45.4 MB (45380444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047156b8adafd241846cd5539cebd45e6e28fe1bd818cd654a0124cef61d4cb2`  
		Last Modified: Wed, 17 Nov 2021 03:27:27 GMT  
		Size: 11.3 MB (11301447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cbf304dd51feb48b321b93ae5b8a5a6ca55c23b51a8dc0d9642c3c3b5081a7`  
		Last Modified: Wed, 17 Nov 2021 03:27:26 GMT  
		Size: 4.3 MB (4342326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6e9db633dd66ac91ed2df32c5900c5a1ae82b58cc9261fd240913743d283ca`  
		Last Modified: Wed, 17 Nov 2021 03:27:45 GMT  
		Size: 49.8 MB (49762330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:3b6dcef1865cc1d9df51cfcede2b22a42810d59e1ed7f2dd6f1a2afdab2da382
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.6 MB (106589552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f1b47c4fc7cd09da1eadb373e1b3639dd3ea6f0d0a7f277a6f9a3a1badf1916`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 00:55:37 GMT
ADD file:eb65cc31f82e76c4ea5a8f21e4cad1372399517ee41a759740ff91d1d23b9e44 in / 
# Tue, 12 Oct 2021 00:55:38 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:54:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:54:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 05:55:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d2f67fd5897d122073fc9ad347c1fb9faec31555c47b3ee6ff64ca2b553034ed`  
		Last Modified: Tue, 12 Oct 2021 01:13:31 GMT  
		Size: 44.1 MB (44091932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b4f8f4eb65e840d4778dd2e77e7cc6d546cbd55ed717e53e017c853e7c07d1`  
		Last Modified: Tue, 12 Oct 2021 06:12:15 GMT  
		Size: 10.4 MB (10351740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec0c01cd7d7e35fbb8d775a4bca6166749569cbf3c1bc4b9a5aee530bff8978`  
		Last Modified: Tue, 12 Oct 2021 06:12:12 GMT  
		Size: 4.2 MB (4161429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb3ac8456e186fb75e7aaf1c21260430344e8cf1d6cd6fdaec9bfb9ab5a0741`  
		Last Modified: Tue, 12 Oct 2021 06:12:58 GMT  
		Size: 48.0 MB (47984451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:06b12ba3a191d0ec83b7588cd9cb7e94e5206746fe70cef1b57974f1c21f5097
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102120397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c01627a3706745a8b4f9600a77ff4453ce771391c424dff9199dbdfbec858c24`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:04:57 GMT
ADD file:61da3fcef3aea99b4927189cfcb823a65b0e911a3f4436e44ea84a57a7919ff3 in / 
# Wed, 17 Nov 2021 02:04:58 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:54:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:54:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 02:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e4d54b576c2fcdd259e57bac14c4e1a2623f6e5dc9a0b1facaed7fe59d891e86`  
		Last Modified: Wed, 17 Nov 2021 02:22:03 GMT  
		Size: 42.1 MB (42116868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf04dd2447fcded30a4c9a8d7a054ccb2e4c4db4118989ea05bf2e56d60a8924`  
		Last Modified: Wed, 17 Nov 2021 03:14:24 GMT  
		Size: 10.0 MB (9956153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b37c8e78d6ca4f8e5467e0ec7ef61eef6101e99c8154472df98aa34159f5974`  
		Last Modified: Wed, 17 Nov 2021 03:14:21 GMT  
		Size: 3.9 MB (3921214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fcf28009119cc468ce87b98d583e8c51d3703937d10d502a704f1032bc2b26`  
		Last Modified: Wed, 17 Nov 2021 03:15:08 GMT  
		Size: 46.1 MB (46126162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:eee3dd1c4660b65af7e8f4b3b200e6b89d3b7f43fa955fcb1678a602aef8a32e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105000011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52b744ede03418aaf0da398c56b90d7f07486c457d319e40f083d7ed41ea3639`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:33 GMT
ADD file:3225671be4edc3599e29ebd06516b95573246e68bf29649c402ed87c03c109b5 in / 
# Wed, 17 Nov 2021 02:42:34 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:32:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:32:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:32:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c64a4bafe4ad6fc05fcc6d76d2a06f168f331ffbc87e518fb4ca4ea22e75527e`  
		Last Modified: Wed, 17 Nov 2021 02:51:11 GMT  
		Size: 43.2 MB (43174478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deaddc7c2a37cd151a9001bbe7816f06f5f36ac6d53cc0d02fe2b327f85a2c7e`  
		Last Modified: Wed, 17 Nov 2021 13:40:24 GMT  
		Size: 10.2 MB (10216788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61401ffc70123532d1f4886b9ebd00e11d1155a2363117bf5aab10353c373dc9`  
		Last Modified: Wed, 17 Nov 2021 13:40:23 GMT  
		Size: 3.9 MB (3873891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185eee4daee1ed1fa34e853c2332cc4253415d7e015143b2432a96047c88d828`  
		Last Modified: Wed, 17 Nov 2021 13:40:43 GMT  
		Size: 47.7 MB (47734854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:3dd7dfec75397dae002735d04557b86aaaf641dbf609cd11f267f7740392d841
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.3 MB (113285816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10424f2f9fa56c237f5a1cb67f32e5286a03841b408bf07e8c6d4f87b5757030`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:42:19 GMT
ADD file:5a6f08cc731f24357c3702231256fb05eb0a97733779b2ace406ba3c9bf64baa in / 
# Tue, 12 Oct 2021 01:42:19 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:42:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:42:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 04:43:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d2ef4e90cca7406b4907a34e3571153fc56e3ecc9b2b5fdbb7787f22877cfec5`  
		Last Modified: Tue, 12 Oct 2021 01:51:58 GMT  
		Size: 46.1 MB (46097164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9020db84c7cf31b7929c21a2b6fe2123900e91c7391ad6f4ee5560a934f382`  
		Last Modified: Tue, 12 Oct 2021 04:52:49 GMT  
		Size: 11.4 MB (11358857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8cbe9196a8b6bd3825445c718bc5a248b7c295b4d9f45756819e8bf27cb72b`  
		Last Modified: Tue, 12 Oct 2021 04:52:47 GMT  
		Size: 4.6 MB (4565012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7454f0fe0ebf5d024897d682d46181ab978a980f7f40caa2492a83cc39f75ec`  
		Last Modified: Tue, 12 Oct 2021 04:53:20 GMT  
		Size: 51.3 MB (51264783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:unstable`

```console
$ docker pull buildpack-deps@sha256:b11103e6002f002f86e02cb10b9cef8b4a2cf90715e61d7cf395454bb089662e
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
$ docker pull buildpack-deps@sha256:de2c4024f4b15d8d4c980231c950776d5a75d15255ac95ebf4d7fc164fd26cc5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **492.2 MB (492225831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54138805f9191923bd18fae65421f211dad9ebf7d18c4e55fc9f640874f0b585`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:21:50 GMT
ADD file:1f62518cec36eb3320e38344c0d36779557214cfce8bc32eda000183a34a0ffa in / 
# Wed, 17 Nov 2021 02:21:51 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:17:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:17:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:18:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fef5443775fe054990b02e8f72c4c5bc7792c6a5bf6ef8df110873a81676a87`  
		Last Modified: Wed, 17 Nov 2021 02:28:03 GMT  
		Size: 55.8 MB (55758091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b63aa91be04004e56a4d31d70c789eadabfebe392e2f76a862eaa2fdd70dcfd`  
		Last Modified: Wed, 17 Nov 2021 03:25:48 GMT  
		Size: 5.3 MB (5269763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f625d605a0450d800b57ca6e2e0662fba5094348ccbf581c053a485802ebe1`  
		Last Modified: Wed, 17 Nov 2021 03:25:49 GMT  
		Size: 11.8 MB (11756478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f0dd71d7f2f690f062de61d743dd487108ccd38089c95218a295206a6c68c3`  
		Last Modified: Wed, 17 Nov 2021 03:26:09 GMT  
		Size: 55.9 MB (55936130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3929219b522d034efb90c4bdfcc3dc832476eea68565e8fdd758c5302b0766c2`  
		Last Modified: Wed, 17 Nov 2021 03:27:15 GMT  
		Size: 363.5 MB (363505369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:215a46aa6f638cf9e220fab73f63e86e8bfab8c61cfd70685dbda87356f34fa8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **474.9 MB (474871327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd2a73342dfad8a3515950c7aab1d759d8165ed5f42f656523b75f8e7b6ef43a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 00:53:53 GMT
ADD file:2918872df07d47b9a7862abf3b22f39600ab45587fcd02466bdefa775a3fc2dd in / 
# Tue, 12 Oct 2021 00:53:54 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:49:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:49:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 05:50:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:53:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8f73c109c91bd2f18faab4d6862ba33d940956d6457aaaaeeda5e8f72281edcc`  
		Last Modified: Tue, 12 Oct 2021 01:11:00 GMT  
		Size: 53.2 MB (53186352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd99c7b364b1329f3fc27bcb8d50810c30d8a7928b7518c93f2d538a1124daa0`  
		Last Modified: Tue, 12 Oct 2021 06:07:28 GMT  
		Size: 5.1 MB (5122384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8779df359e844ab400aaeab5d2001cf6d805ff10af17660fd4577296ecbf7f9`  
		Last Modified: Tue, 12 Oct 2021 06:07:30 GMT  
		Size: 10.6 MB (10606788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83014d4ab58f54e38e974b2de48f1a41a6bee268a7b6ebb1050582b1d782db1b`  
		Last Modified: Tue, 12 Oct 2021 06:08:20 GMT  
		Size: 53.4 MB (53442505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af54fd52817c8dff8e7fb1fb4b62845da3ed7da902c46ad93c9210945460647`  
		Last Modified: Tue, 12 Oct 2021 06:11:57 GMT  
		Size: 352.5 MB (352513298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:0e27ca88aaec10d98a1a69d635898d0de8d28f06ef64c3e111940e973d556ea0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **447.4 MB (447442275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2068124a06286aeecf9bb8a71ec407a13f888636b5b5030a394286b666e0f17d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:03:10 GMT
ADD file:df29fec66c741f67158d8ed2094810758d4a7cfb2c7cba3dbe60e5bc11ed824a in / 
# Wed, 17 Nov 2021 02:03:11 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:49:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:49:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 02:50:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:53:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:339de498e0e3324e5657ae3bd0868b26e4518664b7405a1fb321434233c56211`  
		Last Modified: Wed, 17 Nov 2021 02:19:45 GMT  
		Size: 50.9 MB (50860308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b9096006210de2acfc2854bd14870e0046c7c41610d75f402e14c7fa186a10`  
		Last Modified: Wed, 17 Nov 2021 03:10:01 GMT  
		Size: 5.0 MB (5029921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8864516b2a87655fdd355f203892d84f29fb0f553f371f37e7027ceb5017ec34`  
		Last Modified: Wed, 17 Nov 2021 03:10:03 GMT  
		Size: 11.1 MB (11067071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e207fc56e058029a1aa1e0cae4ac127bfa621c4e822edde8fdad43037978ac`  
		Last Modified: Wed, 17 Nov 2021 03:10:51 GMT  
		Size: 51.6 MB (51586431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31acdea0339066b9fdb9e8d5b74ff20f7ec64f9c62a7bf2ae54f21f2d6f1dcdb`  
		Last Modified: Wed, 17 Nov 2021 03:14:06 GMT  
		Size: 328.9 MB (328898544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c5e577cbb626d2867b19ce7ce967421f0665abf3c9cdb76e1574bff2ae26e9f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.7 MB (484718199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cb63aed3f12bbd933a07cf611eb991b7dec3ec3d9008ec829ec5ec30aa40b74`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:41:46 GMT
ADD file:6547698ce9c0dce5d390e739342bd015a0c3266dba4ef5828dc1b1a9eb46e826 in / 
# Wed, 17 Nov 2021 02:41:47 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:29:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:29:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:30:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:31:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:67eeb578521bba47ceed6d5c2de23409a33ec3c1c6fda03d83e22d74dc1cdb76`  
		Last Modified: Wed, 17 Nov 2021 02:49:53 GMT  
		Size: 54.8 MB (54767045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f777f34bfc0463ddee51fc9ba3a1f668f6072f8431123ab0571266c60fb89c`  
		Last Modified: Wed, 17 Nov 2021 13:38:51 GMT  
		Size: 5.3 MB (5253448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e720a8fffb7aadf0b926dc4c5b3d7cb21c21c6ec5e507ddcdb546f5483b5a44e`  
		Last Modified: Wed, 17 Nov 2021 13:38:52 GMT  
		Size: 11.5 MB (11525452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cab4dc0eb95cf2e9a2e2a5f77eca7d76108730f09e1e205c09465b4fa35934`  
		Last Modified: Wed, 17 Nov 2021 13:39:12 GMT  
		Size: 56.0 MB (55987448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c004de456b5e733bd6cf254df397e043de9b362c370460e313ed02fe89d4de81`  
		Last Modified: Wed, 17 Nov 2021 13:40:11 GMT  
		Size: 357.2 MB (357184806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:4ea2edd31669732d12dce321d6928127ffbe9073c24d96085b9ca44c2933bfab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.4 MB (332367435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea23a81b9c83e610134b648dd92aba29502de7ae1aa419876e7ab76976e253a2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:27 GMT
ADD file:9ab0c16547aac0a32292246b35737ca5260c5942d5e26ca1381be39c9e321ee5 in / 
# Tue, 12 Oct 2021 01:41:27 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:40:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:40:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 04:40:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:42:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c36fe1aa4217cf0326227a0bdcadc16e85d2670bd6485518167903dfc6934c65`  
		Last Modified: Tue, 12 Oct 2021 01:50:33 GMT  
		Size: 56.7 MB (56716103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1cefa3abf3c8d9687bfe164fbd73be6245f1e0c523603077cfcffd5881a3778`  
		Last Modified: Tue, 12 Oct 2021 04:51:12 GMT  
		Size: 5.3 MB (5346244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902f94685b9ef6228bbe2d7c552fb6d02ea5e723469df5c9e980d102fd9c6aa2`  
		Last Modified: Tue, 12 Oct 2021 04:51:13 GMT  
		Size: 11.3 MB (11281973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802e1fd067f1198f877ff5bc97afd5870c21a28609a1919a09063ff8aacf5fd4`  
		Last Modified: Tue, 12 Oct 2021 04:51:37 GMT  
		Size: 57.2 MB (57159249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ecb28b33acfca8e5784c5c3b85c0efb3eeb8d08971fe4e1e1dee2cc768ee8d`  
		Last Modified: Tue, 12 Oct 2021 04:52:26 GMT  
		Size: 201.9 MB (201863866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:d85ae18394cee324adf13254d7ec82ba0f2b66e532a1b07e1bf9ce1bade8da76
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **549.8 MB (549780160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a665b5eab25ab4ed0aaf7891e0b735ee8cabe629675356cb418ecd9a7771755c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:12:23 GMT
ADD file:9e3985f5064204cf4c74f2d464977349398f8e0325083d223b22ace99f5dfa3a in / 
# Wed, 17 Nov 2021 02:12:24 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:39:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:39:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 08:41:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:45:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b79f1dde26df3dbfdaf094cc43f4dc602b492e9dd707f7a7874e1366808028c5`  
		Last Modified: Wed, 17 Nov 2021 02:22:36 GMT  
		Size: 54.4 MB (54365459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c0e1963482abb9ea5592b86c11c6528aebf6fe675fd25fdeb440cd4f999043`  
		Last Modified: Wed, 17 Nov 2021 08:52:05 GMT  
		Size: 5.2 MB (5227764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0761e303fe4f33cd92c7d2d5ce49857285721fb135e5bf569abf4ec59745f3d`  
		Last Modified: Wed, 17 Nov 2021 08:52:07 GMT  
		Size: 11.8 MB (11755031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c476b323dda6fd93fbb86e98139e76c07bff3f2d7a4b07b087d8e2c114b346f2`  
		Last Modified: Wed, 17 Nov 2021 08:52:57 GMT  
		Size: 54.7 MB (54724326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea5b4a56a5596c25bbe127b531db840714709450c79dc686fb6cadb3ca56d6b`  
		Last Modified: Wed, 17 Nov 2021 08:57:22 GMT  
		Size: 423.7 MB (423707580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:a36f7bd93877cf70c960b650bc009777ba9a4e1a8a4c54e2a062ea7543d6e6e3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **490.1 MB (490107816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c48763889dcaa835be669cbc061b277dce92e01b77549cf143c08d77b60c8d15`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 03:32:54 GMT
ADD file:33bc17dd3e3b6cd8c5ac37c8382a5d2b8e3ee8384b598b69b0d17b813dcfc767 in / 
# Wed, 17 Nov 2021 03:33:15 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:07:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:08:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 08:11:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:23:09 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:60fa303f933c621481dd7a32f72de0e35b85a3567ff116516725c45089e1cb88`  
		Last Modified: Wed, 17 Nov 2021 04:05:01 GMT  
		Size: 60.0 MB (60045015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a3dd48191daf1a5544d8a3146aececcefc7d4f8fe8e7e64e723022de0e5bae`  
		Last Modified: Wed, 17 Nov 2021 08:31:39 GMT  
		Size: 5.5 MB (5531621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147c14b8f9e107cd759a99e83c419ee5c8c99e500d16d4bbbfdb94cf6126b724`  
		Last Modified: Wed, 17 Nov 2021 08:31:39 GMT  
		Size: 12.6 MB (12551297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16114ff6b100453ae456bca4961ed144a5cd72589c05128a5b44f063feab7bb`  
		Last Modified: Wed, 17 Nov 2021 08:32:21 GMT  
		Size: 60.4 MB (60400057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e03566f3ff76ccaf4843d621b4de9ff1a4ee9e74293314b7c986934b6be759d`  
		Last Modified: Wed, 17 Nov 2021 08:33:58 GMT  
		Size: 351.6 MB (351579826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:7ab7d4a74146b5374310fdaf408c2b278bcc7b29f972af025baebb48315f3c0b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343151630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70b618750b60d86f44a77d1d23690393cf206bada324151d86c6a22e64af1c7c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:14:24 GMT
ADD file:9ce8adafd95fc1e31db924edf473abf22a68101cad20cd078c35db5fa719b34b in / 
# Wed, 17 Nov 2021 02:14:27 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:56:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:58:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:02:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:11:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a35675c997377ee8bf94b0a94460a6d2fd72a26b5c7fc6194b13ae99da869125`  
		Last Modified: Wed, 17 Nov 2021 02:30:42 GMT  
		Size: 51.5 MB (51522304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6561ec3264f30875424c0937b41795ce70f58306ddfe766af2fcb7d266b6a6`  
		Last Modified: Wed, 17 Nov 2021 03:35:29 GMT  
		Size: 5.1 MB (5080232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f12be064689662dab642f65c8e821186c7247cf7ea84901a22b9e2584d51ee`  
		Last Modified: Wed, 17 Nov 2021 03:35:32 GMT  
		Size: 11.1 MB (11140508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077cd6f4305eeccad12d3a65baeff88b63dd35ab2735a8b6ca9d8f523e0b6a0a`  
		Last Modified: Wed, 17 Nov 2021 03:37:41 GMT  
		Size: 52.0 MB (52047230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3022710ce0174de31ed5f93fad3d58e7093927e84afdebfe2ee1e4a0bf48a54`  
		Last Modified: Wed, 17 Nov 2021 03:43:51 GMT  
		Size: 223.4 MB (223361356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:01443347d94c5d12c4c092d73f4e8954a0534604ba46a76e51e266d41e1adee0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **445.9 MB (445921270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef208aa2298803038eb573bf20ffc382beb5cb388e6ce838fd0cb92765f14a07`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:43:42 GMT
ADD file:ba3a56dbd46c1324142a33ad1eefa66c34fda8c9c635140debf01131cb259e63 in / 
# Wed, 17 Nov 2021 02:43:45 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:11:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:12:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:12:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:13:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3595b50e30d7d0d412c142596638dbf5abfc27f196fe5d138ded04b66fd2b50e`  
		Last Modified: Wed, 17 Nov 2021 02:49:48 GMT  
		Size: 54.0 MB (53965664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634664d8b893813a04761069646d85aea7164717481b8c7e3f500e4260fc39ee`  
		Last Modified: Wed, 17 Nov 2021 03:19:03 GMT  
		Size: 5.2 MB (5248300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1780c6b7bcc6484f6ae6602c37ffd3bb2c9aad27b1b2587b796a5824e8b6575`  
		Last Modified: Wed, 17 Nov 2021 03:19:03 GMT  
		Size: 11.6 MB (11647079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a6bd04c7a7df4cb7de2e064bcfa156db3e89664ab5448cf33cf12043705f4f5`  
		Last Modified: Wed, 17 Nov 2021 03:19:17 GMT  
		Size: 55.3 MB (55308755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d56ccdfeb3f75ba623e571ad85ef9c45f32b1e527abc14d9e5164dca7dbd76`  
		Last Modified: Wed, 17 Nov 2021 03:19:59 GMT  
		Size: 319.8 MB (319751472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:unstable-curl`

```console
$ docker pull buildpack-deps@sha256:bfffe4a3acc134d001cdcf237d588a1e9caebafd5707bd0b9d392800a322b926
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
$ docker pull buildpack-deps@sha256:19dfc5e7628b593c8056b31cbe197a24fffbe1d35a9b17adfd2f59a34641a4d8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.8 MB (72784332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07490f1b8ba2320e2026f3266933346b545ee1a5e75319a686e3575bac5b7f55`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:21:50 GMT
ADD file:1f62518cec36eb3320e38344c0d36779557214cfce8bc32eda000183a34a0ffa in / 
# Wed, 17 Nov 2021 02:21:51 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:17:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:17:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0fef5443775fe054990b02e8f72c4c5bc7792c6a5bf6ef8df110873a81676a87`  
		Last Modified: Wed, 17 Nov 2021 02:28:03 GMT  
		Size: 55.8 MB (55758091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b63aa91be04004e56a4d31d70c789eadabfebe392e2f76a862eaa2fdd70dcfd`  
		Last Modified: Wed, 17 Nov 2021 03:25:48 GMT  
		Size: 5.3 MB (5269763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f625d605a0450d800b57ca6e2e0662fba5094348ccbf581c053a485802ebe1`  
		Last Modified: Wed, 17 Nov 2021 03:25:49 GMT  
		Size: 11.8 MB (11756478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:93a96196f940f2470a5f63e45ed1eea93d39f49454b3461ce4f86003f32e88b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68915524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0426cef40090f80992e6f69498065959d6e618dd140a8a21341a317c7ce7f274`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 00:53:53 GMT
ADD file:2918872df07d47b9a7862abf3b22f39600ab45587fcd02466bdefa775a3fc2dd in / 
# Tue, 12 Oct 2021 00:53:54 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:49:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:49:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8f73c109c91bd2f18faab4d6862ba33d940956d6457aaaaeeda5e8f72281edcc`  
		Last Modified: Tue, 12 Oct 2021 01:11:00 GMT  
		Size: 53.2 MB (53186352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd99c7b364b1329f3fc27bcb8d50810c30d8a7928b7518c93f2d538a1124daa0`  
		Last Modified: Tue, 12 Oct 2021 06:07:28 GMT  
		Size: 5.1 MB (5122384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8779df359e844ab400aaeab5d2001cf6d805ff10af17660fd4577296ecbf7f9`  
		Last Modified: Tue, 12 Oct 2021 06:07:30 GMT  
		Size: 10.6 MB (10606788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:67b214acbcd9f9a68874338a7751ff7c36fbfaf55bf4c8085992ae1d47249822
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (66957300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17a529394265f7fd2fbce68d31a42a78128feabb2a05da15f6db6613f9a9f76d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:03:10 GMT
ADD file:df29fec66c741f67158d8ed2094810758d4a7cfb2c7cba3dbe60e5bc11ed824a in / 
# Wed, 17 Nov 2021 02:03:11 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:49:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:49:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:339de498e0e3324e5657ae3bd0868b26e4518664b7405a1fb321434233c56211`  
		Last Modified: Wed, 17 Nov 2021 02:19:45 GMT  
		Size: 50.9 MB (50860308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b9096006210de2acfc2854bd14870e0046c7c41610d75f402e14c7fa186a10`  
		Last Modified: Wed, 17 Nov 2021 03:10:01 GMT  
		Size: 5.0 MB (5029921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8864516b2a87655fdd355f203892d84f29fb0f553f371f37e7027ceb5017ec34`  
		Last Modified: Wed, 17 Nov 2021 03:10:03 GMT  
		Size: 11.1 MB (11067071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:739c39731b3c78675e5b07d31cfd783cbcaa98f52bcd3e90fcd44c9a307e6676
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.5 MB (71545945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a03eacbbae2823342ae5c042212eaa4d8a7fd2b691788aca661c794de4be92dd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:41:46 GMT
ADD file:6547698ce9c0dce5d390e739342bd015a0c3266dba4ef5828dc1b1a9eb46e826 in / 
# Wed, 17 Nov 2021 02:41:47 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:29:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:29:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:67eeb578521bba47ceed6d5c2de23409a33ec3c1c6fda03d83e22d74dc1cdb76`  
		Last Modified: Wed, 17 Nov 2021 02:49:53 GMT  
		Size: 54.8 MB (54767045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f777f34bfc0463ddee51fc9ba3a1f668f6072f8431123ab0571266c60fb89c`  
		Last Modified: Wed, 17 Nov 2021 13:38:51 GMT  
		Size: 5.3 MB (5253448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e720a8fffb7aadf0b926dc4c5b3d7cb21c21c6ec5e507ddcdb546f5483b5a44e`  
		Last Modified: Wed, 17 Nov 2021 13:38:52 GMT  
		Size: 11.5 MB (11525452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:4dd56a29db23efb893ab16850832733df3813b7a11f292dee71fd5094fd58a3c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.3 MB (73344320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:962d74b000a7400b45ea570dcd0f3351f2de7987db6d7cbd3225992e396a156d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:27 GMT
ADD file:9ab0c16547aac0a32292246b35737ca5260c5942d5e26ca1381be39c9e321ee5 in / 
# Tue, 12 Oct 2021 01:41:27 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:40:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:40:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c36fe1aa4217cf0326227a0bdcadc16e85d2670bd6485518167903dfc6934c65`  
		Last Modified: Tue, 12 Oct 2021 01:50:33 GMT  
		Size: 56.7 MB (56716103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1cefa3abf3c8d9687bfe164fbd73be6245f1e0c523603077cfcffd5881a3778`  
		Last Modified: Tue, 12 Oct 2021 04:51:12 GMT  
		Size: 5.3 MB (5346244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902f94685b9ef6228bbe2d7c552fb6d02ea5e723469df5c9e980d102fd9c6aa2`  
		Last Modified: Tue, 12 Oct 2021 04:51:13 GMT  
		Size: 11.3 MB (11281973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:7cb7cefc9fa6132910698c9133093c1f9b92416218f2ee05824d1bd3c04bf7af
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71348254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c188c28686d73282c6cc150448e2c28b123c0faf48b12f0c6ba204562bd511d0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:12:23 GMT
ADD file:9e3985f5064204cf4c74f2d464977349398f8e0325083d223b22ace99f5dfa3a in / 
# Wed, 17 Nov 2021 02:12:24 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:39:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:39:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b79f1dde26df3dbfdaf094cc43f4dc602b492e9dd707f7a7874e1366808028c5`  
		Last Modified: Wed, 17 Nov 2021 02:22:36 GMT  
		Size: 54.4 MB (54365459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c0e1963482abb9ea5592b86c11c6528aebf6fe675fd25fdeb440cd4f999043`  
		Last Modified: Wed, 17 Nov 2021 08:52:05 GMT  
		Size: 5.2 MB (5227764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0761e303fe4f33cd92c7d2d5ce49857285721fb135e5bf569abf4ec59745f3d`  
		Last Modified: Wed, 17 Nov 2021 08:52:07 GMT  
		Size: 11.8 MB (11755031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:b66398bb06582e08079239ae0b55efcdaa4a6ce35f62aef40ad59f2066a751a1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.1 MB (78127933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4909eb043acba9dfc8f6ced1c81d8f31d080bf218205bcff6428112c4bbfecd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 03:32:54 GMT
ADD file:33bc17dd3e3b6cd8c5ac37c8382a5d2b8e3ee8384b598b69b0d17b813dcfc767 in / 
# Wed, 17 Nov 2021 03:33:15 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:07:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:08:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:60fa303f933c621481dd7a32f72de0e35b85a3567ff116516725c45089e1cb88`  
		Last Modified: Wed, 17 Nov 2021 04:05:01 GMT  
		Size: 60.0 MB (60045015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a3dd48191daf1a5544d8a3146aececcefc7d4f8fe8e7e64e723022de0e5bae`  
		Last Modified: Wed, 17 Nov 2021 08:31:39 GMT  
		Size: 5.5 MB (5531621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147c14b8f9e107cd759a99e83c419ee5c8c99e500d16d4bbbfdb94cf6126b724`  
		Last Modified: Wed, 17 Nov 2021 08:31:39 GMT  
		Size: 12.6 MB (12551297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:c56a5966672afb0d47c167ad7358e0979cd24aef6efa756a7d6814b137b647df
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67743044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c2ef8905089a0b83a3817c763b00709bc4c9c53504e843a8e09c10005a148e6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:14:24 GMT
ADD file:9ce8adafd95fc1e31db924edf473abf22a68101cad20cd078c35db5fa719b34b in / 
# Wed, 17 Nov 2021 02:14:27 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:56:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:58:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a35675c997377ee8bf94b0a94460a6d2fd72a26b5c7fc6194b13ae99da869125`  
		Last Modified: Wed, 17 Nov 2021 02:30:42 GMT  
		Size: 51.5 MB (51522304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6561ec3264f30875424c0937b41795ce70f58306ddfe766af2fcb7d266b6a6`  
		Last Modified: Wed, 17 Nov 2021 03:35:29 GMT  
		Size: 5.1 MB (5080232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f12be064689662dab642f65c8e821186c7247cf7ea84901a22b9e2584d51ee`  
		Last Modified: Wed, 17 Nov 2021 03:35:32 GMT  
		Size: 11.1 MB (11140508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:40088f08cf065fbc90807be108a7a28a69ba5cf9a42b702be39a8c7e51925ab5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.9 MB (70861043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab27d0591464195b772d890535dec1c22fe3a85b97d9aff1dbb6f656574b113c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:43:42 GMT
ADD file:ba3a56dbd46c1324142a33ad1eefa66c34fda8c9c635140debf01131cb259e63 in / 
# Wed, 17 Nov 2021 02:43:45 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:11:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:12:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3595b50e30d7d0d412c142596638dbf5abfc27f196fe5d138ded04b66fd2b50e`  
		Last Modified: Wed, 17 Nov 2021 02:49:48 GMT  
		Size: 54.0 MB (53965664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634664d8b893813a04761069646d85aea7164717481b8c7e3f500e4260fc39ee`  
		Last Modified: Wed, 17 Nov 2021 03:19:03 GMT  
		Size: 5.2 MB (5248300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1780c6b7bcc6484f6ae6602c37ffd3bb2c9aad27b1b2587b796a5824e8b6575`  
		Last Modified: Wed, 17 Nov 2021 03:19:03 GMT  
		Size: 11.6 MB (11647079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:unstable-scm`

```console
$ docker pull buildpack-deps@sha256:df709a87f131d005c85caf81955466cc7b0448e415eddbf201b4afadb88dce0f
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
$ docker pull buildpack-deps@sha256:62c202ce5cf8cf05bcb2ba5a873e1590fb65fadeeb82a6c0909b7dc0585d74f8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128720462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c577bace026f3ec0ecea3874f32bad4f5b02436f6da5fe8a140ca47b896691f4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:21:50 GMT
ADD file:1f62518cec36eb3320e38344c0d36779557214cfce8bc32eda000183a34a0ffa in / 
# Wed, 17 Nov 2021 02:21:51 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:17:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:17:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:18:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fef5443775fe054990b02e8f72c4c5bc7792c6a5bf6ef8df110873a81676a87`  
		Last Modified: Wed, 17 Nov 2021 02:28:03 GMT  
		Size: 55.8 MB (55758091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b63aa91be04004e56a4d31d70c789eadabfebe392e2f76a862eaa2fdd70dcfd`  
		Last Modified: Wed, 17 Nov 2021 03:25:48 GMT  
		Size: 5.3 MB (5269763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f625d605a0450d800b57ca6e2e0662fba5094348ccbf581c053a485802ebe1`  
		Last Modified: Wed, 17 Nov 2021 03:25:49 GMT  
		Size: 11.8 MB (11756478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f0dd71d7f2f690f062de61d743dd487108ccd38089c95218a295206a6c68c3`  
		Last Modified: Wed, 17 Nov 2021 03:26:09 GMT  
		Size: 55.9 MB (55936130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:a6fd6b6ff59a9e3a097d8125f6ca8b78882f804f0ca5bec557784676e4d379a3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.4 MB (122358029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33b4f3e109e84ef325b2927539c9c569367e50198086ed8d72be40ef36742c34`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 00:53:53 GMT
ADD file:2918872df07d47b9a7862abf3b22f39600ab45587fcd02466bdefa775a3fc2dd in / 
# Tue, 12 Oct 2021 00:53:54 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:49:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:49:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 05:50:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8f73c109c91bd2f18faab4d6862ba33d940956d6457aaaaeeda5e8f72281edcc`  
		Last Modified: Tue, 12 Oct 2021 01:11:00 GMT  
		Size: 53.2 MB (53186352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd99c7b364b1329f3fc27bcb8d50810c30d8a7928b7518c93f2d538a1124daa0`  
		Last Modified: Tue, 12 Oct 2021 06:07:28 GMT  
		Size: 5.1 MB (5122384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8779df359e844ab400aaeab5d2001cf6d805ff10af17660fd4577296ecbf7f9`  
		Last Modified: Tue, 12 Oct 2021 06:07:30 GMT  
		Size: 10.6 MB (10606788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83014d4ab58f54e38e974b2de48f1a41a6bee268a7b6ebb1050582b1d782db1b`  
		Last Modified: Tue, 12 Oct 2021 06:08:20 GMT  
		Size: 53.4 MB (53442505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:e25517d9e4d5c71b0fd71f8672be17b1407629cf364b7b4c875a48dd1572d1d9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.5 MB (118543731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b22e7df05fd0bffeca4c0755b5570159b2a6f9ae77bca4317c40c4257b7e6e1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:03:10 GMT
ADD file:df29fec66c741f67158d8ed2094810758d4a7cfb2c7cba3dbe60e5bc11ed824a in / 
# Wed, 17 Nov 2021 02:03:11 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:49:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:49:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 02:50:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:339de498e0e3324e5657ae3bd0868b26e4518664b7405a1fb321434233c56211`  
		Last Modified: Wed, 17 Nov 2021 02:19:45 GMT  
		Size: 50.9 MB (50860308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b9096006210de2acfc2854bd14870e0046c7c41610d75f402e14c7fa186a10`  
		Last Modified: Wed, 17 Nov 2021 03:10:01 GMT  
		Size: 5.0 MB (5029921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8864516b2a87655fdd355f203892d84f29fb0f553f371f37e7027ceb5017ec34`  
		Last Modified: Wed, 17 Nov 2021 03:10:03 GMT  
		Size: 11.1 MB (11067071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e207fc56e058029a1aa1e0cae4ac127bfa621c4e822edde8fdad43037978ac`  
		Last Modified: Wed, 17 Nov 2021 03:10:51 GMT  
		Size: 51.6 MB (51586431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3057f63e28cc1fe4f0dd11039577f14ac057f713e42e2b2e13000b37b8b86967
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127533393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4bbe255f47709b63ebef085398bae156c616dc66fa9f1980c105e345911141a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:41:46 GMT
ADD file:6547698ce9c0dce5d390e739342bd015a0c3266dba4ef5828dc1b1a9eb46e826 in / 
# Wed, 17 Nov 2021 02:41:47 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:29:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:29:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:30:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:67eeb578521bba47ceed6d5c2de23409a33ec3c1c6fda03d83e22d74dc1cdb76`  
		Last Modified: Wed, 17 Nov 2021 02:49:53 GMT  
		Size: 54.8 MB (54767045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f777f34bfc0463ddee51fc9ba3a1f668f6072f8431123ab0571266c60fb89c`  
		Last Modified: Wed, 17 Nov 2021 13:38:51 GMT  
		Size: 5.3 MB (5253448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e720a8fffb7aadf0b926dc4c5b3d7cb21c21c6ec5e507ddcdb546f5483b5a44e`  
		Last Modified: Wed, 17 Nov 2021 13:38:52 GMT  
		Size: 11.5 MB (11525452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cab4dc0eb95cf2e9a2e2a5f77eca7d76108730f09e1e205c09465b4fa35934`  
		Last Modified: Wed, 17 Nov 2021 13:39:12 GMT  
		Size: 56.0 MB (55987448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:733772bac49de30e8a05b0ad0e7d0340e5b5089313a4dfdb7f57a6d60552b79c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.5 MB (130503569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41174274a4fa2d6806ed55fabbfd91e97b22e8a8178e2412b0e819bceda895d8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:27 GMT
ADD file:9ab0c16547aac0a32292246b35737ca5260c5942d5e26ca1381be39c9e321ee5 in / 
# Tue, 12 Oct 2021 01:41:27 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:40:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:40:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 04:40:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c36fe1aa4217cf0326227a0bdcadc16e85d2670bd6485518167903dfc6934c65`  
		Last Modified: Tue, 12 Oct 2021 01:50:33 GMT  
		Size: 56.7 MB (56716103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1cefa3abf3c8d9687bfe164fbd73be6245f1e0c523603077cfcffd5881a3778`  
		Last Modified: Tue, 12 Oct 2021 04:51:12 GMT  
		Size: 5.3 MB (5346244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902f94685b9ef6228bbe2d7c552fb6d02ea5e723469df5c9e980d102fd9c6aa2`  
		Last Modified: Tue, 12 Oct 2021 04:51:13 GMT  
		Size: 11.3 MB (11281973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802e1fd067f1198f877ff5bc97afd5870c21a28609a1919a09063ff8aacf5fd4`  
		Last Modified: Tue, 12 Oct 2021 04:51:37 GMT  
		Size: 57.2 MB (57159249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:277451baec3ac7c41ff286c5d4bf89c602eb089f8ec4b24e96281dac4cea121f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.1 MB (126072580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48b49a0d880ec3185395fff15df7416540f343c3c377be897de3965fb23c1cfd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:12:23 GMT
ADD file:9e3985f5064204cf4c74f2d464977349398f8e0325083d223b22ace99f5dfa3a in / 
# Wed, 17 Nov 2021 02:12:24 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:39:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:39:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 08:41:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b79f1dde26df3dbfdaf094cc43f4dc602b492e9dd707f7a7874e1366808028c5`  
		Last Modified: Wed, 17 Nov 2021 02:22:36 GMT  
		Size: 54.4 MB (54365459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c0e1963482abb9ea5592b86c11c6528aebf6fe675fd25fdeb440cd4f999043`  
		Last Modified: Wed, 17 Nov 2021 08:52:05 GMT  
		Size: 5.2 MB (5227764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0761e303fe4f33cd92c7d2d5ce49857285721fb135e5bf569abf4ec59745f3d`  
		Last Modified: Wed, 17 Nov 2021 08:52:07 GMT  
		Size: 11.8 MB (11755031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c476b323dda6fd93fbb86e98139e76c07bff3f2d7a4b07b087d8e2c114b346f2`  
		Last Modified: Wed, 17 Nov 2021 08:52:57 GMT  
		Size: 54.7 MB (54724326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:8262acfa4cec540a727499b029781e6d9a768c80567ef0a550cc50eb38db0b5e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.5 MB (138527990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70616a1063b2854769c53da57f912b1b4adb02a65b34be74ac6b6749e1606f88`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 03:32:54 GMT
ADD file:33bc17dd3e3b6cd8c5ac37c8382a5d2b8e3ee8384b598b69b0d17b813dcfc767 in / 
# Wed, 17 Nov 2021 03:33:15 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:07:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:08:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 08:11:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:60fa303f933c621481dd7a32f72de0e35b85a3567ff116516725c45089e1cb88`  
		Last Modified: Wed, 17 Nov 2021 04:05:01 GMT  
		Size: 60.0 MB (60045015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a3dd48191daf1a5544d8a3146aececcefc7d4f8fe8e7e64e723022de0e5bae`  
		Last Modified: Wed, 17 Nov 2021 08:31:39 GMT  
		Size: 5.5 MB (5531621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147c14b8f9e107cd759a99e83c419ee5c8c99e500d16d4bbbfdb94cf6126b724`  
		Last Modified: Wed, 17 Nov 2021 08:31:39 GMT  
		Size: 12.6 MB (12551297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16114ff6b100453ae456bca4961ed144a5cd72589c05128a5b44f063feab7bb`  
		Last Modified: Wed, 17 Nov 2021 08:32:21 GMT  
		Size: 60.4 MB (60400057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:8486f624b42b956b1401a5bd240b03ad282ea1e54edb5242ea846893478a20ab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.8 MB (119790274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b441fc86b4e2662aeadd8e308872b18de076f1c73c976e045a69988dcff041e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:14:24 GMT
ADD file:9ce8adafd95fc1e31db924edf473abf22a68101cad20cd078c35db5fa719b34b in / 
# Wed, 17 Nov 2021 02:14:27 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:56:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:58:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:02:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a35675c997377ee8bf94b0a94460a6d2fd72a26b5c7fc6194b13ae99da869125`  
		Last Modified: Wed, 17 Nov 2021 02:30:42 GMT  
		Size: 51.5 MB (51522304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6561ec3264f30875424c0937b41795ce70f58306ddfe766af2fcb7d266b6a6`  
		Last Modified: Wed, 17 Nov 2021 03:35:29 GMT  
		Size: 5.1 MB (5080232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f12be064689662dab642f65c8e821186c7247cf7ea84901a22b9e2584d51ee`  
		Last Modified: Wed, 17 Nov 2021 03:35:32 GMT  
		Size: 11.1 MB (11140508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077cd6f4305eeccad12d3a65baeff88b63dd35ab2735a8b6ca9d8f523e0b6a0a`  
		Last Modified: Wed, 17 Nov 2021 03:37:41 GMT  
		Size: 52.0 MB (52047230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:8e5535d8b76c576ccc669d4f642fe2ed78be80df9778331222b1c87425845db7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.2 MB (126169798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6223c90d2c69ea15d0c2c6ca6033b860ee5f424c5d543919e86bc305d827047e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:43:42 GMT
ADD file:ba3a56dbd46c1324142a33ad1eefa66c34fda8c9c635140debf01131cb259e63 in / 
# Wed, 17 Nov 2021 02:43:45 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:11:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:12:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:12:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3595b50e30d7d0d412c142596638dbf5abfc27f196fe5d138ded04b66fd2b50e`  
		Last Modified: Wed, 17 Nov 2021 02:49:48 GMT  
		Size: 54.0 MB (53965664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634664d8b893813a04761069646d85aea7164717481b8c7e3f500e4260fc39ee`  
		Last Modified: Wed, 17 Nov 2021 03:19:03 GMT  
		Size: 5.2 MB (5248300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1780c6b7bcc6484f6ae6602c37ffd3bb2c9aad27b1b2587b796a5824e8b6575`  
		Last Modified: Wed, 17 Nov 2021 03:19:03 GMT  
		Size: 11.6 MB (11647079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a6bd04c7a7df4cb7de2e064bcfa156db3e89664ab5448cf33cf12043705f4f5`  
		Last Modified: Wed, 17 Nov 2021 03:19:17 GMT  
		Size: 55.3 MB (55308755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:xenial`

```console
$ docker pull buildpack-deps@sha256:ed8a3a685f4b0b8e377d4f8c8e1baa7963aea31ba5d2e97294fadaf63def04f0
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
$ docker pull buildpack-deps@sha256:29635a7ce106a6fb76fb04fb862890d50647ad6eccd38ba33456cf9d81c79522
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.0 MB (209962270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:902f82b2116fd21d8e7a7eab834541cd4467bc9f4b2531ff4b257dcf8717a3d8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:48:22 GMT
ADD file:3c6dc937cb7b4c81b42126f377d23320ec1d0a8ca34d38e7c45871f1d08dac43 in / 
# Sat, 16 Oct 2021 01:48:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 16 Oct 2021 01:48:23 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:48:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 16 Oct 2021 01:48:25 GMT
CMD ["/bin/bash"]
# Sat, 16 Oct 2021 03:11:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:11:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 03:11:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:12:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:828b35a09f0b2f3d1dead43aa2468ff5eba6c463423b3fff7ee6d150f6fd1b6b`  
		Last Modified: Thu, 05 Aug 2021 00:25:09 GMT  
		Size: 41.2 MB (41239253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238e9b8fdf46981043813ae269c4420735959dd01d4d15c420b66448523e9adc`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5b1b49195905e9415adfe3583301316ef591d794fcfd12b5cd29103fa7ee6b`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269a6c6175ba12a0fd708883c2625167711f111f24ce2bb79221fda132487e57`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77011f0e629af6f1792d3ccf59b89e6c06bb7f9a0f9ff78fee1d59ca55eda175`  
		Last Modified: Sat, 16 Oct 2021 03:24:02 GMT  
		Size: 6.8 MB (6837244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef3e23489d0258d8ea0afeec7d0eac6009020741bdee47ed1cae3fd5a9004fb`  
		Last Modified: Sat, 16 Oct 2021 03:24:19 GMT  
		Size: 39.8 MB (39815288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0884afca89907fa2ac7f34ac68afcbba8e0be0626d1bb3927c23cbd7cdd9c24`  
		Last Modified: Sat, 16 Oct 2021 03:24:47 GMT  
		Size: 122.1 MB (122068992 bytes)  
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
$ docker pull buildpack-deps@sha256:ea5020e4cda81416f5265e6ff8fb336e1a3b70637de0b68241217f64483b2cef
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
$ docker pull buildpack-deps@sha256:d7f4fe08183763a004061ab5bb9663ab2f51bf303b9be25d3a37d46e9bc4c744
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48077990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27605cc34c887f769b55b6bbaf4811f39a6448d2c48146d5c0ff53270d2a50f5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:48:22 GMT
ADD file:3c6dc937cb7b4c81b42126f377d23320ec1d0a8ca34d38e7c45871f1d08dac43 in / 
# Sat, 16 Oct 2021 01:48:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 16 Oct 2021 01:48:23 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:48:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 16 Oct 2021 01:48:25 GMT
CMD ["/bin/bash"]
# Sat, 16 Oct 2021 03:11:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:11:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:828b35a09f0b2f3d1dead43aa2468ff5eba6c463423b3fff7ee6d150f6fd1b6b`  
		Last Modified: Thu, 05 Aug 2021 00:25:09 GMT  
		Size: 41.2 MB (41239253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238e9b8fdf46981043813ae269c4420735959dd01d4d15c420b66448523e9adc`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5b1b49195905e9415adfe3583301316ef591d794fcfd12b5cd29103fa7ee6b`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269a6c6175ba12a0fd708883c2625167711f111f24ce2bb79221fda132487e57`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77011f0e629af6f1792d3ccf59b89e6c06bb7f9a0f9ff78fee1d59ca55eda175`  
		Last Modified: Sat, 16 Oct 2021 03:24:02 GMT  
		Size: 6.8 MB (6837244 bytes)  
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
$ docker pull buildpack-deps@sha256:7eb08b3466cf0830b1b16429f7a16f428f8441163debd766b8ffabcd3cfffac7
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
$ docker pull buildpack-deps@sha256:676194f83bf0884b02998c5e5783ba66882579a02a3da41de3a8180280f8f5d6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.9 MB (87893278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a849f28400387145666eead1018792c030ac71ad4445140201f4e6395aee9178`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:48:22 GMT
ADD file:3c6dc937cb7b4c81b42126f377d23320ec1d0a8ca34d38e7c45871f1d08dac43 in / 
# Sat, 16 Oct 2021 01:48:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 16 Oct 2021 01:48:23 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:48:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 16 Oct 2021 01:48:25 GMT
CMD ["/bin/bash"]
# Sat, 16 Oct 2021 03:11:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:11:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 03:11:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:828b35a09f0b2f3d1dead43aa2468ff5eba6c463423b3fff7ee6d150f6fd1b6b`  
		Last Modified: Thu, 05 Aug 2021 00:25:09 GMT  
		Size: 41.2 MB (41239253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238e9b8fdf46981043813ae269c4420735959dd01d4d15c420b66448523e9adc`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5b1b49195905e9415adfe3583301316ef591d794fcfd12b5cd29103fa7ee6b`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269a6c6175ba12a0fd708883c2625167711f111f24ce2bb79221fda132487e57`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77011f0e629af6f1792d3ccf59b89e6c06bb7f9a0f9ff78fee1d59ca55eda175`  
		Last Modified: Sat, 16 Oct 2021 03:24:02 GMT  
		Size: 6.8 MB (6837244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef3e23489d0258d8ea0afeec7d0eac6009020741bdee47ed1cae3fd5a9004fb`  
		Last Modified: Sat, 16 Oct 2021 03:24:19 GMT  
		Size: 39.8 MB (39815288 bytes)  
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
