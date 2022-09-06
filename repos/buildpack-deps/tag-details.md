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
-	[`buildpack-deps:22.04`](#buildpack-deps2204)
-	[`buildpack-deps:22.04-curl`](#buildpack-deps2204-curl)
-	[`buildpack-deps:22.04-scm`](#buildpack-deps2204-scm)
-	[`buildpack-deps:22.10`](#buildpack-deps2210)
-	[`buildpack-deps:22.10-curl`](#buildpack-deps2210-curl)
-	[`buildpack-deps:22.10-scm`](#buildpack-deps2210-scm)
-	[`buildpack-deps:bionic`](#buildpack-depsbionic)
-	[`buildpack-deps:bionic-curl`](#buildpack-depsbionic-curl)
-	[`buildpack-deps:bionic-scm`](#buildpack-depsbionic-scm)
-	[`buildpack-deps:bookworm`](#buildpack-depsbookworm)
-	[`buildpack-deps:bookworm-curl`](#buildpack-depsbookworm-curl)
-	[`buildpack-deps:bookworm-scm`](#buildpack-depsbookworm-scm)
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
-	[`buildpack-deps:jammy`](#buildpack-depsjammy)
-	[`buildpack-deps:jammy-curl`](#buildpack-depsjammy-curl)
-	[`buildpack-deps:jammy-scm`](#buildpack-depsjammy-scm)
-	[`buildpack-deps:kinetic`](#buildpack-depskinetic)
-	[`buildpack-deps:kinetic-curl`](#buildpack-depskinetic-curl)
-	[`buildpack-deps:kinetic-scm`](#buildpack-depskinetic-scm)
-	[`buildpack-deps:latest`](#buildpack-depslatest)
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
-	[`buildpack-deps:testing`](#buildpack-depstesting)
-	[`buildpack-deps:testing-curl`](#buildpack-depstesting-curl)
-	[`buildpack-deps:testing-scm`](#buildpack-depstesting-scm)
-	[`buildpack-deps:unstable`](#buildpack-depsunstable)
-	[`buildpack-deps:unstable-curl`](#buildpack-depsunstable-curl)
-	[`buildpack-deps:unstable-scm`](#buildpack-depsunstable-scm)
-	[`buildpack-deps:xenial`](#buildpack-depsxenial)
-	[`buildpack-deps:xenial-curl`](#buildpack-depsxenial-curl)
-	[`buildpack-deps:xenial-scm`](#buildpack-depsxenial-scm)

## `buildpack-deps:16.04`

```console
$ docker pull buildpack-deps@sha256:efffef05dadcc74834c6b4eb5c916ee03a62d315e1a38b0d52e2e442ac55d119
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
$ docker pull buildpack-deps@sha256:324cae93bc58f79fb9a0ce73a3f358bb214f120bf4b20b1605f4d363cd84e71c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.4 MB (202397646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f9369fe76ef4d2ec8e85f2b5f60d860dcaec95b99b6a95200bbc1bd1e4fed6d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:41:46 GMT
ADD file:294a94a081de785c730003a440a0530a85add2bcb60c0f5bc4ce7ee17867ac4e in / 
# Tue, 02 Aug 2022 01:41:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 02 Aug 2022 01:41:48 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:41:49 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 02 Aug 2022 01:41:49 GMT
CMD ["/bin/bash"]
# Tue, 02 Aug 2022 02:03:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 02:03:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 02:04:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 02:05:16 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b95ba076a26b98e98eac4b43596b59c20d1e61a36bcaf2afae3aeebadc8844cf`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 40.3 MB (40312250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c9df55506368eeeb59c5f56bf5d6f9ef4476a6b1e43154eebe32e436e60d7a`  
		Last Modified: Tue, 02 Aug 2022 01:44:42 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60aa30d82c4849b80da22554e0006d9c23c68a807fcb795b2f35ac6c02549eca`  
		Last Modified: Tue, 02 Aug 2022 01:44:42 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61b5d5a768deb5e021d74947bacf44422a006a3495d70395a7d745e07fab3f3`  
		Last Modified: Tue, 02 Aug 2022 01:44:42 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5302476a417ee0052e99816026f14bd6111e868aff0afed105038f5bf2c6ef`  
		Last Modified: Tue, 02 Aug 2022 02:19:12 GMT  
		Size: 6.6 MB (6631595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6ffa599dded0e2d5396a2e5b5cf1c7bef210b53ab5bc8863068549c1ce6bdd`  
		Last Modified: Tue, 02 Aug 2022 02:19:35 GMT  
		Size: 38.2 MB (38162222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c764bf569c904be4755c19d16f88022c4cf1f489d57580e028ade4294cca72`  
		Last Modified: Tue, 02 Aug 2022 02:20:14 GMT  
		Size: 117.3 MB (117290043 bytes)  
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
$ docker pull buildpack-deps@sha256:1e1e74caf2e0e8989c33f3170baddfc3ae848e6b26269fb543dc00053f8c6ec4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.5 MB (236450829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aeeafa7909c0b22a7bbacfb11c178ef12c0ca3d20420f976fa215dd87ccbf58f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:39:28 GMT
ADD file:a4ae521feddf8357667e9361bdd972a69ed945f3857cc8c534652592e432575d in / 
# Tue, 05 Apr 2022 22:39:29 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Apr 2022 22:39:30 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 22:39:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Apr 2022 22:39:32 GMT
CMD ["/bin/bash"]
# Tue, 05 Apr 2022 23:06:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:06:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 05 Apr 2022 23:07:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:09:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1335d7ebdbbb7325d434cf945bcb54cb20f7288e1ca2a1cf140ae02b324646e6`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 45.8 MB (45816182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa6a227af79fa98ebbd1d2da516e2b7ce1cea5519a760cd0f6688738fbdb951`  
		Last Modified: Tue, 05 Apr 2022 22:40:40 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3928723c2c34ecd7264ce4e195ddda11403213b1c93d02e8efcd11de4b07a1`  
		Last Modified: Tue, 05 Apr 2022 22:40:40 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e468001dd2f338d54f47d062d65db61c754f09897744d97084afa15cee021200`  
		Last Modified: Tue, 05 Apr 2022 22:40:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abf8b8634fb64c0b6634daaf98b0d89d01420d22a01f63010623587194cfc7c`  
		Last Modified: Tue, 05 Apr 2022 23:13:08 GMT  
		Size: 7.9 MB (7932551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6d144d968e58673ed441d100257197c971e98922fc325d2b9d2726c37b1669`  
		Last Modified: Tue, 05 Apr 2022 23:13:29 GMT  
		Size: 42.9 MB (42898142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86384a05f478f2b7db7a8e5697851efe9ced94315317560ef2f7b936575f407b`  
		Last Modified: Tue, 05 Apr 2022 23:13:57 GMT  
		Size: 139.8 MB (139802417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:16.04` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:bdf5504d8fad9d8f2637b7afa429d9008f8290629078eec62b30b79581cbab25
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.5 MB (245528509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b86fb1b9cf83165573abf6e47221fa430546b66ca9c4e2a7fbb9014405d52f66`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:32:03 GMT
ADD file:c84969ed4d4e336ec5996e26e35261f683b36f1af7a978df587296ef5e7a2627 in / 
# Tue, 02 Aug 2022 01:32:06 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 02 Aug 2022 01:32:07 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:32:08 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 02 Aug 2022 01:32:08 GMT
CMD ["/bin/bash"]
# Tue, 02 Aug 2022 03:04:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 03:05:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 03:06:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 03:09:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5057452c10cfe2216f39949f909f3cd83002d256d1bbd564ae242352a5460fe2`  
		Last Modified: Sun, 08 Aug 2021 01:00:30 GMT  
		Size: 47.5 MB (47522137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72bced789eccb5759f541a5b15b9a3031c06cc54bdbff1a553cc0ef29ddad2bc`  
		Last Modified: Tue, 02 Aug 2022 01:36:22 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11a61259761ffe18601a628413443ccb5dee06a185a81c902220dfc070801c3`  
		Last Modified: Tue, 02 Aug 2022 01:35:56 GMT  
		Size: 483.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3272460dff18ff8fd96d33337b0ff5cc5d9d2e7f158c662273e1bb760c7f9722`  
		Last Modified: Tue, 02 Aug 2022 01:36:06 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65fd76771481bd61ed3539bc027b95c72e82ceebe357d2d960463332e3348c73`  
		Last Modified: Tue, 02 Aug 2022 03:26:11 GMT  
		Size: 7.7 MB (7693686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6157fa0cdd9af85bd373614103144ea737420e95c79b68ad61350c0104479e7`  
		Last Modified: Tue, 02 Aug 2022 03:26:35 GMT  
		Size: 45.1 MB (45147297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c247b2dc61cdf98e47d6c87cb26414dacc0cbef9f98b918e0900bbbb02d1d34f`  
		Last Modified: Tue, 02 Aug 2022 03:27:21 GMT  
		Size: 145.2 MB (145163883 bytes)  
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
$ docker pull buildpack-deps@sha256:487da0d43010692cb89ce7866ea622e8c2b8a4e6f2b7f5c6fdbf13d68b270890
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
$ docker pull buildpack-deps@sha256:b8906d491e9ea82d98e9a32a481e5ac8dd954ebd450ef51b66dd81d58e2c7758
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46945381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3ccbb2329fe1cdc286597d9fe720ae166a6ae78a42d285f218bdc868a849009`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:41:46 GMT
ADD file:294a94a081de785c730003a440a0530a85add2bcb60c0f5bc4ce7ee17867ac4e in / 
# Tue, 02 Aug 2022 01:41:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 02 Aug 2022 01:41:48 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:41:49 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 02 Aug 2022 01:41:49 GMT
CMD ["/bin/bash"]
# Tue, 02 Aug 2022 02:03:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 02:03:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b95ba076a26b98e98eac4b43596b59c20d1e61a36bcaf2afae3aeebadc8844cf`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 40.3 MB (40312250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c9df55506368eeeb59c5f56bf5d6f9ef4476a6b1e43154eebe32e436e60d7a`  
		Last Modified: Tue, 02 Aug 2022 01:44:42 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60aa30d82c4849b80da22554e0006d9c23c68a807fcb795b2f35ac6c02549eca`  
		Last Modified: Tue, 02 Aug 2022 01:44:42 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61b5d5a768deb5e021d74947bacf44422a006a3495d70395a7d745e07fab3f3`  
		Last Modified: Tue, 02 Aug 2022 01:44:42 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5302476a417ee0052e99816026f14bd6111e868aff0afed105038f5bf2c6ef`  
		Last Modified: Tue, 02 Aug 2022 02:19:12 GMT  
		Size: 6.6 MB (6631595 bytes)  
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
$ docker pull buildpack-deps@sha256:e2aa06904b7f5534f1de9f786e7d2bd4a9b18bc0965bac97a554ae93995a7081
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.8 MB (53750270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaaa97755201d055ca11812e12f2141e4fb1f55691aa21b2670756b6c564781c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:39:28 GMT
ADD file:a4ae521feddf8357667e9361bdd972a69ed945f3857cc8c534652592e432575d in / 
# Tue, 05 Apr 2022 22:39:29 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Apr 2022 22:39:30 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 22:39:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Apr 2022 22:39:32 GMT
CMD ["/bin/bash"]
# Tue, 05 Apr 2022 23:06:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:06:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1335d7ebdbbb7325d434cf945bcb54cb20f7288e1ca2a1cf140ae02b324646e6`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 45.8 MB (45816182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa6a227af79fa98ebbd1d2da516e2b7ce1cea5519a760cd0f6688738fbdb951`  
		Last Modified: Tue, 05 Apr 2022 22:40:40 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3928723c2c34ecd7264ce4e195ddda11403213b1c93d02e8efcd11de4b07a1`  
		Last Modified: Tue, 05 Apr 2022 22:40:40 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e468001dd2f338d54f47d062d65db61c754f09897744d97084afa15cee021200`  
		Last Modified: Tue, 05 Apr 2022 22:40:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abf8b8634fb64c0b6634daaf98b0d89d01420d22a01f63010623587194cfc7c`  
		Last Modified: Tue, 05 Apr 2022 23:13:08 GMT  
		Size: 7.9 MB (7932551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:16.04-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:78a48a34b1b38f960afab1bd4f452bfdf661eed3c719f377a8ea9afb7e96108f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.2 MB (55217329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbbd4191e342ab25bd0eea23323187f991a7f54697f813d022fbddaa02078c96`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:32:03 GMT
ADD file:c84969ed4d4e336ec5996e26e35261f683b36f1af7a978df587296ef5e7a2627 in / 
# Tue, 02 Aug 2022 01:32:06 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 02 Aug 2022 01:32:07 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:32:08 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 02 Aug 2022 01:32:08 GMT
CMD ["/bin/bash"]
# Tue, 02 Aug 2022 03:04:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 03:05:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5057452c10cfe2216f39949f909f3cd83002d256d1bbd564ae242352a5460fe2`  
		Last Modified: Sun, 08 Aug 2021 01:00:30 GMT  
		Size: 47.5 MB (47522137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72bced789eccb5759f541a5b15b9a3031c06cc54bdbff1a553cc0ef29ddad2bc`  
		Last Modified: Tue, 02 Aug 2022 01:36:22 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11a61259761ffe18601a628413443ccb5dee06a185a81c902220dfc070801c3`  
		Last Modified: Tue, 02 Aug 2022 01:35:56 GMT  
		Size: 483.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3272460dff18ff8fd96d33337b0ff5cc5d9d2e7f158c662273e1bb760c7f9722`  
		Last Modified: Tue, 02 Aug 2022 01:36:06 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65fd76771481bd61ed3539bc027b95c72e82ceebe357d2d960463332e3348c73`  
		Last Modified: Tue, 02 Aug 2022 03:26:11 GMT  
		Size: 7.7 MB (7693686 bytes)  
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
$ docker pull buildpack-deps@sha256:c65c40098f64bb19e2428d8d8bfa9a43fe88883acd39102ab9a88b43a421b67e
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
$ docker pull buildpack-deps@sha256:2e7f9d96fec289bb930857a48be7081ba0eb7cb06ac2b78e7f04b88f11e1ce75
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.1 MB (85107603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e970a2a3afffcff7f5e7d40b9772810da49015165b970887e44198ce39742ebd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:41:46 GMT
ADD file:294a94a081de785c730003a440a0530a85add2bcb60c0f5bc4ce7ee17867ac4e in / 
# Tue, 02 Aug 2022 01:41:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 02 Aug 2022 01:41:48 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:41:49 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 02 Aug 2022 01:41:49 GMT
CMD ["/bin/bash"]
# Tue, 02 Aug 2022 02:03:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 02:03:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 02:04:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b95ba076a26b98e98eac4b43596b59c20d1e61a36bcaf2afae3aeebadc8844cf`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 40.3 MB (40312250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c9df55506368eeeb59c5f56bf5d6f9ef4476a6b1e43154eebe32e436e60d7a`  
		Last Modified: Tue, 02 Aug 2022 01:44:42 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60aa30d82c4849b80da22554e0006d9c23c68a807fcb795b2f35ac6c02549eca`  
		Last Modified: Tue, 02 Aug 2022 01:44:42 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61b5d5a768deb5e021d74947bacf44422a006a3495d70395a7d745e07fab3f3`  
		Last Modified: Tue, 02 Aug 2022 01:44:42 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5302476a417ee0052e99816026f14bd6111e868aff0afed105038f5bf2c6ef`  
		Last Modified: Tue, 02 Aug 2022 02:19:12 GMT  
		Size: 6.6 MB (6631595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6ffa599dded0e2d5396a2e5b5cf1c7bef210b53ab5bc8863068549c1ce6bdd`  
		Last Modified: Tue, 02 Aug 2022 02:19:35 GMT  
		Size: 38.2 MB (38162222 bytes)  
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
$ docker pull buildpack-deps@sha256:69d52d4e7c9933b441c84db18e6de0103a2137a9117d289ad5358e21ffbce4b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.6 MB (96648412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7df7e0761688a883d92971b15cde9c5bf0036a95ca1ab2e035171fd5867c14b2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:39:28 GMT
ADD file:a4ae521feddf8357667e9361bdd972a69ed945f3857cc8c534652592e432575d in / 
# Tue, 05 Apr 2022 22:39:29 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Apr 2022 22:39:30 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 22:39:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Apr 2022 22:39:32 GMT
CMD ["/bin/bash"]
# Tue, 05 Apr 2022 23:06:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:06:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 05 Apr 2022 23:07:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1335d7ebdbbb7325d434cf945bcb54cb20f7288e1ca2a1cf140ae02b324646e6`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 45.8 MB (45816182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa6a227af79fa98ebbd1d2da516e2b7ce1cea5519a760cd0f6688738fbdb951`  
		Last Modified: Tue, 05 Apr 2022 22:40:40 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3928723c2c34ecd7264ce4e195ddda11403213b1c93d02e8efcd11de4b07a1`  
		Last Modified: Tue, 05 Apr 2022 22:40:40 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e468001dd2f338d54f47d062d65db61c754f09897744d97084afa15cee021200`  
		Last Modified: Tue, 05 Apr 2022 22:40:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abf8b8634fb64c0b6634daaf98b0d89d01420d22a01f63010623587194cfc7c`  
		Last Modified: Tue, 05 Apr 2022 23:13:08 GMT  
		Size: 7.9 MB (7932551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6d144d968e58673ed441d100257197c971e98922fc325d2b9d2726c37b1669`  
		Last Modified: Tue, 05 Apr 2022 23:13:29 GMT  
		Size: 42.9 MB (42898142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:16.04-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:ec195c6680999f436dcaac43ecb2f433c12e294279f4457108cc09461edf2636
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.4 MB (100364626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54097dd529c992a5b4db8428a52ab66f609f66f1a118b2626a87128df3c5a414`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:32:03 GMT
ADD file:c84969ed4d4e336ec5996e26e35261f683b36f1af7a978df587296ef5e7a2627 in / 
# Tue, 02 Aug 2022 01:32:06 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 02 Aug 2022 01:32:07 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:32:08 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 02 Aug 2022 01:32:08 GMT
CMD ["/bin/bash"]
# Tue, 02 Aug 2022 03:04:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 03:05:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 03:06:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5057452c10cfe2216f39949f909f3cd83002d256d1bbd564ae242352a5460fe2`  
		Last Modified: Sun, 08 Aug 2021 01:00:30 GMT  
		Size: 47.5 MB (47522137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72bced789eccb5759f541a5b15b9a3031c06cc54bdbff1a553cc0ef29ddad2bc`  
		Last Modified: Tue, 02 Aug 2022 01:36:22 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11a61259761ffe18601a628413443ccb5dee06a185a81c902220dfc070801c3`  
		Last Modified: Tue, 02 Aug 2022 01:35:56 GMT  
		Size: 483.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3272460dff18ff8fd96d33337b0ff5cc5d9d2e7f158c662273e1bb760c7f9722`  
		Last Modified: Tue, 02 Aug 2022 01:36:06 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65fd76771481bd61ed3539bc027b95c72e82ceebe357d2d960463332e3348c73`  
		Last Modified: Tue, 02 Aug 2022 03:26:11 GMT  
		Size: 7.7 MB (7693686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6157fa0cdd9af85bd373614103144ea737420e95c79b68ad61350c0104479e7`  
		Last Modified: Tue, 02 Aug 2022 03:26:35 GMT  
		Size: 45.1 MB (45147297 bytes)  
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
$ docker pull buildpack-deps@sha256:9ac27efda917198bf27efc5793d8149435ee00736bba49926fc8a654f5c356a3
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
$ docker pull buildpack-deps@sha256:e528083f16c11b7887692e4e3c95c3a6870518320b2f58540dd7bbe969c6d1b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.4 MB (221392214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5aed41ef81bfee2777d4de5e91ad756fef93503d0700fc0dacc473d761971818`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 19:38:36 GMT
ADD file:8733c7e8faf03d53cb2143ff6ac405362944cfa07422fccd21a3066cc2f42c83 in / 
# Tue, 06 Sep 2022 19:38:37 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:56:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:56:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Sep 2022 19:56:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:59:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:726b8a513d66e3585eb57389171d97fcd348e4914a415891e1da135b85ffa6c3`  
		Last Modified: Fri, 02 Sep 2022 15:41:13 GMT  
		Size: 26.7 MB (26710833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7dbb4551b9c872b2053c38cdd5dd7e02c06107e648b950551a585e5e88394c7`  
		Last Modified: Tue, 06 Sep 2022 20:00:54 GMT  
		Size: 6.6 MB (6630965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79cc7a6dc37d1b46bb3edb182f0a133c77f677de31779964db5569d6137a99d`  
		Last Modified: Tue, 06 Sep 2022 20:00:54 GMT  
		Size: 3.0 MB (3023688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5b4b52eebf079a3d5e1a1decad6af97acccd018f5d50a4c0e9533a54a3cdbc`  
		Last Modified: Tue, 06 Sep 2022 20:01:11 GMT  
		Size: 45.5 MB (45498322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4c3ab92be332905d30314f7e4fc0775d75a34044a859f49564b40fe4e7cffc`  
		Last Modified: Tue, 06 Sep 2022 20:01:40 GMT  
		Size: 139.5 MB (139528406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:0fce3a21c1614e61a642bf5a439ac1770eb692c003e2ae3e08a76e619291b0d0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.6 MB (189556723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e2da3dee6e14720f0c8cb851fba01ac825f58712778a0f763864eeaa456d206`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 19:33:23 GMT
ADD file:45c82fca220161f3905a06e276f12ec0cb3be5c099cca70bb6d495da10088f7d in / 
# Tue, 06 Sep 2022 19:33:24 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:51:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:52:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Sep 2022 19:52:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:53:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:074d633b5bde02245e333b110dde5850e06ea4ebefe4283af6e4dfd8d462b170`  
		Last Modified: Tue, 06 Sep 2022 19:35:07 GMT  
		Size: 22.3 MB (22305954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594729c31c2cb7f63b20f449c44c215064e068c94731174e4b57603ce032fd82`  
		Last Modified: Tue, 06 Sep 2022 19:57:06 GMT  
		Size: 5.7 MB (5698254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da759356c74e12ad90a263cb412b2ea0620a103ffedbdb492aac5586d59cdb83`  
		Last Modified: Tue, 06 Sep 2022 19:57:05 GMT  
		Size: 2.6 MB (2585972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31889323a628fc6a5d5b97236ff7b9500b05e2cafa958463ef4094646c8f3603`  
		Last Modified: Tue, 06 Sep 2022 19:57:25 GMT  
		Size: 40.7 MB (40691568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7cff271266119a86a51033715e0198a3b8755f84d2c5cca74c523f8225cc280`  
		Last Modified: Tue, 06 Sep 2022 19:57:53 GMT  
		Size: 118.3 MB (118274975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3ebaa3c12382c2516c8728bafd1ee97a069548dc91e3dc74d6867d591d5a17ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.5 MB (205513212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:931d6758b74219c522750ad62e920c8098f22702e137a5eed6754217c4556dd8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 18:49:02 GMT
ADD file:26cb5ace98a4462b36211bf28f1e73781dd6d8984350d9bd53243dbe50ae180c in / 
# Tue, 06 Sep 2022 18:49:02 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:12:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:12:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Sep 2022 19:13:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:13:59 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d30cf2a6a25aea48a115837d149468c8de7df7fb51f210b9fa1173c065f7b34c`  
		Last Modified: Tue, 06 Sep 2022 18:50:34 GMT  
		Size: 23.7 MB (23734076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79317661c5fe6a8a22ce652c9fb0999eb96ed08b735a16224e9a795c877780d`  
		Last Modified: Tue, 06 Sep 2022 19:16:57 GMT  
		Size: 6.1 MB (6072017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:737382e506f963b99b1453e20a2fcbb6bc4328a0c68bfc3530b2082a5f3da14f`  
		Last Modified: Tue, 06 Sep 2022 19:16:56 GMT  
		Size: 2.6 MB (2571091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160f71044c4c89d05d500625b4eda19add7227d613b991017a9850f2945440d2`  
		Last Modified: Tue, 06 Sep 2022 19:17:14 GMT  
		Size: 43.3 MB (43296151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ec4cd1624a82a57e6cd377e4126b4e69c04991aca1f9dd6b9380b4a351e588`  
		Last Modified: Tue, 06 Sep 2022 19:17:44 GMT  
		Size: 129.8 MB (129839877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04` - linux; 386

```console
$ docker pull buildpack-deps@sha256:1e08f63aabe1e3e0539b94fb88d71d70045de1b2a09c1cb0678ae765d602281d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.2 MB (218228400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:523091bbe3ef5b646de02652ba174944425c430cba9e8d570d61d6936e640f7c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 18:40:06 GMT
ADD file:31701667cc90b9f4ce7d6ede94bf7dae4d63c49e62d3725094d547f9601e1165 in / 
# Tue, 06 Sep 2022 18:40:07 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:02:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:02:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Sep 2022 19:02:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:04:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10d3032d1995d3163c20a7f2f197299fae258c2ad020a8fd586fd6b7dd1b0e1d`  
		Last Modified: Tue, 06 Sep 2022 18:40:53 GMT  
		Size: 27.2 MB (27164710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360b65e679bf1db70d92b45a6d39c882e074d441412548705adf35d49a12c70a`  
		Last Modified: Tue, 06 Sep 2022 19:06:33 GMT  
		Size: 6.9 MB (6919740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8820513ab0577fe6133989b66cdc2a5a0b1a97af5280746721af55657c0897d7`  
		Last Modified: Tue, 06 Sep 2022 19:06:32 GMT  
		Size: 3.0 MB (3039943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ad90e9fc8930485dc12eedaf8101fe62b983d943986b7325ff502b9d424d75`  
		Last Modified: Tue, 06 Sep 2022 19:06:52 GMT  
		Size: 47.1 MB (47083595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bdffbbc9ce11b7acde16175dcc810b3cd9c5e5f850cac91cfcd033e2c2bcf9`  
		Last Modified: Tue, 06 Sep 2022 19:07:20 GMT  
		Size: 134.0 MB (134020412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:ac71ffe284d77165ccbfe8e4f10276653fde3026f002fc1e2a5557fba36cdfe1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.4 MB (246400050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddcce9c6043a6417a17152dbbefebdc2086e1240454861f17bfdd701a73c7c6f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 19:38:57 GMT
ADD file:1b76d0a41921afefb92711c44ceb312c16828d433b689a951d65c238faa9ac50 in / 
# Tue, 06 Sep 2022 19:38:59 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 20:06:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 20:06:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Sep 2022 20:07:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 20:09:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4abf8f40556a940861bc7fc313acefb89c775273ed06b7d41cfb222ccf8a1438`  
		Last Modified: Tue, 06 Sep 2022 19:40:56 GMT  
		Size: 30.4 MB (30441623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7afd3028934ff054bca1d0bb218e690d2cdb60f7754ad3bb6426c3744e730f`  
		Last Modified: Tue, 06 Sep 2022 20:12:44 GMT  
		Size: 7.1 MB (7050146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33850c25587eb4418b5e6aeccf1c9e6fa5b0baac624020bc56b4d4db8c2742c5`  
		Last Modified: Tue, 06 Sep 2022 20:12:43 GMT  
		Size: 3.7 MB (3720231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677c4d750793a0cab4cd23689261d167383d4e03f7fce03417017fcfd5497d21`  
		Last Modified: Tue, 06 Sep 2022 20:13:12 GMT  
		Size: 53.7 MB (53744408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2548f24520c161a34a9b39bc85562ec79da91528e4742bfafd4dc333ae3b0489`  
		Last Modified: Tue, 06 Sep 2022 20:14:01 GMT  
		Size: 151.4 MB (151443642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:00d5ff189772c956744ca48d4cb80e449ce51e844a304eb5336ed8ff5a1c96d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.7 MB (205748449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d78f4436f2d6ebf559f756716d8782d1472e28502b39ffdd40c045b74f4ea2f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 18:43:36 GMT
ADD file:dbe2a8e3943129e654ee29c636cab2bb10dd7eb0ac27d51e6954af2ccbe22807 in / 
# Tue, 06 Sep 2022 18:43:37 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:11:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:11:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Sep 2022 19:12:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:13:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be6761156800c616810cb8aeb5b3ae71b9a2082f1c1221210befe119f082e879`  
		Last Modified: Tue, 06 Sep 2022 18:45:00 GMT  
		Size: 25.4 MB (25370130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae409e724954611ea7731639a0dab7c4c59fdb64deb51dba5327bc8c5a085c5f`  
		Last Modified: Tue, 06 Sep 2022 19:17:11 GMT  
		Size: 6.3 MB (6324234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aca3edc7c631417c9e3dbbcb30698aed6531dc2482e10dd41ee221de2d450ca5`  
		Last Modified: Tue, 06 Sep 2022 19:17:11 GMT  
		Size: 3.0 MB (2977166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee7b8f6dba5690621ef3c6a174a056a9b68be9f2c37eeb155bc990d0284bcf0`  
		Last Modified: Tue, 06 Sep 2022 19:17:26 GMT  
		Size: 45.0 MB (45043901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:654a99a01d5150ba8cc8996260cf51a2b5c4a95e746908bcf7f69f1a719549ac`  
		Last Modified: Tue, 06 Sep 2022 19:17:50 GMT  
		Size: 126.0 MB (126033018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:18.04-curl`

```console
$ docker pull buildpack-deps@sha256:dcb2d54836f9a7ca1639cd4fd498925e854cfe0a2789eeac075e825d4ec55dd7
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
$ docker pull buildpack-deps@sha256:fb84bfba9252ad0cad4bf624e06d1c893d3b1a7f55e3cc37aa605f5a67d9441d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36365486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64c992125c0697acbdc18105c298d44b3c5e089b2fdfaef91658643be66c77d1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 19:38:36 GMT
ADD file:8733c7e8faf03d53cb2143ff6ac405362944cfa07422fccd21a3066cc2f42c83 in / 
# Tue, 06 Sep 2022 19:38:37 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:56:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:56:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:726b8a513d66e3585eb57389171d97fcd348e4914a415891e1da135b85ffa6c3`  
		Last Modified: Fri, 02 Sep 2022 15:41:13 GMT  
		Size: 26.7 MB (26710833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7dbb4551b9c872b2053c38cdd5dd7e02c06107e648b950551a585e5e88394c7`  
		Last Modified: Tue, 06 Sep 2022 20:00:54 GMT  
		Size: 6.6 MB (6630965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79cc7a6dc37d1b46bb3edb182f0a133c77f677de31779964db5569d6137a99d`  
		Last Modified: Tue, 06 Sep 2022 20:00:54 GMT  
		Size: 3.0 MB (3023688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:afe6b279269826bd9d9a9b77ac80bbd54db65cc922bf5a184f06f6a396719d8e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30590180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53b82ac9f9048c0858ffaed15ca8ef98cdc38e7c07be402ef88ebaf6792962c6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 19:33:23 GMT
ADD file:45c82fca220161f3905a06e276f12ec0cb3be5c099cca70bb6d495da10088f7d in / 
# Tue, 06 Sep 2022 19:33:24 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:51:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:52:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:074d633b5bde02245e333b110dde5850e06ea4ebefe4283af6e4dfd8d462b170`  
		Last Modified: Tue, 06 Sep 2022 19:35:07 GMT  
		Size: 22.3 MB (22305954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594729c31c2cb7f63b20f449c44c215064e068c94731174e4b57603ce032fd82`  
		Last Modified: Tue, 06 Sep 2022 19:57:06 GMT  
		Size: 5.7 MB (5698254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da759356c74e12ad90a263cb412b2ea0620a103ffedbdb492aac5586d59cdb83`  
		Last Modified: Tue, 06 Sep 2022 19:57:05 GMT  
		Size: 2.6 MB (2585972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:2a7863e0c4008a73ef0bda24499179d884f903c73c1669375cb88f15c545fc25
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.4 MB (32377184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07c6a028cf3ecfd36dd9d598bbb927e84f8a27631f594cabce0272768f7bb62f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 18:49:02 GMT
ADD file:26cb5ace98a4462b36211bf28f1e73781dd6d8984350d9bd53243dbe50ae180c in / 
# Tue, 06 Sep 2022 18:49:02 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:12:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:12:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d30cf2a6a25aea48a115837d149468c8de7df7fb51f210b9fa1173c065f7b34c`  
		Last Modified: Tue, 06 Sep 2022 18:50:34 GMT  
		Size: 23.7 MB (23734076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79317661c5fe6a8a22ce652c9fb0999eb96ed08b735a16224e9a795c877780d`  
		Last Modified: Tue, 06 Sep 2022 19:16:57 GMT  
		Size: 6.1 MB (6072017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:737382e506f963b99b1453e20a2fcbb6bc4328a0c68bfc3530b2082a5f3da14f`  
		Last Modified: Tue, 06 Sep 2022 19:16:56 GMT  
		Size: 2.6 MB (2571091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:9843a4e78ba03fb07ec7138d9afdaabb3412478c44103fbca5fc8732b1a29bb8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37124393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab6063d4c02c86863842cda863cdd0b9fc41b99181a9d5bb4e10e93c58167700`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 18:40:06 GMT
ADD file:31701667cc90b9f4ce7d6ede94bf7dae4d63c49e62d3725094d547f9601e1165 in / 
# Tue, 06 Sep 2022 18:40:07 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:02:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:02:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:10d3032d1995d3163c20a7f2f197299fae258c2ad020a8fd586fd6b7dd1b0e1d`  
		Last Modified: Tue, 06 Sep 2022 18:40:53 GMT  
		Size: 27.2 MB (27164710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360b65e679bf1db70d92b45a6d39c882e074d441412548705adf35d49a12c70a`  
		Last Modified: Tue, 06 Sep 2022 19:06:33 GMT  
		Size: 6.9 MB (6919740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8820513ab0577fe6133989b66cdc2a5a0b1a97af5280746721af55657c0897d7`  
		Last Modified: Tue, 06 Sep 2022 19:06:32 GMT  
		Size: 3.0 MB (3039943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:17ba421e87b43d3709f030baae5c32ff973f324914ce189a7ec322b8d465f42c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41212000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f2cd514147c478a3ed7fabf6a7c9ce8924b524298a42b113013caf62abee8b5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 19:38:57 GMT
ADD file:1b76d0a41921afefb92711c44ceb312c16828d433b689a951d65c238faa9ac50 in / 
# Tue, 06 Sep 2022 19:38:59 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 20:06:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 20:06:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4abf8f40556a940861bc7fc313acefb89c775273ed06b7d41cfb222ccf8a1438`  
		Last Modified: Tue, 06 Sep 2022 19:40:56 GMT  
		Size: 30.4 MB (30441623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7afd3028934ff054bca1d0bb218e690d2cdb60f7754ad3bb6426c3744e730f`  
		Last Modified: Tue, 06 Sep 2022 20:12:44 GMT  
		Size: 7.1 MB (7050146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33850c25587eb4418b5e6aeccf1c9e6fa5b0baac624020bc56b4d4db8c2742c5`  
		Last Modified: Tue, 06 Sep 2022 20:12:43 GMT  
		Size: 3.7 MB (3720231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:88bdf05d087dec6348b811e7fe133c6de77ad937052d47ef17e19e9f48313d15
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34671530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1271e59da62b67faad96ae96f4a55cbfdf33568b76dbfc4820467a25e9cc5d51`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 18:43:36 GMT
ADD file:dbe2a8e3943129e654ee29c636cab2bb10dd7eb0ac27d51e6954af2ccbe22807 in / 
# Tue, 06 Sep 2022 18:43:37 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:11:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:11:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:be6761156800c616810cb8aeb5b3ae71b9a2082f1c1221210befe119f082e879`  
		Last Modified: Tue, 06 Sep 2022 18:45:00 GMT  
		Size: 25.4 MB (25370130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae409e724954611ea7731639a0dab7c4c59fdb64deb51dba5327bc8c5a085c5f`  
		Last Modified: Tue, 06 Sep 2022 19:17:11 GMT  
		Size: 6.3 MB (6324234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aca3edc7c631417c9e3dbbcb30698aed6531dc2482e10dd41ee221de2d450ca5`  
		Last Modified: Tue, 06 Sep 2022 19:17:11 GMT  
		Size: 3.0 MB (2977166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:18.04-scm`

```console
$ docker pull buildpack-deps@sha256:60bf73bfe83bfe213a096d826301485d12b23121eb2cb945971b57b12d44f7f5
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
$ docker pull buildpack-deps@sha256:99364dc903d771b32e2c8c419a0a34c5d6a220dd72f1f3a56705d01c8ff04d74
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81863808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc7db731cc6dfe3ba8e4d80592a46f2869a517287d15a058d9c9d66c02583085`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 19:38:36 GMT
ADD file:8733c7e8faf03d53cb2143ff6ac405362944cfa07422fccd21a3066cc2f42c83 in / 
# Tue, 06 Sep 2022 19:38:37 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:56:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:56:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Sep 2022 19:56:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:726b8a513d66e3585eb57389171d97fcd348e4914a415891e1da135b85ffa6c3`  
		Last Modified: Fri, 02 Sep 2022 15:41:13 GMT  
		Size: 26.7 MB (26710833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7dbb4551b9c872b2053c38cdd5dd7e02c06107e648b950551a585e5e88394c7`  
		Last Modified: Tue, 06 Sep 2022 20:00:54 GMT  
		Size: 6.6 MB (6630965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79cc7a6dc37d1b46bb3edb182f0a133c77f677de31779964db5569d6137a99d`  
		Last Modified: Tue, 06 Sep 2022 20:00:54 GMT  
		Size: 3.0 MB (3023688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5b4b52eebf079a3d5e1a1decad6af97acccd018f5d50a4c0e9533a54a3cdbc`  
		Last Modified: Tue, 06 Sep 2022 20:01:11 GMT  
		Size: 45.5 MB (45498322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:b5e3fcf7ff33c0a0102f3dd8b37137429f5b2abb399fdd3287d88d2daf8387a5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71281748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:157ec7a9d18b93b9853234a51689143321a6547d2e65911c5562b7cd3e9b31f2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 19:33:23 GMT
ADD file:45c82fca220161f3905a06e276f12ec0cb3be5c099cca70bb6d495da10088f7d in / 
# Tue, 06 Sep 2022 19:33:24 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:51:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:52:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Sep 2022 19:52:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:074d633b5bde02245e333b110dde5850e06ea4ebefe4283af6e4dfd8d462b170`  
		Last Modified: Tue, 06 Sep 2022 19:35:07 GMT  
		Size: 22.3 MB (22305954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594729c31c2cb7f63b20f449c44c215064e068c94731174e4b57603ce032fd82`  
		Last Modified: Tue, 06 Sep 2022 19:57:06 GMT  
		Size: 5.7 MB (5698254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da759356c74e12ad90a263cb412b2ea0620a103ffedbdb492aac5586d59cdb83`  
		Last Modified: Tue, 06 Sep 2022 19:57:05 GMT  
		Size: 2.6 MB (2585972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31889323a628fc6a5d5b97236ff7b9500b05e2cafa958463ef4094646c8f3603`  
		Last Modified: Tue, 06 Sep 2022 19:57:25 GMT  
		Size: 40.7 MB (40691568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ff7947cce30c9ff5827fef08b8fba331fd9d6b4250e279b46dd5c95c3a6a9fbc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75673335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0910d8ecce3a327c711cb34093bb9b3c9fffef753ecae8c78456571c3564b47e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 18:49:02 GMT
ADD file:26cb5ace98a4462b36211bf28f1e73781dd6d8984350d9bd53243dbe50ae180c in / 
# Tue, 06 Sep 2022 18:49:02 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:12:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:12:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Sep 2022 19:13:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d30cf2a6a25aea48a115837d149468c8de7df7fb51f210b9fa1173c065f7b34c`  
		Last Modified: Tue, 06 Sep 2022 18:50:34 GMT  
		Size: 23.7 MB (23734076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79317661c5fe6a8a22ce652c9fb0999eb96ed08b735a16224e9a795c877780d`  
		Last Modified: Tue, 06 Sep 2022 19:16:57 GMT  
		Size: 6.1 MB (6072017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:737382e506f963b99b1453e20a2fcbb6bc4328a0c68bfc3530b2082a5f3da14f`  
		Last Modified: Tue, 06 Sep 2022 19:16:56 GMT  
		Size: 2.6 MB (2571091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160f71044c4c89d05d500625b4eda19add7227d613b991017a9850f2945440d2`  
		Last Modified: Tue, 06 Sep 2022 19:17:14 GMT  
		Size: 43.3 MB (43296151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:0ebf787eef91cb40d6785f4fee2e318e1caa0efea1ef139dd16efb9cb2170108
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.2 MB (84207988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bade70b0313e63645171fc0d2e32aac037cc1c538a5011e096bf92b7bf9bec62`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 18:40:06 GMT
ADD file:31701667cc90b9f4ce7d6ede94bf7dae4d63c49e62d3725094d547f9601e1165 in / 
# Tue, 06 Sep 2022 18:40:07 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:02:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:02:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Sep 2022 19:02:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10d3032d1995d3163c20a7f2f197299fae258c2ad020a8fd586fd6b7dd1b0e1d`  
		Last Modified: Tue, 06 Sep 2022 18:40:53 GMT  
		Size: 27.2 MB (27164710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360b65e679bf1db70d92b45a6d39c882e074d441412548705adf35d49a12c70a`  
		Last Modified: Tue, 06 Sep 2022 19:06:33 GMT  
		Size: 6.9 MB (6919740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8820513ab0577fe6133989b66cdc2a5a0b1a97af5280746721af55657c0897d7`  
		Last Modified: Tue, 06 Sep 2022 19:06:32 GMT  
		Size: 3.0 MB (3039943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ad90e9fc8930485dc12eedaf8101fe62b983d943986b7325ff502b9d424d75`  
		Last Modified: Tue, 06 Sep 2022 19:06:52 GMT  
		Size: 47.1 MB (47083595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3cb7543c344e0352386e8a80cfe8d4ad2ad58f5d0b15c562893d95425acd39a0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.0 MB (94956408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60cb88494227b72c2ba6f2f4ea540126cfe6da20dd2844ac77122510289f8cf0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 19:38:57 GMT
ADD file:1b76d0a41921afefb92711c44ceb312c16828d433b689a951d65c238faa9ac50 in / 
# Tue, 06 Sep 2022 19:38:59 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 20:06:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 20:06:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Sep 2022 20:07:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4abf8f40556a940861bc7fc313acefb89c775273ed06b7d41cfb222ccf8a1438`  
		Last Modified: Tue, 06 Sep 2022 19:40:56 GMT  
		Size: 30.4 MB (30441623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7afd3028934ff054bca1d0bb218e690d2cdb60f7754ad3bb6426c3744e730f`  
		Last Modified: Tue, 06 Sep 2022 20:12:44 GMT  
		Size: 7.1 MB (7050146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33850c25587eb4418b5e6aeccf1c9e6fa5b0baac624020bc56b4d4db8c2742c5`  
		Last Modified: Tue, 06 Sep 2022 20:12:43 GMT  
		Size: 3.7 MB (3720231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677c4d750793a0cab4cd23689261d167383d4e03f7fce03417017fcfd5497d21`  
		Last Modified: Tue, 06 Sep 2022 20:13:12 GMT  
		Size: 53.7 MB (53744408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a75bb4a086eb933364de634f5df3c444ccf522851ca2519cbb956366f444fce9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79715431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:718e03d049e2e94d8ddad47f516b220c5cdbf5ffde7f2e3a4f0a9a6808c63589`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 18:43:36 GMT
ADD file:dbe2a8e3943129e654ee29c636cab2bb10dd7eb0ac27d51e6954af2ccbe22807 in / 
# Tue, 06 Sep 2022 18:43:37 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:11:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:11:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Sep 2022 19:12:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be6761156800c616810cb8aeb5b3ae71b9a2082f1c1221210befe119f082e879`  
		Last Modified: Tue, 06 Sep 2022 18:45:00 GMT  
		Size: 25.4 MB (25370130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae409e724954611ea7731639a0dab7c4c59fdb64deb51dba5327bc8c5a085c5f`  
		Last Modified: Tue, 06 Sep 2022 19:17:11 GMT  
		Size: 6.3 MB (6324234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aca3edc7c631417c9e3dbbcb30698aed6531dc2482e10dd41ee221de2d450ca5`  
		Last Modified: Tue, 06 Sep 2022 19:17:11 GMT  
		Size: 3.0 MB (2977166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee7b8f6dba5690621ef3c6a174a056a9b68be9f2c37eeb155bc990d0284bcf0`  
		Last Modified: Tue, 06 Sep 2022 19:17:26 GMT  
		Size: 45.0 MB (45043901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:20.04`

```console
$ docker pull buildpack-deps@sha256:7e46c886cfb15a4bb8d6c337f664f56a107e337264a74f80d9a1d0835b83dd61
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
$ docker pull buildpack-deps@sha256:236275a19f23e22211c79a72f7606ead785500c53780cff18e7ebff5fffdada5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.7 MB (245735269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c377f7b08c01644a3b2aa6f083ce6d4f1812e8652efbc64a7b9b550dbfb08132`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:23:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:23:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 02:24:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:27:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aceaa9f66a60a3695a6348be449df629aed61f57a9cbd55a388bdcfa40cb27b7`  
		Last Modified: Fri, 02 Sep 2022 02:37:25 GMT  
		Size: 7.7 MB (7747479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d69e69900ca0c9eb8762e001879c1e84e29d94a2397e389440b1d8689445e5`  
		Last Modified: Fri, 02 Sep 2022 02:37:24 GMT  
		Size: 3.6 MB (3624451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:035d79e04aad5acedcb6ebd870819e030f0f1cb534d55136ac5f6087b31b39f9`  
		Last Modified: Fri, 02 Sep 2022 02:37:44 GMT  
		Size: 60.7 MB (60738066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f65cb058b8e19392f740a77af749897af039a43730af19d5b986a7de8cc696`  
		Last Modified: Fri, 02 Sep 2022 02:38:15 GMT  
		Size: 145.1 MB (145052588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:6cc83b90351f8ac0223faa87e392c2a9f24157d4f422e588bb779baa01f1ce55
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.8 MB (211783596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:581bfa0c33a65661c95cc0c51eb8e5cebb681ebbee12360daadc798008c4d1ee`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 06:08:22 GMT
ADD file:685f4b5f8c1f11b6389e9f929909e1a667abf29814a7ccfb859aae287dacd7e1 in / 
# Fri, 02 Sep 2022 06:08:22 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 09:31:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 09:32:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 09:32:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 09:33:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:eff72fca8e1d166ddfda6ac6c409e888c95950da6c47d360a088219c0ad7ba05`  
		Last Modified: Fri, 02 Sep 2022 06:10:16 GMT  
		Size: 24.6 MB (24588743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0063ca7d240c073b50b399efe49028199e2fc1671c3d5e69e566b2b36dea9282`  
		Last Modified: Fri, 02 Sep 2022 09:41:04 GMT  
		Size: 6.7 MB (6741254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93ac5277e93cfbfa1f89a828713b7c6314babc86f222357de3141883f92a010`  
		Last Modified: Fri, 02 Sep 2022 09:41:04 GMT  
		Size: 3.1 MB (3104403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ccea48caa3d4856a1e5a5278dfb92e187166e74c5f4226090de64a520ae1f91`  
		Last Modified: Fri, 02 Sep 2022 09:41:27 GMT  
		Size: 55.4 MB (55442260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715d9c57028ba4ae9a65a2fe21da32b16c0d47fed424958a335b6ff470ec3fad`  
		Last Modified: Fri, 02 Sep 2022 09:41:57 GMT  
		Size: 121.9 MB (121906936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:6e21811ff53feb197c55dbcb5913e6167d2f756d5225790d038f9b9b82b31c3e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.5 MB (235507390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8031960c5c0d2a8ef476a475b524c69ce8e35c58b47617ebd56fe13cdd990406`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:38:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:38:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 04:39:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:40:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6667cb55d48ba4971074c7d8aa09e7b2368fb83f8ab6336c1ae53675ef8a5fdc`  
		Last Modified: Fri, 02 Sep 2022 04:46:48 GMT  
		Size: 7.6 MB (7614784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f84ae37056f7e9d12b5c5d6fbf1924cc86999a56dd4adeff2f422552b9edf08`  
		Last Modified: Fri, 02 Sep 2022 04:46:48 GMT  
		Size: 3.4 MB (3387844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8330d23b3e1d0fb7320e653a9dba9018129a28846b4d6cffdc5caa044ceee0`  
		Last Modified: Fri, 02 Sep 2022 04:47:09 GMT  
		Size: 60.8 MB (60803136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131f3a8b3e4894860eeb15da87fb3843ad69cebaa2ea4bb04c6b16240a96eef2`  
		Last Modified: Fri, 02 Sep 2022 04:47:40 GMT  
		Size: 136.5 MB (136509809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:b864ae13cc2a8ce0ee0d8dee4231935012a1f332f708f5e160d746b0e322b543
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.5 MB (269549986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3829078671a39b677798e7ff15db74a35aa34c521d9cdba344014e925803e15d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:49:54 GMT
ADD file:eb82827919ea73f9595d7b0b70fe9aa5ff23e16ea6a87f7f9ef4e1905857b789 in / 
# Thu, 01 Sep 2022 23:49:56 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:34:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:35:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 03:36:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:39:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:891f6400ce611ee5975f04ad6d2c68305c76a8628b846df1b1f9ac7c45b1311c`  
		Last Modified: Thu, 01 Sep 2022 23:52:11 GMT  
		Size: 33.3 MB (33295624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c38e8344eceb4e722b9d2cc7cf0d2cdca38bb2870c652f545c8ea652efa4f6`  
		Last Modified: Fri, 02 Sep 2022 03:55:42 GMT  
		Size: 8.7 MB (8704791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059cb2841292be0e2908a7c8f78a0db3f136154b78b70a9881535c8c1080dc3f`  
		Last Modified: Fri, 02 Sep 2022 03:55:41 GMT  
		Size: 4.5 MB (4456160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cd324c0fe479474378bdfc00b7027887775d4396a082938a08a2b3f8163431`  
		Last Modified: Fri, 02 Sep 2022 03:56:12 GMT  
		Size: 69.5 MB (69529571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845e0c714d38e7d101ce3585817a73b34d9f7e53c5810c5ad7ecc1f8469f0e7b`  
		Last Modified: Fri, 02 Sep 2022 03:57:03 GMT  
		Size: 153.6 MB (153563840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:0983feadc237a384bc35d020091ffbf6b9eb5b8b312f716e301223786fa27dd4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.4 MB (226432077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c4f4a81fad6a7cffcc865b12be1766a3f2d65338bbd923218ff0906b2232f3`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:13 GMT
ADD file:75a78d9ec31ac5486bdde3e48ebfc534089c5f38f14850243c2ab2e632f0bbe5 in / 
# Fri, 02 Sep 2022 01:03:16 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:03:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:04:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 02:04:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:06:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b87ab7b8bb5c2a1f34d9a2e9887fde669c33cea7428fdb048362dfa81eccaa75`  
		Last Modified: Fri, 02 Sep 2022 01:04:49 GMT  
		Size: 27.0 MB (27045282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f81ff7514526202dbe703eab1c9f1a8c08e2fdc2c2d56b949c8d1f90825e908`  
		Last Modified: Fri, 02 Sep 2022 02:15:30 GMT  
		Size: 7.4 MB (7397526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30cf575bc155da8ebabf970fa2716a48bb3789c6a3967d83d0f7583991658942`  
		Last Modified: Fri, 02 Sep 2022 02:15:30 GMT  
		Size: 3.5 MB (3542655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:423b3fa0fb4a3902e95b623da0004da02d690cf894720b6584469c6c7709e39a`  
		Last Modified: Fri, 02 Sep 2022 02:15:48 GMT  
		Size: 60.0 MB (60008998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4036fb36c2cf3563cffaf474016b239dfaed09f13efbeea14c7f35e3027aecfb`  
		Last Modified: Fri, 02 Sep 2022 02:16:12 GMT  
		Size: 128.4 MB (128437616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:20.04-curl`

```console
$ docker pull buildpack-deps@sha256:55c8b92c9d110cd78a6118ad40af433837e827a34ea048aea2d9d9a846963ce2
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
$ docker pull buildpack-deps@sha256:859a87863b458751a541038d05e5569e5f62dc78e39091b7b6225a3ea9745a8d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.9 MB (39944615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71654a9ae5f8958dcaa319be61ebc69326d6eb070e287963d83a169357468b2c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:23:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:23:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aceaa9f66a60a3695a6348be449df629aed61f57a9cbd55a388bdcfa40cb27b7`  
		Last Modified: Fri, 02 Sep 2022 02:37:25 GMT  
		Size: 7.7 MB (7747479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d69e69900ca0c9eb8762e001879c1e84e29d94a2397e389440b1d8689445e5`  
		Last Modified: Fri, 02 Sep 2022 02:37:24 GMT  
		Size: 3.6 MB (3624451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:cdcb31c6c524a3dc5e984ae33da46514f4d8e5e660ca81af01394d1a25532bfa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34434400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaa09c1b604887bf598f7cb6368be01387a6cf9daa76e3e9fbedb8b6f152564c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 06:08:22 GMT
ADD file:685f4b5f8c1f11b6389e9f929909e1a667abf29814a7ccfb859aae287dacd7e1 in / 
# Fri, 02 Sep 2022 06:08:22 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 09:31:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 09:32:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:eff72fca8e1d166ddfda6ac6c409e888c95950da6c47d360a088219c0ad7ba05`  
		Last Modified: Fri, 02 Sep 2022 06:10:16 GMT  
		Size: 24.6 MB (24588743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0063ca7d240c073b50b399efe49028199e2fc1671c3d5e69e566b2b36dea9282`  
		Last Modified: Fri, 02 Sep 2022 09:41:04 GMT  
		Size: 6.7 MB (6741254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93ac5277e93cfbfa1f89a828713b7c6314babc86f222357de3141883f92a010`  
		Last Modified: Fri, 02 Sep 2022 09:41:04 GMT  
		Size: 3.1 MB (3104403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7a621cd38afcf8f3d75a8f8dcd631038d460ca67c752870dc041e60595956163
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38194445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84b6a55990e1096425a70e6b907d1ba30b69bbd3131c15a11f2c662b8fe06677`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:38:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:38:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6667cb55d48ba4971074c7d8aa09e7b2368fb83f8ab6336c1ae53675ef8a5fdc`  
		Last Modified: Fri, 02 Sep 2022 04:46:48 GMT  
		Size: 7.6 MB (7614784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f84ae37056f7e9d12b5c5d6fbf1924cc86999a56dd4adeff2f422552b9edf08`  
		Last Modified: Fri, 02 Sep 2022 04:46:48 GMT  
		Size: 3.4 MB (3387844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d47e1f12d9061d2873d9c60f1a8994a2c6caad46a876f0770ecf8e0e76d2f6c9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46456575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:046ee271c995217b16c2b683d8ebb2fd39ceafee110313d8835f9d7e5a71539f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:49:54 GMT
ADD file:eb82827919ea73f9595d7b0b70fe9aa5ff23e16ea6a87f7f9ef4e1905857b789 in / 
# Thu, 01 Sep 2022 23:49:56 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:34:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:35:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:891f6400ce611ee5975f04ad6d2c68305c76a8628b846df1b1f9ac7c45b1311c`  
		Last Modified: Thu, 01 Sep 2022 23:52:11 GMT  
		Size: 33.3 MB (33295624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c38e8344eceb4e722b9d2cc7cf0d2cdca38bb2870c652f545c8ea652efa4f6`  
		Last Modified: Fri, 02 Sep 2022 03:55:42 GMT  
		Size: 8.7 MB (8704791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059cb2841292be0e2908a7c8f78a0db3f136154b78b70a9881535c8c1080dc3f`  
		Last Modified: Fri, 02 Sep 2022 03:55:41 GMT  
		Size: 4.5 MB (4456160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:ab0b4e710273e638ba716aedb8a727f3b67f94ddaa5ad6f5a9d494cf30423b20
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34132358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bbe2f4f13bcb67f1b8b3ba8c4b939fab6dd3106951388314174f8343a01c67f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:09:50 GMT
ADD file:3f3a2d77633db008f6d929f63880dab6bd20eab1e346e715331cc1b32a9d9821 in / 
# Fri, 02 Sep 2022 00:09:51 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 00:59:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 01:00:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6cbb7395a087ad86b87360ff9e4682ac013d19b01b368e0d658aa360440c9e0f`  
		Last Modified: Fri, 02 Sep 2022 00:26:57 GMT  
		Size: 24.2 MB (24243281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da12dcd490d59114c83ba58a7ebb7af8cd20209af19b95285772857279ba9bb3`  
		Last Modified: Fri, 02 Sep 2022 01:48:06 GMT  
		Size: 6.7 MB (6744222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33395e6e037105cb40bc74d80f9d435cd4770ecc1fbeedd173dd4422aaacc2ee`  
		Last Modified: Fri, 02 Sep 2022 01:48:00 GMT  
		Size: 3.1 MB (3144855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:60896cc7f8a1ca84de78ac668cbd48eae132398b8df15d631a211d02450910a6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (37985463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97f45ed43266896cb111d1ed39d77f6d9b84486fac419d2a02bc39d1cd023139`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:13 GMT
ADD file:75a78d9ec31ac5486bdde3e48ebfc534089c5f38f14850243c2ab2e632f0bbe5 in / 
# Fri, 02 Sep 2022 01:03:16 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:03:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:04:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b87ab7b8bb5c2a1f34d9a2e9887fde669c33cea7428fdb048362dfa81eccaa75`  
		Last Modified: Fri, 02 Sep 2022 01:04:49 GMT  
		Size: 27.0 MB (27045282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f81ff7514526202dbe703eab1c9f1a8c08e2fdc2c2d56b949c8d1f90825e908`  
		Last Modified: Fri, 02 Sep 2022 02:15:30 GMT  
		Size: 7.4 MB (7397526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30cf575bc155da8ebabf970fa2716a48bb3789c6a3967d83d0f7583991658942`  
		Last Modified: Fri, 02 Sep 2022 02:15:30 GMT  
		Size: 3.5 MB (3542655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:20.04-scm`

```console
$ docker pull buildpack-deps@sha256:7d9bca39517f49994f28884f7b6b3efbde43df5f81d2c79e3397a858a3e137dd
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
$ docker pull buildpack-deps@sha256:cb3b6e80127a63f7e26f56e3796f245ca5a27f11bacd3a78710dd97a7b41f913
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.7 MB (100682681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcc3de2b9eab267855272f14c781d6e663b027167aec279a939c60d01e405d03`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:23:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:23:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 02:24:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aceaa9f66a60a3695a6348be449df629aed61f57a9cbd55a388bdcfa40cb27b7`  
		Last Modified: Fri, 02 Sep 2022 02:37:25 GMT  
		Size: 7.7 MB (7747479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d69e69900ca0c9eb8762e001879c1e84e29d94a2397e389440b1d8689445e5`  
		Last Modified: Fri, 02 Sep 2022 02:37:24 GMT  
		Size: 3.6 MB (3624451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:035d79e04aad5acedcb6ebd870819e030f0f1cb534d55136ac5f6087b31b39f9`  
		Last Modified: Fri, 02 Sep 2022 02:37:44 GMT  
		Size: 60.7 MB (60738066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:5d5e9c111f46caa080bcb19313e1cfe81cfd742fd3e87fec58d352eb998c0d15
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.9 MB (89876660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21de531d01800e4c366ef96d96e2348db60ea1e047073558e5ceaec1bf8d531c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 06:08:22 GMT
ADD file:685f4b5f8c1f11b6389e9f929909e1a667abf29814a7ccfb859aae287dacd7e1 in / 
# Fri, 02 Sep 2022 06:08:22 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 09:31:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 09:32:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 09:32:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:eff72fca8e1d166ddfda6ac6c409e888c95950da6c47d360a088219c0ad7ba05`  
		Last Modified: Fri, 02 Sep 2022 06:10:16 GMT  
		Size: 24.6 MB (24588743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0063ca7d240c073b50b399efe49028199e2fc1671c3d5e69e566b2b36dea9282`  
		Last Modified: Fri, 02 Sep 2022 09:41:04 GMT  
		Size: 6.7 MB (6741254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93ac5277e93cfbfa1f89a828713b7c6314babc86f222357de3141883f92a010`  
		Last Modified: Fri, 02 Sep 2022 09:41:04 GMT  
		Size: 3.1 MB (3104403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ccea48caa3d4856a1e5a5278dfb92e187166e74c5f4226090de64a520ae1f91`  
		Last Modified: Fri, 02 Sep 2022 09:41:27 GMT  
		Size: 55.4 MB (55442260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7a3530d9a72f8520c05cbf988f91c39234580a6c4d96b32ac4d7f8b80a0bafa3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.0 MB (98997581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce2158f16d69616965d544733bd68e5d2ebc2a66c7085ecbded592b9a3749fd9`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:38:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:38:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 04:39:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6667cb55d48ba4971074c7d8aa09e7b2368fb83f8ab6336c1ae53675ef8a5fdc`  
		Last Modified: Fri, 02 Sep 2022 04:46:48 GMT  
		Size: 7.6 MB (7614784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f84ae37056f7e9d12b5c5d6fbf1924cc86999a56dd4adeff2f422552b9edf08`  
		Last Modified: Fri, 02 Sep 2022 04:46:48 GMT  
		Size: 3.4 MB (3387844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8330d23b3e1d0fb7320e653a9dba9018129a28846b4d6cffdc5caa044ceee0`  
		Last Modified: Fri, 02 Sep 2022 04:47:09 GMT  
		Size: 60.8 MB (60803136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:052898d9b635e422c93fc45a17b62462438b35cfdc07758cd359a5bbed03b19c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (115986146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f181b52cc6edd4eede5610b8576eef3449ccc0e871ad1cdb3e3afd78baf6238`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:49:54 GMT
ADD file:eb82827919ea73f9595d7b0b70fe9aa5ff23e16ea6a87f7f9ef4e1905857b789 in / 
# Thu, 01 Sep 2022 23:49:56 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:34:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:35:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 03:36:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:891f6400ce611ee5975f04ad6d2c68305c76a8628b846df1b1f9ac7c45b1311c`  
		Last Modified: Thu, 01 Sep 2022 23:52:11 GMT  
		Size: 33.3 MB (33295624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c38e8344eceb4e722b9d2cc7cf0d2cdca38bb2870c652f545c8ea652efa4f6`  
		Last Modified: Fri, 02 Sep 2022 03:55:42 GMT  
		Size: 8.7 MB (8704791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059cb2841292be0e2908a7c8f78a0db3f136154b78b70a9881535c8c1080dc3f`  
		Last Modified: Fri, 02 Sep 2022 03:55:41 GMT  
		Size: 4.5 MB (4456160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cd324c0fe479474378bdfc00b7027887775d4396a082938a08a2b3f8163431`  
		Last Modified: Fri, 02 Sep 2022 03:56:12 GMT  
		Size: 69.5 MB (69529571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:e73ed015c1915a4a11fb634719de2f5a4f726ae247375b547314696890939979
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.0 MB (97994461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9ccb9a779d53a17e14d373934b36f3ad284f67126d248adf42298fb815e0610`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:13 GMT
ADD file:75a78d9ec31ac5486bdde3e48ebfc534089c5f38f14850243c2ab2e632f0bbe5 in / 
# Fri, 02 Sep 2022 01:03:16 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:03:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:04:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 02:04:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b87ab7b8bb5c2a1f34d9a2e9887fde669c33cea7428fdb048362dfa81eccaa75`  
		Last Modified: Fri, 02 Sep 2022 01:04:49 GMT  
		Size: 27.0 MB (27045282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f81ff7514526202dbe703eab1c9f1a8c08e2fdc2c2d56b949c8d1f90825e908`  
		Last Modified: Fri, 02 Sep 2022 02:15:30 GMT  
		Size: 7.4 MB (7397526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30cf575bc155da8ebabf970fa2716a48bb3789c6a3967d83d0f7583991658942`  
		Last Modified: Fri, 02 Sep 2022 02:15:30 GMT  
		Size: 3.5 MB (3542655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:423b3fa0fb4a3902e95b623da0004da02d690cf894720b6584469c6c7709e39a`  
		Last Modified: Fri, 02 Sep 2022 02:15:48 GMT  
		Size: 60.0 MB (60008998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.04`

```console
$ docker pull buildpack-deps@sha256:f5f73722f168030ecf95375fb039e764f70a8766f4ffea76682aa2741c9abbe9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:22.04` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:5ea27ebb2fabdd092d8cb56379f17e558c323730e82c5f47e472d369221608ec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.0 MB (249957836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24b6b43211e8cb703aecf97a92e81db48963dcee1b9fb2ef3692bf22762eeb6c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:27:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:28:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 02:28:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:31:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:728cfcfa2f7739d87ae3efda60d01680593fcb2b55fdb5840721012c19335b9a`  
		Last Modified: Fri, 02 Sep 2022 02:38:25 GMT  
		Size: 3.8 MB (3804276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09eda6154af3733cdc766a287039ebbd0d78265b3a7c64ed165045c8849ba1ce`  
		Last Modified: Fri, 02 Sep 2022 02:38:25 GMT  
		Size: 3.6 MB (3560674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a6e6f57df0f885a7603852f5ee2e183c2961cb80d1785032449ad7a31e61ffe`  
		Last Modified: Fri, 02 Sep 2022 02:38:40 GMT  
		Size: 39.3 MB (39338193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69cee3392ebf3b497e43558b59aa5f76c60fc10b2eaf5409de9a941f6dd42ca`  
		Last Modified: Fri, 02 Sep 2022 02:39:13 GMT  
		Size: 172.8 MB (172827987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:87ee84eb8872003687e4599ccc21153aa24f6b8a8558e31b825ab923a5b0fbbb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.6 MB (216605721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a70dc2d9a61ffa7c73f46bd7f5fc0351a4b4582af1b71a777935419f36329ed`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 06:08:32 GMT
ADD file:8b109e7521f26505639a07128de43f93636fcc05ecf26c6358f893f22df38acd in / 
# Fri, 02 Sep 2022 06:08:32 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 09:33:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 09:34:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 09:34:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 09:35:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:af25ea170fdc3ef953710312fcb7b9706eae0149cf05cd81c8281f1c511208bb`  
		Last Modified: Fri, 02 Sep 2022 06:10:34 GMT  
		Size: 27.0 MB (27016783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9398b18a454e124e1f9b5c08d3b8e75027704cf5d81734f403a4852babda0c9e`  
		Last Modified: Fri, 02 Sep 2022 09:42:10 GMT  
		Size: 3.6 MB (3556228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19d83ea0962e81d21c528b9d3bcf4646473a26fe96198cbc633813df2ce7583`  
		Last Modified: Fri, 02 Sep 2022 09:42:09 GMT  
		Size: 3.7 MB (3713683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:456bac4459d3361e1c563bc2e25e0a8f45ce5407f38a18250e9f40e4286be0f2`  
		Last Modified: Fri, 02 Sep 2022 09:42:29 GMT  
		Size: 41.9 MB (41906676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d843b879ac3e2cefa8c53e242aed65d5707151f67433a317e8f836519a2625`  
		Last Modified: Fri, 02 Sep 2022 09:43:01 GMT  
		Size: 140.4 MB (140412351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:419bb1f78244b8b824e28585007ee5603f88acdc520bae8aa8cfbb0869decf02
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.8 MB (240781696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44bca26c57eec16b1355ce87898fd1e703eac1d052e182d9b44a2ef861fe8fa0`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:40:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:40:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 04:41:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:41:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a5013832a9b04a455a3aed1888a43489d8850d9810b8d8fb64744bf814a1d9d`  
		Last Modified: Fri, 02 Sep 2022 04:47:52 GMT  
		Size: 3.8 MB (3776579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00e6a48d7146e6e81a25ce023cb7fb060f7cc202d4d5a9da4bc632e5ac4e05e`  
		Last Modified: Fri, 02 Sep 2022 04:47:52 GMT  
		Size: 3.3 MB (3320662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb48a8c04a0b3dd9a3bfc932ba13906c14770d53cf3bec49dca7acf27f47e0e`  
		Last Modified: Fri, 02 Sep 2022 04:48:09 GMT  
		Size: 39.2 MB (39242094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd94762a4fff6f6574e2054c323e06d6605fc3b0ac948910a65ca6f4b2c16a6e`  
		Last Modified: Fri, 02 Sep 2022 04:48:43 GMT  
		Size: 166.1 MB (166061021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:4c0eb3540a84187cfb3276069e433ed35064a1ed0fc241449621d528a813847b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.8 MB (271782797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9c1de0666ea737305d554a340f11a9c475745fa6e7a42cb195f6bb15c837b57`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:50:09 GMT
ADD file:39b6fa94f6e1300a6fc4b6094e8250c22ecaa6e7c9f934841765d45b919402c5 in / 
# Thu, 01 Sep 2022 23:50:11 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:40:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:40:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 03:41:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:45:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9ef77d5e46df05bf9f34e5871097fd038295a2aa5e29f1806ac3a96aa2545b5f`  
		Last Modified: Thu, 01 Sep 2022 23:52:34 GMT  
		Size: 35.7 MB (35721187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47f3136401182e4158ce50b7b80ede159c628447df84c97f8d16a1fdef5ca73f`  
		Last Modified: Fri, 02 Sep 2022 03:57:16 GMT  
		Size: 4.3 MB (4276033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed57522d1a954e636dbd623f4d22053a0339d16dbc9ce851739f5318e9fd3ad`  
		Last Modified: Fri, 02 Sep 2022 03:57:16 GMT  
		Size: 4.2 MB (4233890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70892ee50c4d77a318fa001df485f8ea6208582b0aa6835eb223cd0c249d1e05`  
		Last Modified: Fri, 02 Sep 2022 03:57:39 GMT  
		Size: 43.8 MB (43760153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:885ac7b7aa4ea854597160aa477647cfd9dbdcc9c5121b1bf62bb68af66ab142`  
		Last Modified: Fri, 02 Sep 2022 03:58:35 GMT  
		Size: 183.8 MB (183791534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:a3a808d8c587c5bfa6527b3fd76f9931de150a4a5b913a182f85b77df7f610a5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.9 MB (274912769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8375021379599486ff37858cacbc9dbcbecea3af36a87f33f667a9c6c26418e3`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:11:51 GMT
ADD file:8cff03722326c5e90e26ae259bde7ddd223c466edfd0d1cd6335b7b550f8156c in / 
# Fri, 02 Sep 2022 00:11:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 01:02:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 01:03:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 01:07:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 01:13:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f04a8971a8d913388890f40190f4d3935404b38efd860b235cf5d4de20959061`  
		Last Modified: Fri, 02 Sep 2022 00:29:20 GMT  
		Size: 27.7 MB (27744005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c893dcd3d9a55418817428155b89e044a2ebfddfa13d6945d70f0e2830099015`  
		Last Modified: Fri, 02 Sep 2022 01:49:29 GMT  
		Size: 3.6 MB (3615909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8351e367bac61d27e9f493ab2fdd756510203f5c595c3c81d6b96d2ac3214ca`  
		Last Modified: Fri, 02 Sep 2022 01:49:27 GMT  
		Size: 3.8 MB (3778105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78cf99d2fae932ddb826d79cfc1fb3069f811bbf8ec7c13a8c03db4b519f566e`  
		Last Modified: Fri, 02 Sep 2022 01:51:48 GMT  
		Size: 42.1 MB (42110525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643cf35c08de9ab511d3bbe352a3dfc7a6c22bb4b6d9c5ae72acd28c346d4599`  
		Last Modified: Fri, 02 Sep 2022 01:58:56 GMT  
		Size: 197.7 MB (197664225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:fb22e95706a5a0e12f4a5df9d0b4f43e090e63050a62cd6b2f81d9d13cb999db
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.7 MB (223654390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af9e578eb33342a177899cd08037bc3c789443a018966b250d40eb3eb60cc51d`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:25 GMT
ADD file:aabc057fd7b1b1f9b4b729222b6dc90e98f846a65bfee1ee57cc899b6cee5a10 in / 
# Fri, 02 Sep 2022 01:03:28 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:06:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:07:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 02:07:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:09:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a32e6a15a6635185097921b9d08997d505b6b6500b6c142ad8e718d87c45ffad`  
		Last Modified: Fri, 02 Sep 2022 01:05:01 GMT  
		Size: 28.6 MB (28643161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba21c1eef45ab363d5dcc84511ca01cdbbe1e6dfdf54dcd8b108e256251e6e5`  
		Last Modified: Fri, 02 Sep 2022 02:16:20 GMT  
		Size: 3.8 MB (3809432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b26595dd670dde31a9dd83588e0dd3408a0d7f51791314f04652f5117a00332`  
		Last Modified: Fri, 02 Sep 2022 02:16:20 GMT  
		Size: 3.5 MB (3471859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b7719a0d5c7493ffa972e138dfd13f216a4e6bbde7a2e90e46cc1d8e2f365f7`  
		Last Modified: Fri, 02 Sep 2022 02:16:32 GMT  
		Size: 39.3 MB (39294502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f983860f6aa64e4e4ad14f4559ce0d12f350ba744092c39c776c39410f60fd`  
		Last Modified: Fri, 02 Sep 2022 02:16:57 GMT  
		Size: 148.4 MB (148435436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.04-curl`

```console
$ docker pull buildpack-deps@sha256:5172cc3839a41474139e50c1d84e15439b41fb3eff707528a28d47ba64f40f73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:22.04-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:8b8f7edeac757b1a514d89c5f6e4082b9f64b1aeb87eeaa31da58dbe9e424ff6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37791656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32d70c81850c25c6f5bf209fbcc9e0b2732e5456ebcaf907d4a139b4e73eb4e7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:27:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:28:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:728cfcfa2f7739d87ae3efda60d01680593fcb2b55fdb5840721012c19335b9a`  
		Last Modified: Fri, 02 Sep 2022 02:38:25 GMT  
		Size: 3.8 MB (3804276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09eda6154af3733cdc766a287039ebbd0d78265b3a7c64ed165045c8849ba1ce`  
		Last Modified: Fri, 02 Sep 2022 02:38:25 GMT  
		Size: 3.6 MB (3560674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:4d5dd081b0038052e395515e2ca6703d1e57c62554368d3d2cb63687fab789ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34286694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca6129cb72bf260d31e0bf82e24d1444ba54d6a83c741657ebeb73c543f11b6c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 06:08:32 GMT
ADD file:8b109e7521f26505639a07128de43f93636fcc05ecf26c6358f893f22df38acd in / 
# Fri, 02 Sep 2022 06:08:32 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 09:33:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 09:34:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:af25ea170fdc3ef953710312fcb7b9706eae0149cf05cd81c8281f1c511208bb`  
		Last Modified: Fri, 02 Sep 2022 06:10:34 GMT  
		Size: 27.0 MB (27016783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9398b18a454e124e1f9b5c08d3b8e75027704cf5d81734f403a4852babda0c9e`  
		Last Modified: Fri, 02 Sep 2022 09:42:10 GMT  
		Size: 3.6 MB (3556228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19d83ea0962e81d21c528b9d3bcf4646473a26fe96198cbc633813df2ce7583`  
		Last Modified: Fri, 02 Sep 2022 09:42:09 GMT  
		Size: 3.7 MB (3713683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:0178fb33c3d226148c4bf4c01d1d7af7995549d4263e44af2da6673ef6604412
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 MB (35478581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9ee4edf34b38bd4fb5d9c8d2833b2f34145eb1ba7fe01817cc0ea98024a9ce7`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:40:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:40:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a5013832a9b04a455a3aed1888a43489d8850d9810b8d8fb64744bf814a1d9d`  
		Last Modified: Fri, 02 Sep 2022 04:47:52 GMT  
		Size: 3.8 MB (3776579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00e6a48d7146e6e81a25ce023cb7fb060f7cc202d4d5a9da4bc632e5ac4e05e`  
		Last Modified: Fri, 02 Sep 2022 04:47:52 GMT  
		Size: 3.3 MB (3320662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:2d7d4ecc910fbb54f4d2d117583d3eaa890cab38b915d426f8af153408db23c8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44231110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e89808adffacf39aa02aa62ead292356f796d3ac914b396422ee1ddad9b1c31e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:50:09 GMT
ADD file:39b6fa94f6e1300a6fc4b6094e8250c22ecaa6e7c9f934841765d45b919402c5 in / 
# Thu, 01 Sep 2022 23:50:11 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:40:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:40:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9ef77d5e46df05bf9f34e5871097fd038295a2aa5e29f1806ac3a96aa2545b5f`  
		Last Modified: Thu, 01 Sep 2022 23:52:34 GMT  
		Size: 35.7 MB (35721187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47f3136401182e4158ce50b7b80ede159c628447df84c97f8d16a1fdef5ca73f`  
		Last Modified: Fri, 02 Sep 2022 03:57:16 GMT  
		Size: 4.3 MB (4276033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed57522d1a954e636dbd623f4d22053a0339d16dbc9ce851739f5318e9fd3ad`  
		Last Modified: Fri, 02 Sep 2022 03:57:16 GMT  
		Size: 4.2 MB (4233890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:37a6e4bfff70a1d2f2343ec0bc7c5b663942e36f797247df635b8586266c5ce8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35138019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:243eb39738059da136ec1fc770b105776ec3d66b623f2e08cb79cfb2b16709fc`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:11:51 GMT
ADD file:8cff03722326c5e90e26ae259bde7ddd223c466edfd0d1cd6335b7b550f8156c in / 
# Fri, 02 Sep 2022 00:11:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 01:02:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 01:03:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f04a8971a8d913388890f40190f4d3935404b38efd860b235cf5d4de20959061`  
		Last Modified: Fri, 02 Sep 2022 00:29:20 GMT  
		Size: 27.7 MB (27744005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c893dcd3d9a55418817428155b89e044a2ebfddfa13d6945d70f0e2830099015`  
		Last Modified: Fri, 02 Sep 2022 01:49:29 GMT  
		Size: 3.6 MB (3615909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8351e367bac61d27e9f493ab2fdd756510203f5c595c3c81d6b96d2ac3214ca`  
		Last Modified: Fri, 02 Sep 2022 01:49:27 GMT  
		Size: 3.8 MB (3778105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:6a7bc5b2496502a65bad30f7cb0b243ced4eed84af1897e94b98cbc971af9aa6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35924452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59742e1d75395c6a6342d0534baf73e19ecec72302e69af41dbd4cf5ac64fe0c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:25 GMT
ADD file:aabc057fd7b1b1f9b4b729222b6dc90e98f846a65bfee1ee57cc899b6cee5a10 in / 
# Fri, 02 Sep 2022 01:03:28 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:06:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:07:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a32e6a15a6635185097921b9d08997d505b6b6500b6c142ad8e718d87c45ffad`  
		Last Modified: Fri, 02 Sep 2022 01:05:01 GMT  
		Size: 28.6 MB (28643161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba21c1eef45ab363d5dcc84511ca01cdbbe1e6dfdf54dcd8b108e256251e6e5`  
		Last Modified: Fri, 02 Sep 2022 02:16:20 GMT  
		Size: 3.8 MB (3809432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b26595dd670dde31a9dd83588e0dd3408a0d7f51791314f04652f5117a00332`  
		Last Modified: Fri, 02 Sep 2022 02:16:20 GMT  
		Size: 3.5 MB (3471859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.04-scm`

```console
$ docker pull buildpack-deps@sha256:a284bfd63ad1a58b6343d35d413e96afa505de655ec6837c303aa63ec23aea19
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:22.04-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:69a05e44c60e1a1002f2d9699f0418c640a3eadc89dcdfc9dbe87db7e7d87887
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77129849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bdf3fac9b188e20ef79a7c6f6472d57ed6eaca4b923b16dfef3262552e212d7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:27:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:28:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 02:28:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:728cfcfa2f7739d87ae3efda60d01680593fcb2b55fdb5840721012c19335b9a`  
		Last Modified: Fri, 02 Sep 2022 02:38:25 GMT  
		Size: 3.8 MB (3804276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09eda6154af3733cdc766a287039ebbd0d78265b3a7c64ed165045c8849ba1ce`  
		Last Modified: Fri, 02 Sep 2022 02:38:25 GMT  
		Size: 3.6 MB (3560674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a6e6f57df0f885a7603852f5ee2e183c2961cb80d1785032449ad7a31e61ffe`  
		Last Modified: Fri, 02 Sep 2022 02:38:40 GMT  
		Size: 39.3 MB (39338193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ce48e296266e7664e9555cd5e4797f8677173754ff8dc85cb3a78618d2569708
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76193370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed4f0c06115901299dd49788abb1b9d4e03e89e614c54efd1bf59111e763ef4a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 06:08:32 GMT
ADD file:8b109e7521f26505639a07128de43f93636fcc05ecf26c6358f893f22df38acd in / 
# Fri, 02 Sep 2022 06:08:32 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 09:33:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 09:34:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 09:34:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:af25ea170fdc3ef953710312fcb7b9706eae0149cf05cd81c8281f1c511208bb`  
		Last Modified: Fri, 02 Sep 2022 06:10:34 GMT  
		Size: 27.0 MB (27016783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9398b18a454e124e1f9b5c08d3b8e75027704cf5d81734f403a4852babda0c9e`  
		Last Modified: Fri, 02 Sep 2022 09:42:10 GMT  
		Size: 3.6 MB (3556228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19d83ea0962e81d21c528b9d3bcf4646473a26fe96198cbc633813df2ce7583`  
		Last Modified: Fri, 02 Sep 2022 09:42:09 GMT  
		Size: 3.7 MB (3713683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:456bac4459d3361e1c563bc2e25e0a8f45ce5407f38a18250e9f40e4286be0f2`  
		Last Modified: Fri, 02 Sep 2022 09:42:29 GMT  
		Size: 41.9 MB (41906676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d2a8efb0e4b21c797f51f9d1ba87902b30e30da3360c017a1666d57d2d1309e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74720675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e4a856aa72ace5cd4c58b5b1cd23888c188dc519c8a3c7bb22796e9060f64b6`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:40:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:40:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 04:41:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a5013832a9b04a455a3aed1888a43489d8850d9810b8d8fb64744bf814a1d9d`  
		Last Modified: Fri, 02 Sep 2022 04:47:52 GMT  
		Size: 3.8 MB (3776579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00e6a48d7146e6e81a25ce023cb7fb060f7cc202d4d5a9da4bc632e5ac4e05e`  
		Last Modified: Fri, 02 Sep 2022 04:47:52 GMT  
		Size: 3.3 MB (3320662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb48a8c04a0b3dd9a3bfc932ba13906c14770d53cf3bec49dca7acf27f47e0e`  
		Last Modified: Fri, 02 Sep 2022 04:48:09 GMT  
		Size: 39.2 MB (39242094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:90e3ff6758a960df5271c39810f50ae7a9af8eb2dfbf402f8a895492fd8072f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.0 MB (87991263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd0871440d7a589078f05df8c44937110743203650e4920096ea0ad39d797173`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:50:09 GMT
ADD file:39b6fa94f6e1300a6fc4b6094e8250c22ecaa6e7c9f934841765d45b919402c5 in / 
# Thu, 01 Sep 2022 23:50:11 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:40:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:40:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 03:41:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9ef77d5e46df05bf9f34e5871097fd038295a2aa5e29f1806ac3a96aa2545b5f`  
		Last Modified: Thu, 01 Sep 2022 23:52:34 GMT  
		Size: 35.7 MB (35721187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47f3136401182e4158ce50b7b80ede159c628447df84c97f8d16a1fdef5ca73f`  
		Last Modified: Fri, 02 Sep 2022 03:57:16 GMT  
		Size: 4.3 MB (4276033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed57522d1a954e636dbd623f4d22053a0339d16dbc9ce851739f5318e9fd3ad`  
		Last Modified: Fri, 02 Sep 2022 03:57:16 GMT  
		Size: 4.2 MB (4233890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70892ee50c4d77a318fa001df485f8ea6208582b0aa6835eb223cd0c249d1e05`  
		Last Modified: Fri, 02 Sep 2022 03:57:39 GMT  
		Size: 43.8 MB (43760153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:5d6c843563e30ae575ac4d38b69a11a921fd690206c62ea029269dba3ca3e7d4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77248544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea8ba9156cd9a9c213f1980abf846f422f40340024a3bb644dd0e1debb94b15c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:11:51 GMT
ADD file:8cff03722326c5e90e26ae259bde7ddd223c466edfd0d1cd6335b7b550f8156c in / 
# Fri, 02 Sep 2022 00:11:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 01:02:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 01:03:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 01:07:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f04a8971a8d913388890f40190f4d3935404b38efd860b235cf5d4de20959061`  
		Last Modified: Fri, 02 Sep 2022 00:29:20 GMT  
		Size: 27.7 MB (27744005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c893dcd3d9a55418817428155b89e044a2ebfddfa13d6945d70f0e2830099015`  
		Last Modified: Fri, 02 Sep 2022 01:49:29 GMT  
		Size: 3.6 MB (3615909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8351e367bac61d27e9f493ab2fdd756510203f5c595c3c81d6b96d2ac3214ca`  
		Last Modified: Fri, 02 Sep 2022 01:49:27 GMT  
		Size: 3.8 MB (3778105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78cf99d2fae932ddb826d79cfc1fb3069f811bbf8ec7c13a8c03db4b519f566e`  
		Last Modified: Fri, 02 Sep 2022 01:51:48 GMT  
		Size: 42.1 MB (42110525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b86d03271a7cf19de9a84a6331f9ad93633a9735a1257e88ed26383a7186520f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75218954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2c746b8e411285ae4bd0c49dac958a98fba1bf3ae25edfb828548488cb80e59`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:25 GMT
ADD file:aabc057fd7b1b1f9b4b729222b6dc90e98f846a65bfee1ee57cc899b6cee5a10 in / 
# Fri, 02 Sep 2022 01:03:28 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:06:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:07:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 02:07:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a32e6a15a6635185097921b9d08997d505b6b6500b6c142ad8e718d87c45ffad`  
		Last Modified: Fri, 02 Sep 2022 01:05:01 GMT  
		Size: 28.6 MB (28643161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba21c1eef45ab363d5dcc84511ca01cdbbe1e6dfdf54dcd8b108e256251e6e5`  
		Last Modified: Fri, 02 Sep 2022 02:16:20 GMT  
		Size: 3.8 MB (3809432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b26595dd670dde31a9dd83588e0dd3408a0d7f51791314f04652f5117a00332`  
		Last Modified: Fri, 02 Sep 2022 02:16:20 GMT  
		Size: 3.5 MB (3471859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b7719a0d5c7493ffa972e138dfd13f216a4e6bbde7a2e90e46cc1d8e2f365f7`  
		Last Modified: Fri, 02 Sep 2022 02:16:32 GMT  
		Size: 39.3 MB (39294502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.10`

```console
$ docker pull buildpack-deps@sha256:c24817e44bda6ad8cc19783d2b65814fce5afa3a1b83857359d0e0d22c849e6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:22.10` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:3c95ad74f79e8e0d742dbf0b70cabffb0135dfa4a377b9191bc38aa416ba6e48
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.4 MB (259350660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d6d2926c4684f01fa0103bb24bdb1b2a93bec0dca4b41885fc0ca5e11f05fd3`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:43 GMT
ADD file:d5de90ac61ee7027aa0900efb669efa73f611463cf73ab2cfdacadf5ab9fee19 in / 
# Thu, 01 Sep 2022 23:46:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:32:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:32:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 02:32:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:35:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0b78030514e08aad79cb596ba84b18b9579e90eac0b8e0c2dec483c3da8dbee8`  
		Last Modified: Thu, 01 Sep 2022 23:48:15 GMT  
		Size: 27.4 MB (27428015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71363ea1301988ddf4ef6039b34a05a19b44a70e1ba2764e95fa0f47b3585c12`  
		Last Modified: Fri, 02 Sep 2022 02:39:23 GMT  
		Size: 6.8 MB (6779788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d261ea038a7743d40031459e01e57001571ca5986a617d9e2d3174c66d98187a`  
		Last Modified: Fri, 02 Sep 2022 02:39:23 GMT  
		Size: 3.6 MB (3633660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dee5c450c1549fab83f54e9138820f82132ebf0b50a52e7ffb97b6074e98c1b`  
		Last Modified: Fri, 02 Sep 2022 02:39:39 GMT  
		Size: 39.7 MB (39729510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf8f5804b753a7685df0f765050b72cb63d67092265ce7d2dacd3391cfa09ace`  
		Last Modified: Fri, 02 Sep 2022 02:40:13 GMT  
		Size: 181.8 MB (181779687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f6c70d3da9e107526ed57d9da0674e7e3bdcd2c3656609d1763abad413898dd8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.3 MB (222315041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76db4726c51f452cfcf90471617a6293cfa2ed57469fa660aa52c3fad7b47eca`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 06:08:44 GMT
ADD file:6fea481ddc80754c10680e7c291055af82ef815eb0fdaf745c49c4f4cdf2afa1 in / 
# Fri, 02 Sep 2022 06:08:44 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 09:35:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 09:35:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 09:36:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 09:36:59 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1f63be4c3b8fca43746377bd8a99dd9b04acdd942d8464feaae1671e6363d920`  
		Last Modified: Fri, 02 Sep 2022 06:10:58 GMT  
		Size: 25.8 MB (25845683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c94aedbe9250aab4e90e8e88c1f2af520548789812f567b90a81f67dc9145e`  
		Last Modified: Fri, 02 Sep 2022 09:43:15 GMT  
		Size: 5.9 MB (5948408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78166495a53038ebe64fd164f5d7e26607173735e8a0e096424b99f947d93cb`  
		Last Modified: Fri, 02 Sep 2022 09:43:14 GMT  
		Size: 3.8 MB (3801422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28471ad57cdb7e9e4d1bd803eae0208867737111fd76d4143f4b6120903361b7`  
		Last Modified: Fri, 02 Sep 2022 09:43:34 GMT  
		Size: 42.6 MB (42593085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd81b6de6e71e74e98034d486ef79416eeab04372473695ef4a57a2dc8dab6b4`  
		Last Modified: Fri, 02 Sep 2022 09:44:07 GMT  
		Size: 144.1 MB (144126443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:bcffca5d2875c3c5e9e2ebbae1682df46d1a2202cc72f8d63670b9e3d68e3503
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.8 MB (246828390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c63411acefb29eac5a58855779b5ce4e65910ca3242fa4cd116d30e28860fa8`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:58:02 GMT
ADD file:1b9e898b22915c14e3d83959e989e2a653148ff82c8e2a1b3dfa8035256219aa in / 
# Fri, 02 Sep 2022 00:58:02 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:42:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:42:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 04:42:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:43:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7c0b344a74c2d365a9a57a618f4a544c4e8e70f341f67973d3a22aee52a267b9`  
		Last Modified: Fri, 02 Sep 2022 01:00:04 GMT  
		Size: 26.7 MB (26663798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21ff0107faab8a809cab0821df6c069bdc690f3cda610960915bb07f0c47780`  
		Last Modified: Fri, 02 Sep 2022 04:48:55 GMT  
		Size: 6.6 MB (6603091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62edf58fe3260c89e551263ca83a26aead51b89196e35322ead3ba9023c23aed`  
		Last Modified: Fri, 02 Sep 2022 04:48:55 GMT  
		Size: 3.4 MB (3390812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df24de8e3685677e98d7d3aea7263fa8e11665eb30549c733d0760b8bdd6a28`  
		Last Modified: Fri, 02 Sep 2022 04:49:12 GMT  
		Size: 39.5 MB (39516416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a7dab39ac145cb27e46bda054f99ccfa338d3b9d323b4053bc8b9bacd5e88c`  
		Last Modified: Fri, 02 Sep 2022 04:49:47 GMT  
		Size: 170.7 MB (170654273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:aacd2841a1e442fc1a51300cf1624bb6f38dffcdff3c27fa7a1e7f942d4a3ebf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.3 MB (282251775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:015622ad1f917fcedd420ed628aa2356b7b6306b47a5885e9a81b47e602f7868`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:50:26 GMT
ADD file:79183abf8a1f4a6d4d04d73bcbe47e66f08bea9796acebd37d515855a459d132 in / 
# Thu, 01 Sep 2022 23:50:28 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:46:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:47:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 03:48:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:51:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ff717d18c49d9ec97ec3efef7dd73fe40829e1902f57d95a91516a42f69a091a`  
		Last Modified: Thu, 01 Sep 2022 23:53:03 GMT  
		Size: 32.1 MB (32082633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76c734e70f580a1e1db27a87020a89cba5ca648c7e9c85068bd42b1e3126ebe`  
		Last Modified: Fri, 02 Sep 2022 03:58:49 GMT  
		Size: 7.8 MB (7750570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09098d7e8658181028c27fff2df2b67293550987d175c5fab78075ddec7dd8ac`  
		Last Modified: Fri, 02 Sep 2022 03:58:48 GMT  
		Size: 4.4 MB (4361359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc897ebe25a803a066f6b1910e20dec6fc0162253745894a729850d1d32c57c8`  
		Last Modified: Fri, 02 Sep 2022 03:59:13 GMT  
		Size: 44.2 MB (44161167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b502c070e035bff4190a1869e54d6a3382719ec5513be9900a64d748b181aaad`  
		Last Modified: Fri, 02 Sep 2022 04:00:12 GMT  
		Size: 193.9 MB (193896046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:73bf7abfabd3ce3f80d631c8b4246bfb77cc7865a6ea4a088e1f1bcd8e898b00
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.8 MB (280785501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86d3e3d306e8b6f9c7a24e537c8ca6080ef2a051ad1d85eeb998da9e2c4ff0b1`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:14:23 GMT
ADD file:7c2ab85ecb4dc221c58ed92c05acad8d0b2ad90e46ec34c0a45fd5a5c3a9f7e2 in / 
# Fri, 02 Sep 2022 00:14:25 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 01:16:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 01:17:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 01:20:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 01:27:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:26010bd634bfca42373b6c36c189031dcce89570ea1226e9462a48d7a684240c`  
		Last Modified: Fri, 02 Sep 2022 00:32:57 GMT  
		Size: 25.6 MB (25594334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0826196a5d14cf0f019090771814dce885e1420c992b36ab31bfed7b28d86cf5`  
		Last Modified: Fri, 02 Sep 2022 02:00:23 GMT  
		Size: 5.9 MB (5930253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add19389e79fd75d5e3421d12568767855677a99cc4cfe5d50d5590034851237`  
		Last Modified: Fri, 02 Sep 2022 02:00:18 GMT  
		Size: 3.9 MB (3881273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f04e7e633bdcb9ab785ebbaa03714ef1fb30b6e9341369572e7eb655916151`  
		Last Modified: Fri, 02 Sep 2022 02:02:44 GMT  
		Size: 42.9 MB (42853430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67eaacb0aa78a362fe9ee225ee0e3ca057354904b8418793e4b7a1511e7aab3`  
		Last Modified: Fri, 02 Sep 2022 02:09:59 GMT  
		Size: 202.5 MB (202526211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a565fb5e9470fccd7e7164a3c87a5b2433fa673dc08c7e1a760184769385eb1c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.8 MB (228802204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfa992f61c6a6e4dbc5ee3ffe027303904613e78c952d7f7192bf0e5b84ed6b4`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:38 GMT
ADD file:61a0b983796cf76453cbc73a44968b8cefb9f90cc922075728432bdbdaaeb854 in / 
# Fri, 02 Sep 2022 01:03:40 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:09:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:10:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 02:10:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:12:16 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a51274124ed15147344e4d31d9378a33521faff1de175e551081c34c14db1b9f`  
		Last Modified: Fri, 02 Sep 2022 01:05:17 GMT  
		Size: 26.0 MB (25995506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a9727cdfe9e4d0ad02573de5f42a04ee40c70d014fcdffb4b684522e06d667`  
		Last Modified: Fri, 02 Sep 2022 02:17:04 GMT  
		Size: 6.5 MB (6470487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd626668509bf2d37bfd328fa211e8e7ad57c719072d9c7f1fc379bc2c187745`  
		Last Modified: Fri, 02 Sep 2022 02:17:04 GMT  
		Size: 3.6 MB (3625387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1947234f2c6685065fd711d09a80a70640e7a9c3b7521b8bbdd0c52afb85d8b5`  
		Last Modified: Fri, 02 Sep 2022 02:17:16 GMT  
		Size: 39.6 MB (39561768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74547493d0510538ad41fae3cfd6a5789215a1d753d5ea8509671d8f743cb2cf`  
		Last Modified: Fri, 02 Sep 2022 02:17:40 GMT  
		Size: 153.1 MB (153149056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.10-curl`

```console
$ docker pull buildpack-deps@sha256:fbadf017868b978bb0f183a345be3b63fb1fe70738386dfc8bb9e93d1effd5f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:22.10-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:4146f09f2e891abdc1f560cf823df40b6c3f0172adb7bf24edf74d69c22fb9e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37841463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:956194632e135c001d0e90d82f832aa6708b7d8beb963b98e27eacc4a96799bb`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:43 GMT
ADD file:d5de90ac61ee7027aa0900efb669efa73f611463cf73ab2cfdacadf5ab9fee19 in / 
# Thu, 01 Sep 2022 23:46:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:32:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:32:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0b78030514e08aad79cb596ba84b18b9579e90eac0b8e0c2dec483c3da8dbee8`  
		Last Modified: Thu, 01 Sep 2022 23:48:15 GMT  
		Size: 27.4 MB (27428015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71363ea1301988ddf4ef6039b34a05a19b44a70e1ba2764e95fa0f47b3585c12`  
		Last Modified: Fri, 02 Sep 2022 02:39:23 GMT  
		Size: 6.8 MB (6779788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d261ea038a7743d40031459e01e57001571ca5986a617d9e2d3174c66d98187a`  
		Last Modified: Fri, 02 Sep 2022 02:39:23 GMT  
		Size: 3.6 MB (3633660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:fc9add13cbee66aac1a50ef350bb1f7a61fbff4028de3ec5aa3853f52186f69f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.6 MB (35595513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19e80e45169f55fa54c17989c92f2067a23b1748bc1d414f7ad0adcc3be10c10`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 06:08:44 GMT
ADD file:6fea481ddc80754c10680e7c291055af82ef815eb0fdaf745c49c4f4cdf2afa1 in / 
# Fri, 02 Sep 2022 06:08:44 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 09:35:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 09:35:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1f63be4c3b8fca43746377bd8a99dd9b04acdd942d8464feaae1671e6363d920`  
		Last Modified: Fri, 02 Sep 2022 06:10:58 GMT  
		Size: 25.8 MB (25845683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c94aedbe9250aab4e90e8e88c1f2af520548789812f567b90a81f67dc9145e`  
		Last Modified: Fri, 02 Sep 2022 09:43:15 GMT  
		Size: 5.9 MB (5948408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78166495a53038ebe64fd164f5d7e26607173735e8a0e096424b99f947d93cb`  
		Last Modified: Fri, 02 Sep 2022 09:43:14 GMT  
		Size: 3.8 MB (3801422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7a58c082c08baa948c0393745478cfc6a621d44aa9e72c0b3e7e6c7d87fb7249
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.7 MB (36657701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ffef9f110163db57eac2f13cd57c0c78b549e7dbf112862ad7ddbbb3c863bf4`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:58:02 GMT
ADD file:1b9e898b22915c14e3d83959e989e2a653148ff82c8e2a1b3dfa8035256219aa in / 
# Fri, 02 Sep 2022 00:58:02 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:42:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:42:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:7c0b344a74c2d365a9a57a618f4a544c4e8e70f341f67973d3a22aee52a267b9`  
		Last Modified: Fri, 02 Sep 2022 01:00:04 GMT  
		Size: 26.7 MB (26663798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21ff0107faab8a809cab0821df6c069bdc690f3cda610960915bb07f0c47780`  
		Last Modified: Fri, 02 Sep 2022 04:48:55 GMT  
		Size: 6.6 MB (6603091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62edf58fe3260c89e551263ca83a26aead51b89196e35322ead3ba9023c23aed`  
		Last Modified: Fri, 02 Sep 2022 04:48:55 GMT  
		Size: 3.4 MB (3390812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:2f1739c1c6b4eac084c3655fe8a0d1f722d5234020ad66d85af3896252831c9e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44194562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb41d3ac587d6f78add9f6b9380f50796d6ba12866658651392d8f42597772c2`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:50:26 GMT
ADD file:79183abf8a1f4a6d4d04d73bcbe47e66f08bea9796acebd37d515855a459d132 in / 
# Thu, 01 Sep 2022 23:50:28 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:46:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:47:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ff717d18c49d9ec97ec3efef7dd73fe40829e1902f57d95a91516a42f69a091a`  
		Last Modified: Thu, 01 Sep 2022 23:53:03 GMT  
		Size: 32.1 MB (32082633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76c734e70f580a1e1db27a87020a89cba5ca648c7e9c85068bd42b1e3126ebe`  
		Last Modified: Fri, 02 Sep 2022 03:58:49 GMT  
		Size: 7.8 MB (7750570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09098d7e8658181028c27fff2df2b67293550987d175c5fab78075ddec7dd8ac`  
		Last Modified: Fri, 02 Sep 2022 03:58:48 GMT  
		Size: 4.4 MB (4361359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:27a5f062d5475bb7448ee24ce8540657304df8857324a254cab4b5b2f88a6995
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.4 MB (35405860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9316adf029fa960eedaf5a870e8ea5d065e27ffc98ed3823c735853fdfc69086`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:14:23 GMT
ADD file:7c2ab85ecb4dc221c58ed92c05acad8d0b2ad90e46ec34c0a45fd5a5c3a9f7e2 in / 
# Fri, 02 Sep 2022 00:14:25 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 01:16:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 01:17:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:26010bd634bfca42373b6c36c189031dcce89570ea1226e9462a48d7a684240c`  
		Last Modified: Fri, 02 Sep 2022 00:32:57 GMT  
		Size: 25.6 MB (25594334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0826196a5d14cf0f019090771814dce885e1420c992b36ab31bfed7b28d86cf5`  
		Last Modified: Fri, 02 Sep 2022 02:00:23 GMT  
		Size: 5.9 MB (5930253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add19389e79fd75d5e3421d12568767855677a99cc4cfe5d50d5590034851237`  
		Last Modified: Fri, 02 Sep 2022 02:00:18 GMT  
		Size: 3.9 MB (3881273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:1a4280bfe4ba337a4d6823ed783b787f4e47c972297bdc1fb87365481d92e6b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.1 MB (36091380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95fe882ebed7bf4928fe0c8bb698fbd2717de58f157144268dc3bf5a5bf74767`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:38 GMT
ADD file:61a0b983796cf76453cbc73a44968b8cefb9f90cc922075728432bdbdaaeb854 in / 
# Fri, 02 Sep 2022 01:03:40 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:09:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:10:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a51274124ed15147344e4d31d9378a33521faff1de175e551081c34c14db1b9f`  
		Last Modified: Fri, 02 Sep 2022 01:05:17 GMT  
		Size: 26.0 MB (25995506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a9727cdfe9e4d0ad02573de5f42a04ee40c70d014fcdffb4b684522e06d667`  
		Last Modified: Fri, 02 Sep 2022 02:17:04 GMT  
		Size: 6.5 MB (6470487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd626668509bf2d37bfd328fa211e8e7ad57c719072d9c7f1fc379bc2c187745`  
		Last Modified: Fri, 02 Sep 2022 02:17:04 GMT  
		Size: 3.6 MB (3625387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.10-scm`

```console
$ docker pull buildpack-deps@sha256:acb0852335a3ebd50b51b14fbfb92eb19a1b99f55dcc4bdfadb2195e8ee5939c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:22.10-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:828ba173c64d2b06cfab5015d103cacabaf810768a3edebde3bc29cbdc44e5b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.6 MB (77570973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdf0e5aaa1e96e04823419e7cc270da44b5ef7482b69063331a8f8dc4851ba7f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:43 GMT
ADD file:d5de90ac61ee7027aa0900efb669efa73f611463cf73ab2cfdacadf5ab9fee19 in / 
# Thu, 01 Sep 2022 23:46:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:32:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:32:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 02:32:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0b78030514e08aad79cb596ba84b18b9579e90eac0b8e0c2dec483c3da8dbee8`  
		Last Modified: Thu, 01 Sep 2022 23:48:15 GMT  
		Size: 27.4 MB (27428015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71363ea1301988ddf4ef6039b34a05a19b44a70e1ba2764e95fa0f47b3585c12`  
		Last Modified: Fri, 02 Sep 2022 02:39:23 GMT  
		Size: 6.8 MB (6779788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d261ea038a7743d40031459e01e57001571ca5986a617d9e2d3174c66d98187a`  
		Last Modified: Fri, 02 Sep 2022 02:39:23 GMT  
		Size: 3.6 MB (3633660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dee5c450c1549fab83f54e9138820f82132ebf0b50a52e7ffb97b6074e98c1b`  
		Last Modified: Fri, 02 Sep 2022 02:39:39 GMT  
		Size: 39.7 MB (39729510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:cfd3f516f9db19a7d0a3397bd2a4556f9fe1196d887519954a604ed38c08ae24
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.2 MB (78188598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b6c836955c987cb709f3f744b01bd49e876b7dfdfddb548a7b840351c8452b0`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 06:08:44 GMT
ADD file:6fea481ddc80754c10680e7c291055af82ef815eb0fdaf745c49c4f4cdf2afa1 in / 
# Fri, 02 Sep 2022 06:08:44 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 09:35:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 09:35:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 09:36:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1f63be4c3b8fca43746377bd8a99dd9b04acdd942d8464feaae1671e6363d920`  
		Last Modified: Fri, 02 Sep 2022 06:10:58 GMT  
		Size: 25.8 MB (25845683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c94aedbe9250aab4e90e8e88c1f2af520548789812f567b90a81f67dc9145e`  
		Last Modified: Fri, 02 Sep 2022 09:43:15 GMT  
		Size: 5.9 MB (5948408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78166495a53038ebe64fd164f5d7e26607173735e8a0e096424b99f947d93cb`  
		Last Modified: Fri, 02 Sep 2022 09:43:14 GMT  
		Size: 3.8 MB (3801422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28471ad57cdb7e9e4d1bd803eae0208867737111fd76d4143f4b6120903361b7`  
		Last Modified: Fri, 02 Sep 2022 09:43:34 GMT  
		Size: 42.6 MB (42593085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:e3b5b4e76e7beab59040a6636f56d76d7503606a20e63a3e2f9ea2a8bb6ac29d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76174117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2b653827e5a547aa259b9c8b69823046c120471f9a42d4cb3c39bfce50ac697`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:58:02 GMT
ADD file:1b9e898b22915c14e3d83959e989e2a653148ff82c8e2a1b3dfa8035256219aa in / 
# Fri, 02 Sep 2022 00:58:02 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:42:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:42:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 04:42:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7c0b344a74c2d365a9a57a618f4a544c4e8e70f341f67973d3a22aee52a267b9`  
		Last Modified: Fri, 02 Sep 2022 01:00:04 GMT  
		Size: 26.7 MB (26663798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21ff0107faab8a809cab0821df6c069bdc690f3cda610960915bb07f0c47780`  
		Last Modified: Fri, 02 Sep 2022 04:48:55 GMT  
		Size: 6.6 MB (6603091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62edf58fe3260c89e551263ca83a26aead51b89196e35322ead3ba9023c23aed`  
		Last Modified: Fri, 02 Sep 2022 04:48:55 GMT  
		Size: 3.4 MB (3390812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df24de8e3685677e98d7d3aea7263fa8e11665eb30549c733d0760b8bdd6a28`  
		Last Modified: Fri, 02 Sep 2022 04:49:12 GMT  
		Size: 39.5 MB (39516416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d1a0061871614fa08a0672d33b54065a27d2ac2e6fddb89f4b8d50f90beebb10
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.4 MB (88355729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb4218919910d1defe9ce53d3c83bc3ee4351f723a43693566be868052037c8d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:50:26 GMT
ADD file:79183abf8a1f4a6d4d04d73bcbe47e66f08bea9796acebd37d515855a459d132 in / 
# Thu, 01 Sep 2022 23:50:28 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:46:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:47:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 03:48:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ff717d18c49d9ec97ec3efef7dd73fe40829e1902f57d95a91516a42f69a091a`  
		Last Modified: Thu, 01 Sep 2022 23:53:03 GMT  
		Size: 32.1 MB (32082633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76c734e70f580a1e1db27a87020a89cba5ca648c7e9c85068bd42b1e3126ebe`  
		Last Modified: Fri, 02 Sep 2022 03:58:49 GMT  
		Size: 7.8 MB (7750570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09098d7e8658181028c27fff2df2b67293550987d175c5fab78075ddec7dd8ac`  
		Last Modified: Fri, 02 Sep 2022 03:58:48 GMT  
		Size: 4.4 MB (4361359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc897ebe25a803a066f6b1910e20dec6fc0162253745894a729850d1d32c57c8`  
		Last Modified: Fri, 02 Sep 2022 03:59:13 GMT  
		Size: 44.2 MB (44161167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:0ecd3a16684ad715fdc64797dcb67e50a578b932508e659b89877e29aeb60c31
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78259290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3eebb88c0344c66b13bb1996a4cd968b97228457505a37dac024aed53fc270e0`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:14:23 GMT
ADD file:7c2ab85ecb4dc221c58ed92c05acad8d0b2ad90e46ec34c0a45fd5a5c3a9f7e2 in / 
# Fri, 02 Sep 2022 00:14:25 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 01:16:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 01:17:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 01:20:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:26010bd634bfca42373b6c36c189031dcce89570ea1226e9462a48d7a684240c`  
		Last Modified: Fri, 02 Sep 2022 00:32:57 GMT  
		Size: 25.6 MB (25594334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0826196a5d14cf0f019090771814dce885e1420c992b36ab31bfed7b28d86cf5`  
		Last Modified: Fri, 02 Sep 2022 02:00:23 GMT  
		Size: 5.9 MB (5930253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add19389e79fd75d5e3421d12568767855677a99cc4cfe5d50d5590034851237`  
		Last Modified: Fri, 02 Sep 2022 02:00:18 GMT  
		Size: 3.9 MB (3881273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f04e7e633bdcb9ab785ebbaa03714ef1fb30b6e9341369572e7eb655916151`  
		Last Modified: Fri, 02 Sep 2022 02:02:44 GMT  
		Size: 42.9 MB (42853430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:f129e4299698e3c5c9ab8769330e17dd80fdc69e682f5705ef355e75dfc32ff8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75653148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:505a854970b8539945a41a684cd6895a2b377733c46184f17c584767122c2b75`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:38 GMT
ADD file:61a0b983796cf76453cbc73a44968b8cefb9f90cc922075728432bdbdaaeb854 in / 
# Fri, 02 Sep 2022 01:03:40 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:09:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:10:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 02:10:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a51274124ed15147344e4d31d9378a33521faff1de175e551081c34c14db1b9f`  
		Last Modified: Fri, 02 Sep 2022 01:05:17 GMT  
		Size: 26.0 MB (25995506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a9727cdfe9e4d0ad02573de5f42a04ee40c70d014fcdffb4b684522e06d667`  
		Last Modified: Fri, 02 Sep 2022 02:17:04 GMT  
		Size: 6.5 MB (6470487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd626668509bf2d37bfd328fa211e8e7ad57c719072d9c7f1fc379bc2c187745`  
		Last Modified: Fri, 02 Sep 2022 02:17:04 GMT  
		Size: 3.6 MB (3625387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1947234f2c6685065fd711d09a80a70640e7a9c3b7521b8bbdd0c52afb85d8b5`  
		Last Modified: Fri, 02 Sep 2022 02:17:16 GMT  
		Size: 39.6 MB (39561768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bionic`

```console
$ docker pull buildpack-deps@sha256:9ac27efda917198bf27efc5793d8149435ee00736bba49926fc8a654f5c356a3
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
$ docker pull buildpack-deps@sha256:e528083f16c11b7887692e4e3c95c3a6870518320b2f58540dd7bbe969c6d1b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.4 MB (221392214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5aed41ef81bfee2777d4de5e91ad756fef93503d0700fc0dacc473d761971818`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 19:38:36 GMT
ADD file:8733c7e8faf03d53cb2143ff6ac405362944cfa07422fccd21a3066cc2f42c83 in / 
# Tue, 06 Sep 2022 19:38:37 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:56:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:56:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Sep 2022 19:56:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:59:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:726b8a513d66e3585eb57389171d97fcd348e4914a415891e1da135b85ffa6c3`  
		Last Modified: Fri, 02 Sep 2022 15:41:13 GMT  
		Size: 26.7 MB (26710833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7dbb4551b9c872b2053c38cdd5dd7e02c06107e648b950551a585e5e88394c7`  
		Last Modified: Tue, 06 Sep 2022 20:00:54 GMT  
		Size: 6.6 MB (6630965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79cc7a6dc37d1b46bb3edb182f0a133c77f677de31779964db5569d6137a99d`  
		Last Modified: Tue, 06 Sep 2022 20:00:54 GMT  
		Size: 3.0 MB (3023688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5b4b52eebf079a3d5e1a1decad6af97acccd018f5d50a4c0e9533a54a3cdbc`  
		Last Modified: Tue, 06 Sep 2022 20:01:11 GMT  
		Size: 45.5 MB (45498322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4c3ab92be332905d30314f7e4fc0775d75a34044a859f49564b40fe4e7cffc`  
		Last Modified: Tue, 06 Sep 2022 20:01:40 GMT  
		Size: 139.5 MB (139528406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:0fce3a21c1614e61a642bf5a439ac1770eb692c003e2ae3e08a76e619291b0d0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.6 MB (189556723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e2da3dee6e14720f0c8cb851fba01ac825f58712778a0f763864eeaa456d206`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 19:33:23 GMT
ADD file:45c82fca220161f3905a06e276f12ec0cb3be5c099cca70bb6d495da10088f7d in / 
# Tue, 06 Sep 2022 19:33:24 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:51:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:52:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Sep 2022 19:52:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:53:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:074d633b5bde02245e333b110dde5850e06ea4ebefe4283af6e4dfd8d462b170`  
		Last Modified: Tue, 06 Sep 2022 19:35:07 GMT  
		Size: 22.3 MB (22305954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594729c31c2cb7f63b20f449c44c215064e068c94731174e4b57603ce032fd82`  
		Last Modified: Tue, 06 Sep 2022 19:57:06 GMT  
		Size: 5.7 MB (5698254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da759356c74e12ad90a263cb412b2ea0620a103ffedbdb492aac5586d59cdb83`  
		Last Modified: Tue, 06 Sep 2022 19:57:05 GMT  
		Size: 2.6 MB (2585972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31889323a628fc6a5d5b97236ff7b9500b05e2cafa958463ef4094646c8f3603`  
		Last Modified: Tue, 06 Sep 2022 19:57:25 GMT  
		Size: 40.7 MB (40691568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7cff271266119a86a51033715e0198a3b8755f84d2c5cca74c523f8225cc280`  
		Last Modified: Tue, 06 Sep 2022 19:57:53 GMT  
		Size: 118.3 MB (118274975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3ebaa3c12382c2516c8728bafd1ee97a069548dc91e3dc74d6867d591d5a17ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.5 MB (205513212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:931d6758b74219c522750ad62e920c8098f22702e137a5eed6754217c4556dd8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 18:49:02 GMT
ADD file:26cb5ace98a4462b36211bf28f1e73781dd6d8984350d9bd53243dbe50ae180c in / 
# Tue, 06 Sep 2022 18:49:02 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:12:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:12:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Sep 2022 19:13:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:13:59 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d30cf2a6a25aea48a115837d149468c8de7df7fb51f210b9fa1173c065f7b34c`  
		Last Modified: Tue, 06 Sep 2022 18:50:34 GMT  
		Size: 23.7 MB (23734076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79317661c5fe6a8a22ce652c9fb0999eb96ed08b735a16224e9a795c877780d`  
		Last Modified: Tue, 06 Sep 2022 19:16:57 GMT  
		Size: 6.1 MB (6072017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:737382e506f963b99b1453e20a2fcbb6bc4328a0c68bfc3530b2082a5f3da14f`  
		Last Modified: Tue, 06 Sep 2022 19:16:56 GMT  
		Size: 2.6 MB (2571091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160f71044c4c89d05d500625b4eda19add7227d613b991017a9850f2945440d2`  
		Last Modified: Tue, 06 Sep 2022 19:17:14 GMT  
		Size: 43.3 MB (43296151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ec4cd1624a82a57e6cd377e4126b4e69c04991aca1f9dd6b9380b4a351e588`  
		Last Modified: Tue, 06 Sep 2022 19:17:44 GMT  
		Size: 129.8 MB (129839877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; 386

```console
$ docker pull buildpack-deps@sha256:1e08f63aabe1e3e0539b94fb88d71d70045de1b2a09c1cb0678ae765d602281d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.2 MB (218228400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:523091bbe3ef5b646de02652ba174944425c430cba9e8d570d61d6936e640f7c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 18:40:06 GMT
ADD file:31701667cc90b9f4ce7d6ede94bf7dae4d63c49e62d3725094d547f9601e1165 in / 
# Tue, 06 Sep 2022 18:40:07 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:02:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:02:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Sep 2022 19:02:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:04:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10d3032d1995d3163c20a7f2f197299fae258c2ad020a8fd586fd6b7dd1b0e1d`  
		Last Modified: Tue, 06 Sep 2022 18:40:53 GMT  
		Size: 27.2 MB (27164710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360b65e679bf1db70d92b45a6d39c882e074d441412548705adf35d49a12c70a`  
		Last Modified: Tue, 06 Sep 2022 19:06:33 GMT  
		Size: 6.9 MB (6919740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8820513ab0577fe6133989b66cdc2a5a0b1a97af5280746721af55657c0897d7`  
		Last Modified: Tue, 06 Sep 2022 19:06:32 GMT  
		Size: 3.0 MB (3039943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ad90e9fc8930485dc12eedaf8101fe62b983d943986b7325ff502b9d424d75`  
		Last Modified: Tue, 06 Sep 2022 19:06:52 GMT  
		Size: 47.1 MB (47083595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bdffbbc9ce11b7acde16175dcc810b3cd9c5e5f850cac91cfcd033e2c2bcf9`  
		Last Modified: Tue, 06 Sep 2022 19:07:20 GMT  
		Size: 134.0 MB (134020412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:ac71ffe284d77165ccbfe8e4f10276653fde3026f002fc1e2a5557fba36cdfe1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.4 MB (246400050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddcce9c6043a6417a17152dbbefebdc2086e1240454861f17bfdd701a73c7c6f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 19:38:57 GMT
ADD file:1b76d0a41921afefb92711c44ceb312c16828d433b689a951d65c238faa9ac50 in / 
# Tue, 06 Sep 2022 19:38:59 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 20:06:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 20:06:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Sep 2022 20:07:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 20:09:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4abf8f40556a940861bc7fc313acefb89c775273ed06b7d41cfb222ccf8a1438`  
		Last Modified: Tue, 06 Sep 2022 19:40:56 GMT  
		Size: 30.4 MB (30441623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7afd3028934ff054bca1d0bb218e690d2cdb60f7754ad3bb6426c3744e730f`  
		Last Modified: Tue, 06 Sep 2022 20:12:44 GMT  
		Size: 7.1 MB (7050146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33850c25587eb4418b5e6aeccf1c9e6fa5b0baac624020bc56b4d4db8c2742c5`  
		Last Modified: Tue, 06 Sep 2022 20:12:43 GMT  
		Size: 3.7 MB (3720231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677c4d750793a0cab4cd23689261d167383d4e03f7fce03417017fcfd5497d21`  
		Last Modified: Tue, 06 Sep 2022 20:13:12 GMT  
		Size: 53.7 MB (53744408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2548f24520c161a34a9b39bc85562ec79da91528e4742bfafd4dc333ae3b0489`  
		Last Modified: Tue, 06 Sep 2022 20:14:01 GMT  
		Size: 151.4 MB (151443642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:00d5ff189772c956744ca48d4cb80e449ce51e844a304eb5336ed8ff5a1c96d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.7 MB (205748449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d78f4436f2d6ebf559f756716d8782d1472e28502b39ffdd40c045b74f4ea2f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 18:43:36 GMT
ADD file:dbe2a8e3943129e654ee29c636cab2bb10dd7eb0ac27d51e6954af2ccbe22807 in / 
# Tue, 06 Sep 2022 18:43:37 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:11:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:11:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Sep 2022 19:12:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:13:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be6761156800c616810cb8aeb5b3ae71b9a2082f1c1221210befe119f082e879`  
		Last Modified: Tue, 06 Sep 2022 18:45:00 GMT  
		Size: 25.4 MB (25370130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae409e724954611ea7731639a0dab7c4c59fdb64deb51dba5327bc8c5a085c5f`  
		Last Modified: Tue, 06 Sep 2022 19:17:11 GMT  
		Size: 6.3 MB (6324234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aca3edc7c631417c9e3dbbcb30698aed6531dc2482e10dd41ee221de2d450ca5`  
		Last Modified: Tue, 06 Sep 2022 19:17:11 GMT  
		Size: 3.0 MB (2977166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee7b8f6dba5690621ef3c6a174a056a9b68be9f2c37eeb155bc990d0284bcf0`  
		Last Modified: Tue, 06 Sep 2022 19:17:26 GMT  
		Size: 45.0 MB (45043901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:654a99a01d5150ba8cc8996260cf51a2b5c4a95e746908bcf7f69f1a719549ac`  
		Last Modified: Tue, 06 Sep 2022 19:17:50 GMT  
		Size: 126.0 MB (126033018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bionic-curl`

```console
$ docker pull buildpack-deps@sha256:dcb2d54836f9a7ca1639cd4fd498925e854cfe0a2789eeac075e825d4ec55dd7
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
$ docker pull buildpack-deps@sha256:fb84bfba9252ad0cad4bf624e06d1c893d3b1a7f55e3cc37aa605f5a67d9441d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36365486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64c992125c0697acbdc18105c298d44b3c5e089b2fdfaef91658643be66c77d1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 19:38:36 GMT
ADD file:8733c7e8faf03d53cb2143ff6ac405362944cfa07422fccd21a3066cc2f42c83 in / 
# Tue, 06 Sep 2022 19:38:37 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:56:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:56:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:726b8a513d66e3585eb57389171d97fcd348e4914a415891e1da135b85ffa6c3`  
		Last Modified: Fri, 02 Sep 2022 15:41:13 GMT  
		Size: 26.7 MB (26710833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7dbb4551b9c872b2053c38cdd5dd7e02c06107e648b950551a585e5e88394c7`  
		Last Modified: Tue, 06 Sep 2022 20:00:54 GMT  
		Size: 6.6 MB (6630965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79cc7a6dc37d1b46bb3edb182f0a133c77f677de31779964db5569d6137a99d`  
		Last Modified: Tue, 06 Sep 2022 20:00:54 GMT  
		Size: 3.0 MB (3023688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:afe6b279269826bd9d9a9b77ac80bbd54db65cc922bf5a184f06f6a396719d8e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30590180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53b82ac9f9048c0858ffaed15ca8ef98cdc38e7c07be402ef88ebaf6792962c6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 19:33:23 GMT
ADD file:45c82fca220161f3905a06e276f12ec0cb3be5c099cca70bb6d495da10088f7d in / 
# Tue, 06 Sep 2022 19:33:24 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:51:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:52:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:074d633b5bde02245e333b110dde5850e06ea4ebefe4283af6e4dfd8d462b170`  
		Last Modified: Tue, 06 Sep 2022 19:35:07 GMT  
		Size: 22.3 MB (22305954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594729c31c2cb7f63b20f449c44c215064e068c94731174e4b57603ce032fd82`  
		Last Modified: Tue, 06 Sep 2022 19:57:06 GMT  
		Size: 5.7 MB (5698254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da759356c74e12ad90a263cb412b2ea0620a103ffedbdb492aac5586d59cdb83`  
		Last Modified: Tue, 06 Sep 2022 19:57:05 GMT  
		Size: 2.6 MB (2585972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:2a7863e0c4008a73ef0bda24499179d884f903c73c1669375cb88f15c545fc25
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.4 MB (32377184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07c6a028cf3ecfd36dd9d598bbb927e84f8a27631f594cabce0272768f7bb62f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 18:49:02 GMT
ADD file:26cb5ace98a4462b36211bf28f1e73781dd6d8984350d9bd53243dbe50ae180c in / 
# Tue, 06 Sep 2022 18:49:02 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:12:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:12:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d30cf2a6a25aea48a115837d149468c8de7df7fb51f210b9fa1173c065f7b34c`  
		Last Modified: Tue, 06 Sep 2022 18:50:34 GMT  
		Size: 23.7 MB (23734076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79317661c5fe6a8a22ce652c9fb0999eb96ed08b735a16224e9a795c877780d`  
		Last Modified: Tue, 06 Sep 2022 19:16:57 GMT  
		Size: 6.1 MB (6072017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:737382e506f963b99b1453e20a2fcbb6bc4328a0c68bfc3530b2082a5f3da14f`  
		Last Modified: Tue, 06 Sep 2022 19:16:56 GMT  
		Size: 2.6 MB (2571091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:9843a4e78ba03fb07ec7138d9afdaabb3412478c44103fbca5fc8732b1a29bb8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37124393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab6063d4c02c86863842cda863cdd0b9fc41b99181a9d5bb4e10e93c58167700`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 18:40:06 GMT
ADD file:31701667cc90b9f4ce7d6ede94bf7dae4d63c49e62d3725094d547f9601e1165 in / 
# Tue, 06 Sep 2022 18:40:07 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:02:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:02:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:10d3032d1995d3163c20a7f2f197299fae258c2ad020a8fd586fd6b7dd1b0e1d`  
		Last Modified: Tue, 06 Sep 2022 18:40:53 GMT  
		Size: 27.2 MB (27164710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360b65e679bf1db70d92b45a6d39c882e074d441412548705adf35d49a12c70a`  
		Last Modified: Tue, 06 Sep 2022 19:06:33 GMT  
		Size: 6.9 MB (6919740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8820513ab0577fe6133989b66cdc2a5a0b1a97af5280746721af55657c0897d7`  
		Last Modified: Tue, 06 Sep 2022 19:06:32 GMT  
		Size: 3.0 MB (3039943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:17ba421e87b43d3709f030baae5c32ff973f324914ce189a7ec322b8d465f42c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41212000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f2cd514147c478a3ed7fabf6a7c9ce8924b524298a42b113013caf62abee8b5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 19:38:57 GMT
ADD file:1b76d0a41921afefb92711c44ceb312c16828d433b689a951d65c238faa9ac50 in / 
# Tue, 06 Sep 2022 19:38:59 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 20:06:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 20:06:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4abf8f40556a940861bc7fc313acefb89c775273ed06b7d41cfb222ccf8a1438`  
		Last Modified: Tue, 06 Sep 2022 19:40:56 GMT  
		Size: 30.4 MB (30441623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7afd3028934ff054bca1d0bb218e690d2cdb60f7754ad3bb6426c3744e730f`  
		Last Modified: Tue, 06 Sep 2022 20:12:44 GMT  
		Size: 7.1 MB (7050146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33850c25587eb4418b5e6aeccf1c9e6fa5b0baac624020bc56b4d4db8c2742c5`  
		Last Modified: Tue, 06 Sep 2022 20:12:43 GMT  
		Size: 3.7 MB (3720231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:88bdf05d087dec6348b811e7fe133c6de77ad937052d47ef17e19e9f48313d15
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34671530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1271e59da62b67faad96ae96f4a55cbfdf33568b76dbfc4820467a25e9cc5d51`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 18:43:36 GMT
ADD file:dbe2a8e3943129e654ee29c636cab2bb10dd7eb0ac27d51e6954af2ccbe22807 in / 
# Tue, 06 Sep 2022 18:43:37 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:11:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:11:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:be6761156800c616810cb8aeb5b3ae71b9a2082f1c1221210befe119f082e879`  
		Last Modified: Tue, 06 Sep 2022 18:45:00 GMT  
		Size: 25.4 MB (25370130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae409e724954611ea7731639a0dab7c4c59fdb64deb51dba5327bc8c5a085c5f`  
		Last Modified: Tue, 06 Sep 2022 19:17:11 GMT  
		Size: 6.3 MB (6324234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aca3edc7c631417c9e3dbbcb30698aed6531dc2482e10dd41ee221de2d450ca5`  
		Last Modified: Tue, 06 Sep 2022 19:17:11 GMT  
		Size: 3.0 MB (2977166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bionic-scm`

```console
$ docker pull buildpack-deps@sha256:60bf73bfe83bfe213a096d826301485d12b23121eb2cb945971b57b12d44f7f5
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
$ docker pull buildpack-deps@sha256:99364dc903d771b32e2c8c419a0a34c5d6a220dd72f1f3a56705d01c8ff04d74
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81863808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc7db731cc6dfe3ba8e4d80592a46f2869a517287d15a058d9c9d66c02583085`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 19:38:36 GMT
ADD file:8733c7e8faf03d53cb2143ff6ac405362944cfa07422fccd21a3066cc2f42c83 in / 
# Tue, 06 Sep 2022 19:38:37 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:56:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:56:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Sep 2022 19:56:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:726b8a513d66e3585eb57389171d97fcd348e4914a415891e1da135b85ffa6c3`  
		Last Modified: Fri, 02 Sep 2022 15:41:13 GMT  
		Size: 26.7 MB (26710833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7dbb4551b9c872b2053c38cdd5dd7e02c06107e648b950551a585e5e88394c7`  
		Last Modified: Tue, 06 Sep 2022 20:00:54 GMT  
		Size: 6.6 MB (6630965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79cc7a6dc37d1b46bb3edb182f0a133c77f677de31779964db5569d6137a99d`  
		Last Modified: Tue, 06 Sep 2022 20:00:54 GMT  
		Size: 3.0 MB (3023688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5b4b52eebf079a3d5e1a1decad6af97acccd018f5d50a4c0e9533a54a3cdbc`  
		Last Modified: Tue, 06 Sep 2022 20:01:11 GMT  
		Size: 45.5 MB (45498322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:b5e3fcf7ff33c0a0102f3dd8b37137429f5b2abb399fdd3287d88d2daf8387a5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71281748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:157ec7a9d18b93b9853234a51689143321a6547d2e65911c5562b7cd3e9b31f2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 19:33:23 GMT
ADD file:45c82fca220161f3905a06e276f12ec0cb3be5c099cca70bb6d495da10088f7d in / 
# Tue, 06 Sep 2022 19:33:24 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:51:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:52:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Sep 2022 19:52:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:074d633b5bde02245e333b110dde5850e06ea4ebefe4283af6e4dfd8d462b170`  
		Last Modified: Tue, 06 Sep 2022 19:35:07 GMT  
		Size: 22.3 MB (22305954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594729c31c2cb7f63b20f449c44c215064e068c94731174e4b57603ce032fd82`  
		Last Modified: Tue, 06 Sep 2022 19:57:06 GMT  
		Size: 5.7 MB (5698254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da759356c74e12ad90a263cb412b2ea0620a103ffedbdb492aac5586d59cdb83`  
		Last Modified: Tue, 06 Sep 2022 19:57:05 GMT  
		Size: 2.6 MB (2585972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31889323a628fc6a5d5b97236ff7b9500b05e2cafa958463ef4094646c8f3603`  
		Last Modified: Tue, 06 Sep 2022 19:57:25 GMT  
		Size: 40.7 MB (40691568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ff7947cce30c9ff5827fef08b8fba331fd9d6b4250e279b46dd5c95c3a6a9fbc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75673335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0910d8ecce3a327c711cb34093bb9b3c9fffef753ecae8c78456571c3564b47e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 18:49:02 GMT
ADD file:26cb5ace98a4462b36211bf28f1e73781dd6d8984350d9bd53243dbe50ae180c in / 
# Tue, 06 Sep 2022 18:49:02 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:12:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:12:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Sep 2022 19:13:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d30cf2a6a25aea48a115837d149468c8de7df7fb51f210b9fa1173c065f7b34c`  
		Last Modified: Tue, 06 Sep 2022 18:50:34 GMT  
		Size: 23.7 MB (23734076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79317661c5fe6a8a22ce652c9fb0999eb96ed08b735a16224e9a795c877780d`  
		Last Modified: Tue, 06 Sep 2022 19:16:57 GMT  
		Size: 6.1 MB (6072017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:737382e506f963b99b1453e20a2fcbb6bc4328a0c68bfc3530b2082a5f3da14f`  
		Last Modified: Tue, 06 Sep 2022 19:16:56 GMT  
		Size: 2.6 MB (2571091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160f71044c4c89d05d500625b4eda19add7227d613b991017a9850f2945440d2`  
		Last Modified: Tue, 06 Sep 2022 19:17:14 GMT  
		Size: 43.3 MB (43296151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:0ebf787eef91cb40d6785f4fee2e318e1caa0efea1ef139dd16efb9cb2170108
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.2 MB (84207988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bade70b0313e63645171fc0d2e32aac037cc1c538a5011e096bf92b7bf9bec62`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 18:40:06 GMT
ADD file:31701667cc90b9f4ce7d6ede94bf7dae4d63c49e62d3725094d547f9601e1165 in / 
# Tue, 06 Sep 2022 18:40:07 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:02:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:02:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Sep 2022 19:02:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10d3032d1995d3163c20a7f2f197299fae258c2ad020a8fd586fd6b7dd1b0e1d`  
		Last Modified: Tue, 06 Sep 2022 18:40:53 GMT  
		Size: 27.2 MB (27164710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360b65e679bf1db70d92b45a6d39c882e074d441412548705adf35d49a12c70a`  
		Last Modified: Tue, 06 Sep 2022 19:06:33 GMT  
		Size: 6.9 MB (6919740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8820513ab0577fe6133989b66cdc2a5a0b1a97af5280746721af55657c0897d7`  
		Last Modified: Tue, 06 Sep 2022 19:06:32 GMT  
		Size: 3.0 MB (3039943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ad90e9fc8930485dc12eedaf8101fe62b983d943986b7325ff502b9d424d75`  
		Last Modified: Tue, 06 Sep 2022 19:06:52 GMT  
		Size: 47.1 MB (47083595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3cb7543c344e0352386e8a80cfe8d4ad2ad58f5d0b15c562893d95425acd39a0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.0 MB (94956408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60cb88494227b72c2ba6f2f4ea540126cfe6da20dd2844ac77122510289f8cf0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 19:38:57 GMT
ADD file:1b76d0a41921afefb92711c44ceb312c16828d433b689a951d65c238faa9ac50 in / 
# Tue, 06 Sep 2022 19:38:59 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 20:06:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 20:06:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Sep 2022 20:07:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4abf8f40556a940861bc7fc313acefb89c775273ed06b7d41cfb222ccf8a1438`  
		Last Modified: Tue, 06 Sep 2022 19:40:56 GMT  
		Size: 30.4 MB (30441623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7afd3028934ff054bca1d0bb218e690d2cdb60f7754ad3bb6426c3744e730f`  
		Last Modified: Tue, 06 Sep 2022 20:12:44 GMT  
		Size: 7.1 MB (7050146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33850c25587eb4418b5e6aeccf1c9e6fa5b0baac624020bc56b4d4db8c2742c5`  
		Last Modified: Tue, 06 Sep 2022 20:12:43 GMT  
		Size: 3.7 MB (3720231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677c4d750793a0cab4cd23689261d167383d4e03f7fce03417017fcfd5497d21`  
		Last Modified: Tue, 06 Sep 2022 20:13:12 GMT  
		Size: 53.7 MB (53744408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a75bb4a086eb933364de634f5df3c444ccf522851ca2519cbb956366f444fce9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79715431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:718e03d049e2e94d8ddad47f516b220c5cdbf5ffde7f2e3a4f0a9a6808c63589`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 18:43:36 GMT
ADD file:dbe2a8e3943129e654ee29c636cab2bb10dd7eb0ac27d51e6954af2ccbe22807 in / 
# Tue, 06 Sep 2022 18:43:37 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:11:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:11:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Sep 2022 19:12:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be6761156800c616810cb8aeb5b3ae71b9a2082f1c1221210befe119f082e879`  
		Last Modified: Tue, 06 Sep 2022 18:45:00 GMT  
		Size: 25.4 MB (25370130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae409e724954611ea7731639a0dab7c4c59fdb64deb51dba5327bc8c5a085c5f`  
		Last Modified: Tue, 06 Sep 2022 19:17:11 GMT  
		Size: 6.3 MB (6324234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aca3edc7c631417c9e3dbbcb30698aed6531dc2482e10dd41ee221de2d450ca5`  
		Last Modified: Tue, 06 Sep 2022 19:17:11 GMT  
		Size: 3.0 MB (2977166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee7b8f6dba5690621ef3c6a174a056a9b68be9f2c37eeb155bc990d0284bcf0`  
		Last Modified: Tue, 06 Sep 2022 19:17:26 GMT  
		Size: 45.0 MB (45043901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bookworm`

```console
$ docker pull buildpack-deps@sha256:3f1c2db6b34ee6bc4359ac8cdbaba18a30caae19e001d8b7bb88a652919765ca
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

### `buildpack-deps:bookworm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:c499dd57309b82d2d43be6cd76563d9713b78e09edac66558e8adb44d73140f2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **562.1 MB (562080993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ce38a856ecb08376f79b2d4fd6cca8d215ab17103b6274edcd9aa076032ade5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:15 GMT
ADD file:7507edfdf016128615e9ba278d471fd6d27c96436e543786b691c93b6f94b56b in / 
# Tue, 23 Aug 2022 00:20:16 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:46:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:46:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 00:46:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:47:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5e784af754e1c7855decd29b818520a98b5b539515cd7c199c5dbceb6cc4a45f`  
		Last Modified: Tue, 23 Aug 2022 00:23:57 GMT  
		Size: 52.7 MB (52725730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06352499c53ea1415d7d7121128de838e832cbc465b145c71d05fb7b74a91c0`  
		Last Modified: Tue, 23 Aug 2022 00:54:04 GMT  
		Size: 9.3 MB (9298815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e88fbc1ce3af2aec72e131f3b876f2554849f8d6291840fbaf61b24970e54c3`  
		Last Modified: Tue, 23 Aug 2022 00:54:04 GMT  
		Size: 11.3 MB (11272439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2afebddf0d45a19b246f4ff1ead1dd600b48cc494afd00873819774f29c6f388`  
		Last Modified: Tue, 23 Aug 2022 00:54:22 GMT  
		Size: 57.6 MB (57602962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7909283d0b83eb6d0800ae7c471c60ae0891ef4c36524f7ff60b725616e553ed`  
		Last Modified: Tue, 23 Aug 2022 00:55:27 GMT  
		Size: 431.2 MB (431181047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:97f078f2318ddd0d5e369b26b804cae7895b80a64cfdb38598ed08f09b59de96
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **512.6 MB (512603026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9338cdc62f6d8b5386b6ceae633ea50d5f36bd4d30c72201040efca568d03302`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:16:08 GMT
ADD file:dbc0c48f409cbe73d340bec8639492807b8c28fa6907379a17a958448dca1829 in / 
# Tue, 23 Aug 2022 01:16:08 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 06:16:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 06:16:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 06:16:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 06:18:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3204f8dd2e8fdf47391628664d2c96551393e3e0abd1e471abeb57296519c816`  
		Last Modified: Tue, 23 Aug 2022 01:21:24 GMT  
		Size: 51.8 MB (51814042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2edbed2d89089bed15e37327dce17d68521ccd0390a9172314785a01bb2918c5`  
		Last Modified: Tue, 23 Aug 2022 06:24:42 GMT  
		Size: 8.7 MB (8740375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ead884b6cf02ae26001f7fa32ee0d5127f5b1f36fe6d675bf0ab7b8b81baa00`  
		Last Modified: Tue, 23 Aug 2022 06:24:42 GMT  
		Size: 10.9 MB (10946896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e395af4802fa3dfe5d8dc10a19e4fb9ea0adaa8951ba0595e9c756a12d412bb8`  
		Last Modified: Tue, 23 Aug 2022 06:25:07 GMT  
		Size: 55.3 MB (55284425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509d388565301a498f7b95d89df044727bf2633fd54aacd973fc712a97327789`  
		Last Modified: Tue, 23 Aug 2022 06:26:41 GMT  
		Size: 385.8 MB (385817288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ebbb69050ba98917a5a15e299ba7aa9339f319cd4cdd3156bfebb53cbebf582d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **500.2 MB (500233814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bad6c9a12283cdf877c74e1d905354fcb63b8be182f414c2de79272cd53bf52`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:42:14 GMT
ADD file:590ff1916ed8a15a7a205153d20c2823a242c228573a1868134df4bdd95f10d8 in / 
# Tue, 23 Aug 2022 01:42:14 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 12:57:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 12:57:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 12:58:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 12:59:43 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b4a2cf95b2637a1520aeb527ca7569456a3bcf1d740f72cc418357cbe490704d`  
		Last Modified: Tue, 23 Aug 2022 01:48:45 GMT  
		Size: 49.6 MB (49555090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0a9319f004c20513b7f62d6d76d1b1959183b5ad5b488373ca6330a9d6797b`  
		Last Modified: Tue, 23 Aug 2022 13:09:50 GMT  
		Size: 8.4 MB (8402996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fd63a2d6ab83a6d913419cd2a446fc94d0d9a4c654bf2a3c13dfe3a7116609`  
		Last Modified: Tue, 23 Aug 2022 13:09:49 GMT  
		Size: 10.6 MB (10589855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c7d7ae465211d33c40484e48402566e419669463cab573010f1ab877df64a9`  
		Last Modified: Tue, 23 Aug 2022 13:10:16 GMT  
		Size: 53.3 MB (53323503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ac7c9931aada6b836dce88ec19cd79064ffe2024e95270c239c73860ab7d72`  
		Last Modified: Tue, 23 Aug 2022 13:11:44 GMT  
		Size: 378.4 MB (378362370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:b8074d04677387c84532dbc39903d4a7ba2dbac38fa624956417e4b251024d25
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **551.9 MB (551918652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1473f33d94d3c58cb12b6d618f9cafa967b830841c427a4fa8717f924dd351b2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:51:53 GMT
ADD file:f94a576f262c4fcf5112164145c04850c826787b299878e7e126754d1211a51c in / 
# Tue, 23 Aug 2022 01:51:53 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:25:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:25:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 02:26:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:27:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7dd208a8a7339c037c691e6ace1cd3f94803ee4c17a3211b9ccadf01d1ff2ca9`  
		Last Modified: Tue, 23 Aug 2022 01:56:50 GMT  
		Size: 53.1 MB (53117563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a6d7761ab15abc5f27917ed7e543565cb302e30ac8bd10819c205f079ec603`  
		Last Modified: Tue, 23 Aug 2022 02:35:05 GMT  
		Size: 9.1 MB (9133938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d472709c6f5c8abe91373fba2db77fd3b0946f573269803173452485abc6ff8b`  
		Last Modified: Tue, 23 Aug 2022 02:35:05 GMT  
		Size: 11.1 MB (11062413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247b0fb5989ae9d485d4b97b959d16adfaeb2e92bf9a74bd8b1f677bb7f3e1c5`  
		Last Modified: Tue, 23 Aug 2022 02:35:25 GMT  
		Size: 57.5 MB (57496084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e62402acaffd55bc794eef07b132e4223f8f48067c5d1df8909da8f8de8e39`  
		Last Modified: Tue, 23 Aug 2022 02:36:32 GMT  
		Size: 421.1 MB (421108654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8539ef8ee56afeb586b85e49787586a5111a6de92bc10b9f37ca69bd9309ad13
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.1 MB (355072478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b32f2b395672361202ddd299bd9ee7fb01a3d461778187967fb1f32cdf4a2d82`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:01:59 GMT
ADD file:1c8ebe8b69a2d3c236c8a947162fab2e579f4bf01bff01695a3c46557f6c73f4 in / 
# Tue, 23 Aug 2022 01:02:00 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:28:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:28:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:29:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:31:24 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:29bf8f676853094720e43096224f2ec8a31ffa3752cf7a1e52fb9e72ae069480`  
		Last Modified: Tue, 23 Aug 2022 01:07:13 GMT  
		Size: 54.1 MB (54096938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0426ba96c16ee4ea8eb5b5322685d94b842c455938234d92ca07814c6ae081`  
		Last Modified: Tue, 23 Aug 2022 01:38:51 GMT  
		Size: 9.5 MB (9475146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86201f3e5308e2da4dad080700c08b4d6a0a02c265e56c7a0cdae2889f16b442`  
		Last Modified: Tue, 23 Aug 2022 01:38:51 GMT  
		Size: 11.5 MB (11473600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4eae1a3c8a2b637c155af3a0e81b010eea8632db588e887a59f57d020ad81a8`  
		Last Modified: Tue, 23 Aug 2022 01:39:11 GMT  
		Size: 59.1 MB (59102590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ecd69ec89ab5cbb90df7026e375153b4bae6f2e062807e484c266484a434f19`  
		Last Modified: Tue, 23 Aug 2022 01:39:48 GMT  
		Size: 220.9 MB (220924204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:a33f9fc319310e0dc05df0ac31354c80d3a3752809f776e4531c09131e54f6df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **588.8 MB (588838001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16b0b2ddf00ac1d07da3682f6cfc85609adb6af1836c17a484332e1d9817ccfe`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:09:18 GMT
ADD file:2b4a878ee82590d9ee2da01a2501742d21f6d050a0002f9bd484a4d7c8620d2e in / 
# Tue, 23 Aug 2022 00:09:23 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 22:12:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 22:13:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 22:15:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 22:23:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4b18e364c6342ca1244071a2f94edf42b92a5b7997d16df3b26467139f3f0603`  
		Last Modified: Tue, 23 Aug 2022 00:17:33 GMT  
		Size: 53.1 MB (53119349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5edf0a5e5947b8da11a8b58c48bd00dc43fe37b1375dd57214cc77b72c0bc009`  
		Last Modified: Tue, 23 Aug 2022 22:43:15 GMT  
		Size: 8.7 MB (8660383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd311acb344ec357f0aa8b600c00bac50d5489700c6ec00ff2ec71f10bf3789`  
		Last Modified: Tue, 23 Aug 2022 22:43:14 GMT  
		Size: 11.0 MB (11042106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6304e93b6d685763966db039d84593203f3027de2420ebe4cf0e2865b59ee64d`  
		Last Modified: Tue, 23 Aug 2022 22:44:05 GMT  
		Size: 56.5 MB (56454547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d95aec47b529f681de91b7db74b4fdb10f85a8019db378445bf8e551565e0369`  
		Last Modified: Tue, 23 Aug 2022 22:48:49 GMT  
		Size: 459.6 MB (459561616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:ee2a6c73ac3292db2fa2fbf661eb2e89b0efb41e7d31d177c394eef94afc20fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **561.4 MB (561424552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f377208d9b0ee3a46f734c8e72364e0683ef2f7b1516eaa2a8fc4b2eb0878050`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:23:48 GMT
ADD file:92444ce23c3227ef88446469c37fc41decda1ba975ddfb1be3e1ebb1e694471b in / 
# Tue, 23 Aug 2022 01:23:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:52:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:52:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:53:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:57:32 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a2d2f2c5b4e64eabb8a7632609e67883239433d932129bf478f7614059a9aabe`  
		Last Modified: Tue, 23 Aug 2022 01:29:05 GMT  
		Size: 57.3 MB (57289866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b43c7a1c5614eda4b722aada1632b2b42c7499b945bcd902a405d6811943e66`  
		Last Modified: Tue, 23 Aug 2022 02:08:15 GMT  
		Size: 9.9 MB (9888870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4983e94a7031bdb88baa08be05b8f42254ef49f65245663476650772c95d77`  
		Last Modified: Tue, 23 Aug 2022 02:08:15 GMT  
		Size: 12.1 MB (12083610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea4205d8530bba3b66567e144b76048ea3deb5e2f1d3604690cc87c10af416f`  
		Last Modified: Tue, 23 Aug 2022 02:08:43 GMT  
		Size: 62.4 MB (62419202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e108af90182e1e05955b926792132c93a713e0f0ae2b578251685acee0a56d`  
		Last Modified: Tue, 23 Aug 2022 02:10:29 GMT  
		Size: 419.7 MB (419743004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:8c0ab6fb48d76634a12d5294e8bca9d24a5b9906ced33a933a040932fd7b8c51
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **506.2 MB (506202129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a30d9f47701b1b9e8e1facf3f4c9c146ebb42ad42f38bb07e3be148d38711791`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:53:14 GMT
ADD file:e8167229629003ac0dcc7f0bcc35a939121e9b4a88b67483883c2741f5415634 in / 
# Tue, 23 Aug 2022 00:53:16 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 09:49:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 09:49:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 09:49:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 09:51:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bfa0b60dda37e3a2f71f5d19d0259a51a84ce3f8e9deff107720c9868e69769b`  
		Last Modified: Tue, 23 Aug 2022 00:57:59 GMT  
		Size: 51.6 MB (51559576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9f7dae28c5d2750f7a41520dc8fec8c6914c21a7ced6fbda8b32c01477bc57`  
		Last Modified: Tue, 23 Aug 2022 09:58:50 GMT  
		Size: 8.9 MB (8941068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a871302fe26c06a3669e3a3f80c6e947aba9fbecf2fddb59dfe0739cf8a3f48a`  
		Last Modified: Tue, 23 Aug 2022 09:58:50 GMT  
		Size: 11.2 MB (11166576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f7f08e932daba42246e92ace2e6a7084e92eb623212ae6d100ba95f988439df`  
		Last Modified: Tue, 23 Aug 2022 09:59:04 GMT  
		Size: 56.9 MB (56866268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7411d09609a3404724d2396baedced7c080958509598eeaf565769349ead75`  
		Last Modified: Tue, 23 Aug 2022 09:59:51 GMT  
		Size: 377.7 MB (377668641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bookworm-curl`

```console
$ docker pull buildpack-deps@sha256:920db90394b6ae75318c2d0abffd0e57dec63104639684dc07b01dd38a87adf5
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

### `buildpack-deps:bookworm-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:a2c9bcba0f65768c2f380cdb068c2ea33e88f7186a94142f0a02884cbbecae2d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.3 MB (73296984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96518376d229d3c3d2c3f2977817cd43b1253209b546da45f802bdd6fede1ef5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:15 GMT
ADD file:7507edfdf016128615e9ba278d471fd6d27c96436e543786b691c93b6f94b56b in / 
# Tue, 23 Aug 2022 00:20:16 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:46:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:46:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5e784af754e1c7855decd29b818520a98b5b539515cd7c199c5dbceb6cc4a45f`  
		Last Modified: Tue, 23 Aug 2022 00:23:57 GMT  
		Size: 52.7 MB (52725730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06352499c53ea1415d7d7121128de838e832cbc465b145c71d05fb7b74a91c0`  
		Last Modified: Tue, 23 Aug 2022 00:54:04 GMT  
		Size: 9.3 MB (9298815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e88fbc1ce3af2aec72e131f3b876f2554849f8d6291840fbaf61b24970e54c3`  
		Last Modified: Tue, 23 Aug 2022 00:54:04 GMT  
		Size: 11.3 MB (11272439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:46faed2ba6d4fb76b3258765430464b1a7003b23ed86435d2752c89d397c5b0b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.5 MB (71501313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc2b9a42ac97d4c443a8cd1be847430cb3bd4ea1d867a7f662c15cb1144dc327`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:16:08 GMT
ADD file:dbc0c48f409cbe73d340bec8639492807b8c28fa6907379a17a958448dca1829 in / 
# Tue, 23 Aug 2022 01:16:08 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 06:16:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 06:16:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3204f8dd2e8fdf47391628664d2c96551393e3e0abd1e471abeb57296519c816`  
		Last Modified: Tue, 23 Aug 2022 01:21:24 GMT  
		Size: 51.8 MB (51814042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2edbed2d89089bed15e37327dce17d68521ccd0390a9172314785a01bb2918c5`  
		Last Modified: Tue, 23 Aug 2022 06:24:42 GMT  
		Size: 8.7 MB (8740375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ead884b6cf02ae26001f7fa32ee0d5127f5b1f36fe6d675bf0ab7b8b81baa00`  
		Last Modified: Tue, 23 Aug 2022 06:24:42 GMT  
		Size: 10.9 MB (10946896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:eca2e025d883dc6e53b0bcba83bba2ebbd9180d026142ba402bee57e7e36cb1a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68547941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fdb79dc67924d7dc4d70c832938055d861fd8a72ba69c93b61f05333fb06605`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:42:14 GMT
ADD file:590ff1916ed8a15a7a205153d20c2823a242c228573a1868134df4bdd95f10d8 in / 
# Tue, 23 Aug 2022 01:42:14 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 12:57:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 12:57:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b4a2cf95b2637a1520aeb527ca7569456a3bcf1d740f72cc418357cbe490704d`  
		Last Modified: Tue, 23 Aug 2022 01:48:45 GMT  
		Size: 49.6 MB (49555090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0a9319f004c20513b7f62d6d76d1b1959183b5ad5b488373ca6330a9d6797b`  
		Last Modified: Tue, 23 Aug 2022 13:09:50 GMT  
		Size: 8.4 MB (8402996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fd63a2d6ab83a6d913419cd2a446fc94d0d9a4c654bf2a3c13dfe3a7116609`  
		Last Modified: Tue, 23 Aug 2022 13:09:49 GMT  
		Size: 10.6 MB (10589855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:af43066ded189a6b7e29c63c61133429e2c2b2d43a2e58d2daa76efe5b917bc3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.3 MB (73313914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1d0bb4e26e6776a1c17038201bde02c005f88d7bfa7354e7d0e3218ddf36414`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:51:53 GMT
ADD file:f94a576f262c4fcf5112164145c04850c826787b299878e7e126754d1211a51c in / 
# Tue, 23 Aug 2022 01:51:53 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:25:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:25:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:7dd208a8a7339c037c691e6ace1cd3f94803ee4c17a3211b9ccadf01d1ff2ca9`  
		Last Modified: Tue, 23 Aug 2022 01:56:50 GMT  
		Size: 53.1 MB (53117563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a6d7761ab15abc5f27917ed7e543565cb302e30ac8bd10819c205f079ec603`  
		Last Modified: Tue, 23 Aug 2022 02:35:05 GMT  
		Size: 9.1 MB (9133938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d472709c6f5c8abe91373fba2db77fd3b0946f573269803173452485abc6ff8b`  
		Last Modified: Tue, 23 Aug 2022 02:35:05 GMT  
		Size: 11.1 MB (11062413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:be37277a8a268026b2fabbf0c0d4d77c022a17d6dd095e2cedc7d8f4a4b3cf65
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.0 MB (75045684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6b54df36b64a7450c4db38d1ca99f0ef6f8533945a326f1f4f7ac4e6e9ef983`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:01:59 GMT
ADD file:1c8ebe8b69a2d3c236c8a947162fab2e579f4bf01bff01695a3c46557f6c73f4 in / 
# Tue, 23 Aug 2022 01:02:00 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:28:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:28:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:29bf8f676853094720e43096224f2ec8a31ffa3752cf7a1e52fb9e72ae069480`  
		Last Modified: Tue, 23 Aug 2022 01:07:13 GMT  
		Size: 54.1 MB (54096938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0426ba96c16ee4ea8eb5b5322685d94b842c455938234d92ca07814c6ae081`  
		Last Modified: Tue, 23 Aug 2022 01:38:51 GMT  
		Size: 9.5 MB (9475146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86201f3e5308e2da4dad080700c08b4d6a0a02c265e56c7a0cdae2889f16b442`  
		Last Modified: Tue, 23 Aug 2022 01:38:51 GMT  
		Size: 11.5 MB (11473600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:aab0c69c14ce9ef03205d8e14af84b378de16c95451a791e6e33bb12746a53e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.8 MB (72821838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb89bf0a7e7dccfef6cd4f619698b29111d786ef44c4c96ae76088989fef2bb0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:09:18 GMT
ADD file:2b4a878ee82590d9ee2da01a2501742d21f6d050a0002f9bd484a4d7c8620d2e in / 
# Tue, 23 Aug 2022 00:09:23 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 22:12:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 22:13:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4b18e364c6342ca1244071a2f94edf42b92a5b7997d16df3b26467139f3f0603`  
		Last Modified: Tue, 23 Aug 2022 00:17:33 GMT  
		Size: 53.1 MB (53119349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5edf0a5e5947b8da11a8b58c48bd00dc43fe37b1375dd57214cc77b72c0bc009`  
		Last Modified: Tue, 23 Aug 2022 22:43:15 GMT  
		Size: 8.7 MB (8660383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd311acb344ec357f0aa8b600c00bac50d5489700c6ec00ff2ec71f10bf3789`  
		Last Modified: Tue, 23 Aug 2022 22:43:14 GMT  
		Size: 11.0 MB (11042106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:085f8dcab702213ca234e533f0d7c394b315c6558341fd0d71206dd815305279
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.3 MB (79262346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf0eeff677f73e0eec150a7ebe08f2cbd0fae801a6f253e6709522d4569a6163`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:23:48 GMT
ADD file:92444ce23c3227ef88446469c37fc41decda1ba975ddfb1be3e1ebb1e694471b in / 
# Tue, 23 Aug 2022 01:23:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:52:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:52:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a2d2f2c5b4e64eabb8a7632609e67883239433d932129bf478f7614059a9aabe`  
		Last Modified: Tue, 23 Aug 2022 01:29:05 GMT  
		Size: 57.3 MB (57289866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b43c7a1c5614eda4b722aada1632b2b42c7499b945bcd902a405d6811943e66`  
		Last Modified: Tue, 23 Aug 2022 02:08:15 GMT  
		Size: 9.9 MB (9888870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4983e94a7031bdb88baa08be05b8f42254ef49f65245663476650772c95d77`  
		Last Modified: Tue, 23 Aug 2022 02:08:15 GMT  
		Size: 12.1 MB (12083610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:fb68ac36160a91bfb4682cfdaef3cf44fb33fbf32c01d787a5adee5c5d70ae7c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.7 MB (71667220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca9c5e8d57f49cedaab70bf6f460b53ecd1b779bc00692d82088c8274aac7f3c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:53:14 GMT
ADD file:e8167229629003ac0dcc7f0bcc35a939121e9b4a88b67483883c2741f5415634 in / 
# Tue, 23 Aug 2022 00:53:16 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 09:49:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 09:49:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:bfa0b60dda37e3a2f71f5d19d0259a51a84ce3f8e9deff107720c9868e69769b`  
		Last Modified: Tue, 23 Aug 2022 00:57:59 GMT  
		Size: 51.6 MB (51559576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9f7dae28c5d2750f7a41520dc8fec8c6914c21a7ced6fbda8b32c01477bc57`  
		Last Modified: Tue, 23 Aug 2022 09:58:50 GMT  
		Size: 8.9 MB (8941068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a871302fe26c06a3669e3a3f80c6e947aba9fbecf2fddb59dfe0739cf8a3f48a`  
		Last Modified: Tue, 23 Aug 2022 09:58:50 GMT  
		Size: 11.2 MB (11166576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bookworm-scm`

```console
$ docker pull buildpack-deps@sha256:9043c34b103e0c0c1c4e5bb7a18c064a3f5dc3c4823ab73e33c9e688f3e10dd6
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

### `buildpack-deps:bookworm-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:f679dfea28b543518362ad66cac6b1240302cdfc6f6253e1529bd0c0063f9ccb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.9 MB (130899946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5065f8a27ab438502224d3d8c878db108e01f3cc1d35cb19090300d6ba573049`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:15 GMT
ADD file:7507edfdf016128615e9ba278d471fd6d27c96436e543786b691c93b6f94b56b in / 
# Tue, 23 Aug 2022 00:20:16 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:46:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:46:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 00:46:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5e784af754e1c7855decd29b818520a98b5b539515cd7c199c5dbceb6cc4a45f`  
		Last Modified: Tue, 23 Aug 2022 00:23:57 GMT  
		Size: 52.7 MB (52725730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06352499c53ea1415d7d7121128de838e832cbc465b145c71d05fb7b74a91c0`  
		Last Modified: Tue, 23 Aug 2022 00:54:04 GMT  
		Size: 9.3 MB (9298815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e88fbc1ce3af2aec72e131f3b876f2554849f8d6291840fbaf61b24970e54c3`  
		Last Modified: Tue, 23 Aug 2022 00:54:04 GMT  
		Size: 11.3 MB (11272439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2afebddf0d45a19b246f4ff1ead1dd600b48cc494afd00873819774f29c6f388`  
		Last Modified: Tue, 23 Aug 2022 00:54:22 GMT  
		Size: 57.6 MB (57602962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:dc1c4e9ae95084f819ce284e2799135e73f0749ff86245301b5df7ab70a27a27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.8 MB (126785738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6df0ab6a1f8c5c5224f0b76a13da3b636bf824c3286b34e306e7a71fc9ba6ba0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:16:08 GMT
ADD file:dbc0c48f409cbe73d340bec8639492807b8c28fa6907379a17a958448dca1829 in / 
# Tue, 23 Aug 2022 01:16:08 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 06:16:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 06:16:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 06:16:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3204f8dd2e8fdf47391628664d2c96551393e3e0abd1e471abeb57296519c816`  
		Last Modified: Tue, 23 Aug 2022 01:21:24 GMT  
		Size: 51.8 MB (51814042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2edbed2d89089bed15e37327dce17d68521ccd0390a9172314785a01bb2918c5`  
		Last Modified: Tue, 23 Aug 2022 06:24:42 GMT  
		Size: 8.7 MB (8740375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ead884b6cf02ae26001f7fa32ee0d5127f5b1f36fe6d675bf0ab7b8b81baa00`  
		Last Modified: Tue, 23 Aug 2022 06:24:42 GMT  
		Size: 10.9 MB (10946896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e395af4802fa3dfe5d8dc10a19e4fb9ea0adaa8951ba0595e9c756a12d412bb8`  
		Last Modified: Tue, 23 Aug 2022 06:25:07 GMT  
		Size: 55.3 MB (55284425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:c50fdc3cc8971109d7e2fb62ae7f6e0654628f84a110f1113a842ee045e776ac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.9 MB (121871444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3aaa5ae4912b2de292b9affa365fa17be839dbd9222323714858cc9d901bb30`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:42:14 GMT
ADD file:590ff1916ed8a15a7a205153d20c2823a242c228573a1868134df4bdd95f10d8 in / 
# Tue, 23 Aug 2022 01:42:14 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 12:57:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 12:57:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 12:58:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b4a2cf95b2637a1520aeb527ca7569456a3bcf1d740f72cc418357cbe490704d`  
		Last Modified: Tue, 23 Aug 2022 01:48:45 GMT  
		Size: 49.6 MB (49555090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0a9319f004c20513b7f62d6d76d1b1959183b5ad5b488373ca6330a9d6797b`  
		Last Modified: Tue, 23 Aug 2022 13:09:50 GMT  
		Size: 8.4 MB (8402996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fd63a2d6ab83a6d913419cd2a446fc94d0d9a4c654bf2a3c13dfe3a7116609`  
		Last Modified: Tue, 23 Aug 2022 13:09:49 GMT  
		Size: 10.6 MB (10589855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c7d7ae465211d33c40484e48402566e419669463cab573010f1ab877df64a9`  
		Last Modified: Tue, 23 Aug 2022 13:10:16 GMT  
		Size: 53.3 MB (53323503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:0155117db9306b41c236e921e5f76a0bd743851a0ef03fdd0375580ad644862f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.8 MB (130809998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5866f5d0d44278637ed443b0e5d5a0e8b808d2c70c50503fc468ffa7d2bf8b13`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:51:53 GMT
ADD file:f94a576f262c4fcf5112164145c04850c826787b299878e7e126754d1211a51c in / 
# Tue, 23 Aug 2022 01:51:53 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:25:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:25:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 02:26:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7dd208a8a7339c037c691e6ace1cd3f94803ee4c17a3211b9ccadf01d1ff2ca9`  
		Last Modified: Tue, 23 Aug 2022 01:56:50 GMT  
		Size: 53.1 MB (53117563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a6d7761ab15abc5f27917ed7e543565cb302e30ac8bd10819c205f079ec603`  
		Last Modified: Tue, 23 Aug 2022 02:35:05 GMT  
		Size: 9.1 MB (9133938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d472709c6f5c8abe91373fba2db77fd3b0946f573269803173452485abc6ff8b`  
		Last Modified: Tue, 23 Aug 2022 02:35:05 GMT  
		Size: 11.1 MB (11062413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247b0fb5989ae9d485d4b97b959d16adfaeb2e92bf9a74bd8b1f677bb7f3e1c5`  
		Last Modified: Tue, 23 Aug 2022 02:35:25 GMT  
		Size: 57.5 MB (57496084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:1a6e04486d701fe9f175abed959a5794adb184ded2d14ea520fda84aa445ba9c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.1 MB (134148274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8346a4ca2444870e8bb65aff75d4d4cf6711229035f48bacd81de5aee6ec3ee`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:01:59 GMT
ADD file:1c8ebe8b69a2d3c236c8a947162fab2e579f4bf01bff01695a3c46557f6c73f4 in / 
# Tue, 23 Aug 2022 01:02:00 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:28:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:28:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:29:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:29bf8f676853094720e43096224f2ec8a31ffa3752cf7a1e52fb9e72ae069480`  
		Last Modified: Tue, 23 Aug 2022 01:07:13 GMT  
		Size: 54.1 MB (54096938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0426ba96c16ee4ea8eb5b5322685d94b842c455938234d92ca07814c6ae081`  
		Last Modified: Tue, 23 Aug 2022 01:38:51 GMT  
		Size: 9.5 MB (9475146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86201f3e5308e2da4dad080700c08b4d6a0a02c265e56c7a0cdae2889f16b442`  
		Last Modified: Tue, 23 Aug 2022 01:38:51 GMT  
		Size: 11.5 MB (11473600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4eae1a3c8a2b637c155af3a0e81b010eea8632db588e887a59f57d020ad81a8`  
		Last Modified: Tue, 23 Aug 2022 01:39:11 GMT  
		Size: 59.1 MB (59102590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:eeced580e9256e37c10c45f4f3ba1068a3eea3bb6380d105192d70491e16f28f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.3 MB (129276385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:955ae09e149c1e982f8e43e476d7d60341fcfcfc48248c24ef4c5b84e97d70be`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:09:18 GMT
ADD file:2b4a878ee82590d9ee2da01a2501742d21f6d050a0002f9bd484a4d7c8620d2e in / 
# Tue, 23 Aug 2022 00:09:23 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 22:12:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 22:13:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 22:15:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4b18e364c6342ca1244071a2f94edf42b92a5b7997d16df3b26467139f3f0603`  
		Last Modified: Tue, 23 Aug 2022 00:17:33 GMT  
		Size: 53.1 MB (53119349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5edf0a5e5947b8da11a8b58c48bd00dc43fe37b1375dd57214cc77b72c0bc009`  
		Last Modified: Tue, 23 Aug 2022 22:43:15 GMT  
		Size: 8.7 MB (8660383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd311acb344ec357f0aa8b600c00bac50d5489700c6ec00ff2ec71f10bf3789`  
		Last Modified: Tue, 23 Aug 2022 22:43:14 GMT  
		Size: 11.0 MB (11042106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6304e93b6d685763966db039d84593203f3027de2420ebe4cf0e2865b59ee64d`  
		Last Modified: Tue, 23 Aug 2022 22:44:05 GMT  
		Size: 56.5 MB (56454547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:1ae72a86df0538f6c86e6177acda8b42ac2b5bc5b16f91d75bd6dff1d570c92c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.7 MB (141681548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f9e0dbaf8822ad89bf60827cb4b2f3927b1784af8cc2d1ff24f2e790d144376`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:23:48 GMT
ADD file:92444ce23c3227ef88446469c37fc41decda1ba975ddfb1be3e1ebb1e694471b in / 
# Tue, 23 Aug 2022 01:23:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:52:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:52:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:53:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a2d2f2c5b4e64eabb8a7632609e67883239433d932129bf478f7614059a9aabe`  
		Last Modified: Tue, 23 Aug 2022 01:29:05 GMT  
		Size: 57.3 MB (57289866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b43c7a1c5614eda4b722aada1632b2b42c7499b945bcd902a405d6811943e66`  
		Last Modified: Tue, 23 Aug 2022 02:08:15 GMT  
		Size: 9.9 MB (9888870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4983e94a7031bdb88baa08be05b8f42254ef49f65245663476650772c95d77`  
		Last Modified: Tue, 23 Aug 2022 02:08:15 GMT  
		Size: 12.1 MB (12083610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea4205d8530bba3b66567e144b76048ea3deb5e2f1d3604690cc87c10af416f`  
		Last Modified: Tue, 23 Aug 2022 02:08:43 GMT  
		Size: 62.4 MB (62419202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a35ea6986151b6a9cfa303d6c7b88d34eb1efbdda23f410a313539d54216369d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.5 MB (128533488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49e0602dc9c0c8d0c36a03cf960026a77c297d6572bb13d8c27894d283bde270`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:53:14 GMT
ADD file:e8167229629003ac0dcc7f0bcc35a939121e9b4a88b67483883c2741f5415634 in / 
# Tue, 23 Aug 2022 00:53:16 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 09:49:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 09:49:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 09:49:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bfa0b60dda37e3a2f71f5d19d0259a51a84ce3f8e9deff107720c9868e69769b`  
		Last Modified: Tue, 23 Aug 2022 00:57:59 GMT  
		Size: 51.6 MB (51559576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9f7dae28c5d2750f7a41520dc8fec8c6914c21a7ced6fbda8b32c01477bc57`  
		Last Modified: Tue, 23 Aug 2022 09:58:50 GMT  
		Size: 8.9 MB (8941068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a871302fe26c06a3669e3a3f80c6e947aba9fbecf2fddb59dfe0739cf8a3f48a`  
		Last Modified: Tue, 23 Aug 2022 09:58:50 GMT  
		Size: 11.2 MB (11166576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f7f08e932daba42246e92ace2e6a7084e92eb623212ae6d100ba95f988439df`  
		Last Modified: Tue, 23 Aug 2022 09:59:04 GMT  
		Size: 56.9 MB (56866268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bullseye`

```console
$ docker pull buildpack-deps@sha256:872ba70b0805b817db42d9ea75f066b5fe2be82d04d0dab69e41810edd9aa3f9
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
$ docker pull buildpack-deps@sha256:fdd46ac593b0dc4c54497b36e00e54c7759d068d9b9f014bd5b47bed430d4c2f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.4 MB (322416189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1966d2c176635cea14ac52f6a8a1d7d57101cb829eae63a9f3597cdee7a0ef6f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:40 GMT
ADD file:6944d322f4c04bd2192061822af5cbec8ac0a6b424c461d66174d32aed604972 in / 
# Tue, 23 Aug 2022 00:20:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:48:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:48:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 00:48:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:49:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1671565cc8df8c365c9b661d3fbc164e73d01f1b0430c6179588428f99a9da2e`  
		Last Modified: Tue, 23 Aug 2022 00:24:32 GMT  
		Size: 55.0 MB (55007555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e94d13e55e7a4ef17ff21376f57fb95c7e1706931f8704aa99260968d81f6e4`  
		Last Modified: Tue, 23 Aug 2022 00:55:37 GMT  
		Size: 5.2 MB (5163019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9c7528c685216129e8e67bf362a7702e7b1daa585ab85546a41508830657d6`  
		Last Modified: Tue, 23 Aug 2022 00:55:38 GMT  
		Size: 10.9 MB (10876472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ad072f9cd16fc8eb93b182b20e758e11acc0ef60babef0bf1043c08de1901a`  
		Last Modified: Tue, 23 Aug 2022 00:55:57 GMT  
		Size: 54.6 MB (54584135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b983117533b718374f1701ef593dd2afa6613c7908c6553be8e2a150e6448a`  
		Last Modified: Tue, 23 Aug 2022 00:56:35 GMT  
		Size: 196.8 MB (196785008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:48f086404ea033fe19fa0dd18cd1989c0b585f07c7353ff246098068b1075971
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.5 MB (295500312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:543ae8ede83fbb55855cee053b3a548534170a1c9e89ce34e227685abb1a46f2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:16:51 GMT
ADD file:132abd62c4fa546798c96d5b1f6f409de9ee27242caf6c479d65309b764c3ece in / 
# Tue, 23 Aug 2022 01:16:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 06:19:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 06:19:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 06:19:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 06:21:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1918e2afd901ca723b3483d8d521789daac45ddbaae2bf9fd813933e826f39b4`  
		Last Modified: Tue, 23 Aug 2022 01:22:10 GMT  
		Size: 52.5 MB (52547848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a58d3f469ed5c6be23bbc74a836bceb306e58e8cd5e58e4464c2b23519543a`  
		Last Modified: Tue, 23 Aug 2022 06:26:58 GMT  
		Size: 5.1 MB (5070690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61379bcded34629fad0582d1d42f2cba36b5f418591509e15301773304e7c7c0`  
		Last Modified: Tue, 23 Aug 2022 06:26:59 GMT  
		Size: 10.6 MB (10573758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c872e375903a379cc5ab82220655ab6973d82f8b48ab51b42d197a4ab189b6b`  
		Last Modified: Tue, 23 Aug 2022 06:27:30 GMT  
		Size: 52.3 MB (52320330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8993dbe2a09d90eb21f3d73a07f953f77bed210372ca285a9f7d8046891b8aa`  
		Last Modified: Tue, 23 Aug 2022 06:28:23 GMT  
		Size: 175.0 MB (174987686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:520bd48d184d2e1e72a3180fb98d6b1a72b711d77e12bcfb2dba659f40f40cc8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.0 MB (282979755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1d91ec2297d651816190904a39f4d4be0b91a78799a8484ab081b8081bd860d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:42:43 GMT
ADD file:21190c24a038c3c9de64b88797bf00e4c4319bd598c7c465cab2ca88d0502416 in / 
# Tue, 23 Aug 2022 01:42:43 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 12:59:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:00:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 13:00:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:01:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c715a126a4d5182c28d2d7b1c81de847bfbbacf6851819fef3eb28e3feb7db0e`  
		Last Modified: Tue, 23 Aug 2022 01:49:30 GMT  
		Size: 50.2 MB (50204931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cecc62e275236714359bda7d1f9c8412e8fa8539f3ef682eebd9c77986c927d`  
		Last Modified: Tue, 23 Aug 2022 13:11:58 GMT  
		Size: 4.9 MB (4930827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818eb872fe75602d611beeac0db63da0a4d8a67aee8b909d5114814f76446a5e`  
		Last Modified: Tue, 23 Aug 2022 13:11:59 GMT  
		Size: 10.2 MB (10217900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94cbc350f4a21916bb6fe70920c962a4889a5059aee86258e4d8263f0c7afbef`  
		Last Modified: Tue, 23 Aug 2022 13:12:28 GMT  
		Size: 50.3 MB (50342476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfc7e160811f0c470f91fe54fc02b224cb6ccbca07472ffcff55826d15bb26d`  
		Last Modified: Tue, 23 Aug 2022 13:13:20 GMT  
		Size: 167.3 MB (167283621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:6a657d9df2ce6540c05ceccaae91f294cb8ad870d9ea7cbc582a0642a5a8e0e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.7 MB (313684616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c31d31f8a9a1673a5b75dcc8e41518512dc0227c069e4cb4a48a9d45a3ade89`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:16 GMT
ADD file:ce6014a27d18915dc6d46c5c1f0f894f0027d1e41fbebb1599c16371b7bab2f1 in / 
# Tue, 23 Aug 2022 01:52:18 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:27:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:28:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 02:28:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:29:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cd84405c8b9e7a8c3d580c2148d25120dd697ea61e1cb55a62f33e67988b7043`  
		Last Modified: Tue, 23 Aug 2022 01:57:29 GMT  
		Size: 53.7 MB (53690830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d98e120b809269e56de468d2b91569789c521011e4d9b1806e43fd04462de2`  
		Last Modified: Tue, 23 Aug 2022 02:36:44 GMT  
		Size: 4.9 MB (4944180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb6be5911b40ca548e48c10b09cb2312f1698b4c84f09711c69389a94b1a8be`  
		Last Modified: Tue, 23 Aug 2022 02:36:44 GMT  
		Size: 10.7 MB (10657442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db608c3c3ce3568556faf63acbc2069811afe242faf8992ccf0ab1986ee38e4f`  
		Last Modified: Tue, 23 Aug 2022 02:37:07 GMT  
		Size: 54.7 MB (54680886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef10f752bfb9bb5888d549687e75a51ad78e1523ee87958e8b464cbd4dee4bb2`  
		Last Modified: Tue, 23 Aug 2022 02:37:46 GMT  
		Size: 189.7 MB (189711278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; 386

```console
$ docker pull buildpack-deps@sha256:6462b9cedd6360f9ac58ef0a745ed79497259cf4382b330b0a6ade58054037fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.8 MB (327786054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a954a50143d33244bd5b54771fe808f36befea012da728e64638c4f80b3f6b8c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:24 GMT
ADD file:4012c41187a03bdb3d37bec80f6255a1d46582e3ed145b4f313e42196529e524 in / 
# Tue, 23 Aug 2022 01:02:25 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:31:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:31:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:32:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:33:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6f683b9c66ef80b527ee5e4cb11969c6e0c1400ab69a4f1279af90f5766d70c7`  
		Last Modified: Tue, 23 Aug 2022 01:07:53 GMT  
		Size: 56.0 MB (56012624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f506948c8aa6d2e0693b583a388ce5e10b4393763bd2ea2529af3bfaa07f0c92`  
		Last Modified: Tue, 23 Aug 2022 01:40:01 GMT  
		Size: 5.1 MB (5085725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915cb3138c0c978b1806934d3f979cff24ecaed321fe7e13caa292cf9ca73dcc`  
		Last Modified: Tue, 23 Aug 2022 01:40:01 GMT  
		Size: 11.0 MB (11032841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc001487b6a15d61b32ac2dbd4b06bdede894077b8fcd3fa2f3969f98052bc3`  
		Last Modified: Tue, 23 Aug 2022 01:40:24 GMT  
		Size: 55.9 MB (55922719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e27a84eb0ba3a89f9e9e474d9c853c2dc7e9c83ef7d1e7281d208fd866b4c3`  
		Last Modified: Tue, 23 Aug 2022 01:41:12 GMT  
		Size: 199.7 MB (199732145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:a2b9c6b327a9a223c3efa1706bc2b9db685a596067cf19dcdd74613196680350
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.1 MB (301099619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44d5d833b9dcbd729eba0daafec46b29b0f0c91fb9dabc2d09bf20e3ce4d4b07`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:10:38 GMT
ADD file:a55d19f262e8338f932ce871c1cbc1718f9f74a5002212f38fea74f3858460a9 in / 
# Tue, 23 Aug 2022 00:10:43 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 22:24:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 22:24:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 22:26:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 22:33:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5ce438ccc597187e8a0dab5cc8906e6a0ec75a9320e55225ad2ec24765f7c0b4`  
		Last Modified: Tue, 23 Aug 2022 00:18:51 GMT  
		Size: 53.3 MB (53272999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567ecdfd8aa8d0bdcecff06b6b73dfbde6ae5451a3afec2a33aee7ca527b61e9`  
		Last Modified: Tue, 23 Aug 2022 22:49:03 GMT  
		Size: 4.9 MB (4918268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9374a0689765aeaeee15bb1c011bddd8cb323e6002385ceb42952a14d3210410`  
		Last Modified: Tue, 23 Aug 2022 22:49:06 GMT  
		Size: 10.7 MB (10661281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ccffd65aa7de17818aaae93c681cc96ca65baf5ab87b1989328259e139d360d`  
		Last Modified: Tue, 23 Aug 2022 22:49:57 GMT  
		Size: 53.3 MB (53304283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba6ce1b89a90d1ecaf04f415e6b8d8885f95ffc7c0a9357b6ef5545fc5e668e2`  
		Last Modified: Tue, 23 Aug 2022 22:52:01 GMT  
		Size: 178.9 MB (178942788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d26e0e6609eee5d0cc12d24a0e666e615785a20c5f2bcc91b8c39a3a1a85d14f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.0 MB (330981508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4404daf2be9fe8125eb280020678875923138a2f95a6de510414b2979fc8ea78`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:24:30 GMT
ADD file:c498f58d8dc50a2a20679642be8f6f43de8b79455438a1c237ef4c94a9ffe34c in / 
# Tue, 23 Aug 2022 01:24:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:58:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:59:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:01:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:62d01a7bda469557451a05bab1d4de7f53dd936e8032b36635019fd54cd927e4`  
		Last Modified: Tue, 23 Aug 2022 01:29:57 GMT  
		Size: 58.9 MB (58909173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b002340b938f821f3b0978eb9bfc47d2b8fe91b33c50508bd618c3c4b0ffe0`  
		Last Modified: Tue, 23 Aug 2022 02:10:43 GMT  
		Size: 5.4 MB (5412576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c65f43f4fd248e0fd18c35535f21fcafa740bdde05c5c367f32926f478e55f`  
		Last Modified: Tue, 23 Aug 2022 02:10:44 GMT  
		Size: 11.6 MB (11628949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6e7f52d8f52b4e830cdd20f538730eebe893f6c1f11aac1d0457ae132da2e8`  
		Last Modified: Tue, 23 Aug 2022 02:11:16 GMT  
		Size: 58.9 MB (58866219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35fecee5c5cd927c82781b73850d4cbf96c866f08985a8a76ee30c510df49f06`  
		Last Modified: Tue, 23 Aug 2022 02:12:17 GMT  
		Size: 196.2 MB (196164591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:7137006106c6222467d1d066c08b261d2ac29572e757ca58573eb833e89bb865
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.1 MB (296058506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:640e9d9a4e7fd555cdb338b68646231938a22a5a3322a831aa6f652376231080`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:53:42 GMT
ADD file:799d2eac4bf12dcb56eca0b771da879e8873a2a81b4d74520db7d6665d448ff6 in / 
# Tue, 23 Aug 2022 00:53:45 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 09:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 09:51:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 09:51:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 09:52:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e8428caa8cb9dd5cd48266f588e1d935181b0d75e5f4680a9d4d03700d44289`  
		Last Modified: Tue, 23 Aug 2022 01:01:15 GMT  
		Size: 53.3 MB (53279185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b41fe9abb9a7707d3bfd9881e997384ad70ba3f811c4152a16e11585318bd5`  
		Last Modified: Tue, 23 Aug 2022 09:59:58 GMT  
		Size: 5.1 MB (5146782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0215c1024f20ea76e1b536fcf226d87a639e72806443621a0bf52a719c0218fd`  
		Last Modified: Tue, 23 Aug 2022 09:59:59 GMT  
		Size: 10.8 MB (10765873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aeff4b644e5176d180f566f9889b6ed12e443f2fb955b119865cc113d26c3b1`  
		Last Modified: Tue, 23 Aug 2022 10:00:19 GMT  
		Size: 54.1 MB (54054805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e54f765beb5bf3b5c78fed34fddcc79e45dd90b63b47b01505666e38691ce6`  
		Last Modified: Tue, 23 Aug 2022 10:00:47 GMT  
		Size: 172.8 MB (172811861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bullseye-curl`

```console
$ docker pull buildpack-deps@sha256:eff18a8892c860c0db39795ed358137ba3216e5d240c912784210b438c28ddd8
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
$ docker pull buildpack-deps@sha256:1188bf8e99d160a3c226aafc7c799a0ad149eb3f6fdb99bddf16d0fc6624aa7c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.0 MB (71047046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3daa7ad5dfdd4bacbfa1c950fe1c68cfd3d10f276bc1218936f710b50c924a5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:40 GMT
ADD file:6944d322f4c04bd2192061822af5cbec8ac0a6b424c461d66174d32aed604972 in / 
# Tue, 23 Aug 2022 00:20:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:48:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:48:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1671565cc8df8c365c9b661d3fbc164e73d01f1b0430c6179588428f99a9da2e`  
		Last Modified: Tue, 23 Aug 2022 00:24:32 GMT  
		Size: 55.0 MB (55007555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e94d13e55e7a4ef17ff21376f57fb95c7e1706931f8704aa99260968d81f6e4`  
		Last Modified: Tue, 23 Aug 2022 00:55:37 GMT  
		Size: 5.2 MB (5163019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9c7528c685216129e8e67bf362a7702e7b1daa585ab85546a41508830657d6`  
		Last Modified: Tue, 23 Aug 2022 00:55:38 GMT  
		Size: 10.9 MB (10876472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:9241cca9693c0372458ebec46ddb886fc0bffe1b9aeee2c7d4dfc0050b1a55d0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.2 MB (68192296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f44e91617f5732bcc2b11f0aa7d00e23d82a7b4f67e4d5a7787a52433fa706df`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:16:51 GMT
ADD file:132abd62c4fa546798c96d5b1f6f409de9ee27242caf6c479d65309b764c3ece in / 
# Tue, 23 Aug 2022 01:16:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 06:19:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 06:19:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1918e2afd901ca723b3483d8d521789daac45ddbaae2bf9fd813933e826f39b4`  
		Last Modified: Tue, 23 Aug 2022 01:22:10 GMT  
		Size: 52.5 MB (52547848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a58d3f469ed5c6be23bbc74a836bceb306e58e8cd5e58e4464c2b23519543a`  
		Last Modified: Tue, 23 Aug 2022 06:26:58 GMT  
		Size: 5.1 MB (5070690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61379bcded34629fad0582d1d42f2cba36b5f418591509e15301773304e7c7c0`  
		Last Modified: Tue, 23 Aug 2022 06:26:59 GMT  
		Size: 10.6 MB (10573758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:56c33d4b477957b573aed7cc5367f95d01459a2a0a6312c42994c79f488b1cdc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65353658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f92c349465773257e5ffe974e22d6a19ca708f3db946ebf552668157b43ba5c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:42:43 GMT
ADD file:21190c24a038c3c9de64b88797bf00e4c4319bd598c7c465cab2ca88d0502416 in / 
# Tue, 23 Aug 2022 01:42:43 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 12:59:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:00:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c715a126a4d5182c28d2d7b1c81de847bfbbacf6851819fef3eb28e3feb7db0e`  
		Last Modified: Tue, 23 Aug 2022 01:49:30 GMT  
		Size: 50.2 MB (50204931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cecc62e275236714359bda7d1f9c8412e8fa8539f3ef682eebd9c77986c927d`  
		Last Modified: Tue, 23 Aug 2022 13:11:58 GMT  
		Size: 4.9 MB (4930827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818eb872fe75602d611beeac0db63da0a4d8a67aee8b909d5114814f76446a5e`  
		Last Modified: Tue, 23 Aug 2022 13:11:59 GMT  
		Size: 10.2 MB (10217900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:224dfb7f5032a11af8748f4e65daa8f50f478612b91b1c9176a7ef035ed374ba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.3 MB (69292452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93d7443e4194085764e49b9d96d081bc973eba35516e6d88b0058b0854b2970e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:16 GMT
ADD file:ce6014a27d18915dc6d46c5c1f0f894f0027d1e41fbebb1599c16371b7bab2f1 in / 
# Tue, 23 Aug 2022 01:52:18 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:27:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:28:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:cd84405c8b9e7a8c3d580c2148d25120dd697ea61e1cb55a62f33e67988b7043`  
		Last Modified: Tue, 23 Aug 2022 01:57:29 GMT  
		Size: 53.7 MB (53690830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d98e120b809269e56de468d2b91569789c521011e4d9b1806e43fd04462de2`  
		Last Modified: Tue, 23 Aug 2022 02:36:44 GMT  
		Size: 4.9 MB (4944180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb6be5911b40ca548e48c10b09cb2312f1698b4c84f09711c69389a94b1a8be`  
		Last Modified: Tue, 23 Aug 2022 02:36:44 GMT  
		Size: 10.7 MB (10657442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:0d9e01a77b19864476557d06dadfb768771a3b89333dbbf3b7c3fd10138e3fa7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.1 MB (72131190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c00fec5790de3e13e4285b83054a6850bd58812ba11a6858bbfc8607533256b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:24 GMT
ADD file:4012c41187a03bdb3d37bec80f6255a1d46582e3ed145b4f313e42196529e524 in / 
# Tue, 23 Aug 2022 01:02:25 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:31:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:31:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6f683b9c66ef80b527ee5e4cb11969c6e0c1400ab69a4f1279af90f5766d70c7`  
		Last Modified: Tue, 23 Aug 2022 01:07:53 GMT  
		Size: 56.0 MB (56012624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f506948c8aa6d2e0693b583a388ce5e10b4393763bd2ea2529af3bfaa07f0c92`  
		Last Modified: Tue, 23 Aug 2022 01:40:01 GMT  
		Size: 5.1 MB (5085725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915cb3138c0c978b1806934d3f979cff24ecaed321fe7e13caa292cf9ca73dcc`  
		Last Modified: Tue, 23 Aug 2022 01:40:01 GMT  
		Size: 11.0 MB (11032841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:b88de28a9b03c3efa219ebe99731c2dcf063299c1769c16ab9fe8fdacf59ff38
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68852548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15015eb73f5ade0114232ff8e03c9c853246f11dd35a7f95196f6c3eef74d820`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:10:38 GMT
ADD file:a55d19f262e8338f932ce871c1cbc1718f9f74a5002212f38fea74f3858460a9 in / 
# Tue, 23 Aug 2022 00:10:43 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 22:24:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 22:24:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5ce438ccc597187e8a0dab5cc8906e6a0ec75a9320e55225ad2ec24765f7c0b4`  
		Last Modified: Tue, 23 Aug 2022 00:18:51 GMT  
		Size: 53.3 MB (53272999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567ecdfd8aa8d0bdcecff06b6b73dfbde6ae5451a3afec2a33aee7ca527b61e9`  
		Last Modified: Tue, 23 Aug 2022 22:49:03 GMT  
		Size: 4.9 MB (4918268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9374a0689765aeaeee15bb1c011bddd8cb323e6002385ceb42952a14d3210410`  
		Last Modified: Tue, 23 Aug 2022 22:49:06 GMT  
		Size: 10.7 MB (10661281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d8b7e1a18e133da0ea19134be7a76cdd22ec4f10fb6a01976563fcbea1555ce0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.0 MB (75950698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d703a630725af8cf9c5a1f40484ae8fc94e5360d191852caf1164235d16cd71`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:24:30 GMT
ADD file:c498f58d8dc50a2a20679642be8f6f43de8b79455438a1c237ef4c94a9ffe34c in / 
# Tue, 23 Aug 2022 01:24:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:58:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:62d01a7bda469557451a05bab1d4de7f53dd936e8032b36635019fd54cd927e4`  
		Last Modified: Tue, 23 Aug 2022 01:29:57 GMT  
		Size: 58.9 MB (58909173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b002340b938f821f3b0978eb9bfc47d2b8fe91b33c50508bd618c3c4b0ffe0`  
		Last Modified: Tue, 23 Aug 2022 02:10:43 GMT  
		Size: 5.4 MB (5412576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c65f43f4fd248e0fd18c35535f21fcafa740bdde05c5c367f32926f478e55f`  
		Last Modified: Tue, 23 Aug 2022 02:10:44 GMT  
		Size: 11.6 MB (11628949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:8d5fc4782913393f45ddd1ea898bcb30f1bb102bcf7d603315f3a6aaec9ea202
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69191840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a21a8727c9bc59c13f1f4b1072ecef25e905519ec56c0235f3a2d399dbdede69`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:53:42 GMT
ADD file:799d2eac4bf12dcb56eca0b771da879e8873a2a81b4d74520db7d6665d448ff6 in / 
# Tue, 23 Aug 2022 00:53:45 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 09:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 09:51:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6e8428caa8cb9dd5cd48266f588e1d935181b0d75e5f4680a9d4d03700d44289`  
		Last Modified: Tue, 23 Aug 2022 01:01:15 GMT  
		Size: 53.3 MB (53279185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b41fe9abb9a7707d3bfd9881e997384ad70ba3f811c4152a16e11585318bd5`  
		Last Modified: Tue, 23 Aug 2022 09:59:58 GMT  
		Size: 5.1 MB (5146782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0215c1024f20ea76e1b536fcf226d87a639e72806443621a0bf52a719c0218fd`  
		Last Modified: Tue, 23 Aug 2022 09:59:59 GMT  
		Size: 10.8 MB (10765873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bullseye-scm`

```console
$ docker pull buildpack-deps@sha256:a7a9dbad2a104ca82facdb49ca65421b485045a3a51aad05bd44609b839401a1
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
$ docker pull buildpack-deps@sha256:6c1872f4ea21628b7c323305593b94d6ecc5125852b4a03827c6d38b473835d2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.6 MB (125631181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e73278505bb143c007d79f686483ae493b77ad2ad4f7cadc67deeb86f4dd38e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:40 GMT
ADD file:6944d322f4c04bd2192061822af5cbec8ac0a6b424c461d66174d32aed604972 in / 
# Tue, 23 Aug 2022 00:20:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:48:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:48:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 00:48:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1671565cc8df8c365c9b661d3fbc164e73d01f1b0430c6179588428f99a9da2e`  
		Last Modified: Tue, 23 Aug 2022 00:24:32 GMT  
		Size: 55.0 MB (55007555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e94d13e55e7a4ef17ff21376f57fb95c7e1706931f8704aa99260968d81f6e4`  
		Last Modified: Tue, 23 Aug 2022 00:55:37 GMT  
		Size: 5.2 MB (5163019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9c7528c685216129e8e67bf362a7702e7b1daa585ab85546a41508830657d6`  
		Last Modified: Tue, 23 Aug 2022 00:55:38 GMT  
		Size: 10.9 MB (10876472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ad072f9cd16fc8eb93b182b20e758e11acc0ef60babef0bf1043c08de1901a`  
		Last Modified: Tue, 23 Aug 2022 00:55:57 GMT  
		Size: 54.6 MB (54584135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:f544bf2e62950527f9e904a056de2ffc7f7d57a0051cc0a83f53029d715f2847
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.5 MB (120512626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:254098229367b0e03446fdc4d0858c497972184186719e50d9853daf38a33bb0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:16:51 GMT
ADD file:132abd62c4fa546798c96d5b1f6f409de9ee27242caf6c479d65309b764c3ece in / 
# Tue, 23 Aug 2022 01:16:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 06:19:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 06:19:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 06:19:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1918e2afd901ca723b3483d8d521789daac45ddbaae2bf9fd813933e826f39b4`  
		Last Modified: Tue, 23 Aug 2022 01:22:10 GMT  
		Size: 52.5 MB (52547848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a58d3f469ed5c6be23bbc74a836bceb306e58e8cd5e58e4464c2b23519543a`  
		Last Modified: Tue, 23 Aug 2022 06:26:58 GMT  
		Size: 5.1 MB (5070690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61379bcded34629fad0582d1d42f2cba36b5f418591509e15301773304e7c7c0`  
		Last Modified: Tue, 23 Aug 2022 06:26:59 GMT  
		Size: 10.6 MB (10573758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c872e375903a379cc5ab82220655ab6973d82f8b48ab51b42d197a4ab189b6b`  
		Last Modified: Tue, 23 Aug 2022 06:27:30 GMT  
		Size: 52.3 MB (52320330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:495a7139ac1f0b677a9476288d454f9dfd4763312ef4dc4d467ce3f29c36caed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.7 MB (115696134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e362c69b51c9b48c55b381399fc2b7a49ec81e115a633a60638b43084b817c9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:42:43 GMT
ADD file:21190c24a038c3c9de64b88797bf00e4c4319bd598c7c465cab2ca88d0502416 in / 
# Tue, 23 Aug 2022 01:42:43 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 12:59:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:00:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 13:00:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c715a126a4d5182c28d2d7b1c81de847bfbbacf6851819fef3eb28e3feb7db0e`  
		Last Modified: Tue, 23 Aug 2022 01:49:30 GMT  
		Size: 50.2 MB (50204931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cecc62e275236714359bda7d1f9c8412e8fa8539f3ef682eebd9c77986c927d`  
		Last Modified: Tue, 23 Aug 2022 13:11:58 GMT  
		Size: 4.9 MB (4930827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818eb872fe75602d611beeac0db63da0a4d8a67aee8b909d5114814f76446a5e`  
		Last Modified: Tue, 23 Aug 2022 13:11:59 GMT  
		Size: 10.2 MB (10217900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94cbc350f4a21916bb6fe70920c962a4889a5059aee86258e4d8263f0c7afbef`  
		Last Modified: Tue, 23 Aug 2022 13:12:28 GMT  
		Size: 50.3 MB (50342476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:5156f3bb278fb0dda42cdf0b406331f8809ab19a049e6ea5506665811c002475
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.0 MB (123973338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acf31c8a1856f38bfa1a001f3b72d3e9678c5aadee3ec10352d90f571361e1fe`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:16 GMT
ADD file:ce6014a27d18915dc6d46c5c1f0f894f0027d1e41fbebb1599c16371b7bab2f1 in / 
# Tue, 23 Aug 2022 01:52:18 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:27:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:28:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 02:28:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cd84405c8b9e7a8c3d580c2148d25120dd697ea61e1cb55a62f33e67988b7043`  
		Last Modified: Tue, 23 Aug 2022 01:57:29 GMT  
		Size: 53.7 MB (53690830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d98e120b809269e56de468d2b91569789c521011e4d9b1806e43fd04462de2`  
		Last Modified: Tue, 23 Aug 2022 02:36:44 GMT  
		Size: 4.9 MB (4944180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb6be5911b40ca548e48c10b09cb2312f1698b4c84f09711c69389a94b1a8be`  
		Last Modified: Tue, 23 Aug 2022 02:36:44 GMT  
		Size: 10.7 MB (10657442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db608c3c3ce3568556faf63acbc2069811afe242faf8992ccf0ab1986ee38e4f`  
		Last Modified: Tue, 23 Aug 2022 02:37:07 GMT  
		Size: 54.7 MB (54680886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:1afc200fb3ee2b4b85c5c984fbbc088ff53286077a843588bc04c935cd6b7416
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.1 MB (128053909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bceeed6ce487fd59052390091c5f4300ff05ada27c1650c1dbf83f91a4d9788b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:24 GMT
ADD file:4012c41187a03bdb3d37bec80f6255a1d46582e3ed145b4f313e42196529e524 in / 
# Tue, 23 Aug 2022 01:02:25 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:31:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:31:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:32:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6f683b9c66ef80b527ee5e4cb11969c6e0c1400ab69a4f1279af90f5766d70c7`  
		Last Modified: Tue, 23 Aug 2022 01:07:53 GMT  
		Size: 56.0 MB (56012624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f506948c8aa6d2e0693b583a388ce5e10b4393763bd2ea2529af3bfaa07f0c92`  
		Last Modified: Tue, 23 Aug 2022 01:40:01 GMT  
		Size: 5.1 MB (5085725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915cb3138c0c978b1806934d3f979cff24ecaed321fe7e13caa292cf9ca73dcc`  
		Last Modified: Tue, 23 Aug 2022 01:40:01 GMT  
		Size: 11.0 MB (11032841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc001487b6a15d61b32ac2dbd4b06bdede894077b8fcd3fa2f3969f98052bc3`  
		Last Modified: Tue, 23 Aug 2022 01:40:24 GMT  
		Size: 55.9 MB (55922719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:c8f075c6f8d978558f03a94da80ad547aa3e8af5a92a9b3d461d8db9b40542bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122156831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fdba3c8b6471cc9b1138ee1a4111402f4476b568b1735d38c33912c379db3b3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:10:38 GMT
ADD file:a55d19f262e8338f932ce871c1cbc1718f9f74a5002212f38fea74f3858460a9 in / 
# Tue, 23 Aug 2022 00:10:43 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 22:24:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 22:24:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 22:26:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5ce438ccc597187e8a0dab5cc8906e6a0ec75a9320e55225ad2ec24765f7c0b4`  
		Last Modified: Tue, 23 Aug 2022 00:18:51 GMT  
		Size: 53.3 MB (53272999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567ecdfd8aa8d0bdcecff06b6b73dfbde6ae5451a3afec2a33aee7ca527b61e9`  
		Last Modified: Tue, 23 Aug 2022 22:49:03 GMT  
		Size: 4.9 MB (4918268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9374a0689765aeaeee15bb1c011bddd8cb323e6002385ceb42952a14d3210410`  
		Last Modified: Tue, 23 Aug 2022 22:49:06 GMT  
		Size: 10.7 MB (10661281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ccffd65aa7de17818aaae93c681cc96ca65baf5ab87b1989328259e139d360d`  
		Last Modified: Tue, 23 Aug 2022 22:49:57 GMT  
		Size: 53.3 MB (53304283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:cb31310b3598fc3d3ad9daa40df9a133a6e2e360aee409d29191203c4686d095
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134816917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30881ed3045278b91be936aafc665ff71cd8bc93d39d8b69650de485729b3d02`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:24:30 GMT
ADD file:c498f58d8dc50a2a20679642be8f6f43de8b79455438a1c237ef4c94a9ffe34c in / 
# Tue, 23 Aug 2022 01:24:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:58:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:59:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:62d01a7bda469557451a05bab1d4de7f53dd936e8032b36635019fd54cd927e4`  
		Last Modified: Tue, 23 Aug 2022 01:29:57 GMT  
		Size: 58.9 MB (58909173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b002340b938f821f3b0978eb9bfc47d2b8fe91b33c50508bd618c3c4b0ffe0`  
		Last Modified: Tue, 23 Aug 2022 02:10:43 GMT  
		Size: 5.4 MB (5412576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c65f43f4fd248e0fd18c35535f21fcafa740bdde05c5c367f32926f478e55f`  
		Last Modified: Tue, 23 Aug 2022 02:10:44 GMT  
		Size: 11.6 MB (11628949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6e7f52d8f52b4e830cdd20f538730eebe893f6c1f11aac1d0457ae132da2e8`  
		Last Modified: Tue, 23 Aug 2022 02:11:16 GMT  
		Size: 58.9 MB (58866219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:fe781f689e6f87bbf043328a5546a3c8810e4bb71bf4aace341aa84bc8e2aab4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123246645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd05daa086ec2eb9eb0d8724cfebe627e1a621d31c39e41c49c480e60b4413fd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:53:42 GMT
ADD file:799d2eac4bf12dcb56eca0b771da879e8873a2a81b4d74520db7d6665d448ff6 in / 
# Tue, 23 Aug 2022 00:53:45 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 09:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 09:51:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 09:51:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e8428caa8cb9dd5cd48266f588e1d935181b0d75e5f4680a9d4d03700d44289`  
		Last Modified: Tue, 23 Aug 2022 01:01:15 GMT  
		Size: 53.3 MB (53279185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b41fe9abb9a7707d3bfd9881e997384ad70ba3f811c4152a16e11585318bd5`  
		Last Modified: Tue, 23 Aug 2022 09:59:58 GMT  
		Size: 5.1 MB (5146782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0215c1024f20ea76e1b536fcf226d87a639e72806443621a0bf52a719c0218fd`  
		Last Modified: Tue, 23 Aug 2022 09:59:59 GMT  
		Size: 10.8 MB (10765873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aeff4b644e5176d180f566f9889b6ed12e443f2fb955b119865cc113d26c3b1`  
		Last Modified: Tue, 23 Aug 2022 10:00:19 GMT  
		Size: 54.1 MB (54054805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:buster`

```console
$ docker pull buildpack-deps@sha256:d73ba7863f3958cade1ef32f7620c3751ba5cd9653ff382a1b222ec17906884e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:buster` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:54ef455d50cec890ed58b814dd005747a088aeff36543169bc85c99b9ceba5a5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.6 MB (312645189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7f74fbf296e791b18cd52ed04807250ec4ec525b4305015447d0660198477c5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:00 GMT
ADD file:d420ffdf63082e03517284553796e5a100e425201458860f07b1aa8598c5929a in / 
# Tue, 23 Aug 2022 00:21:00 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:49:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:49:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 00:49:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:50:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76dff75df4d9dbdf29a4459adaec745740bfb476cd915906e33eddd9cd94db93`  
		Last Modified: Tue, 23 Aug 2022 00:25:20 GMT  
		Size: 50.4 MB (50440273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8c90a1c4bb422a88cc9ff532712db3c6a7a8cdc5030af2e60ec51947f2c8aa`  
		Last Modified: Tue, 23 Aug 2022 00:56:49 GMT  
		Size: 7.9 MB (7856913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3662c1050803c4e17c1848dffe636eae5e6e5aafb8f1fffcf82248ccfef21c2`  
		Last Modified: Tue, 23 Aug 2022 00:56:49 GMT  
		Size: 10.0 MB (9998130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5dcb7dd59206e662084addf318ef296595c82800a9107e362439db4c158df9`  
		Last Modified: Tue, 23 Aug 2022 00:57:06 GMT  
		Size: 51.8 MB (51843805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa57cc7ce3410dc0507beaaf475eb582c5ffccea2d603d2c024b77a69990aba2`  
		Last Modified: Tue, 23 Aug 2022 00:57:40 GMT  
		Size: 192.5 MB (192506068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:e67231ddffab43682ab5597e54d94ccb319a189890cd39e8ca9627a3ce4b1a78
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.5 MB (278465267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f54ac2d77406431a8ece5e7baf1d11a14105ce733fe737b9be9dd484ec6e41e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:18 GMT
ADD file:f02e7759ba5d55ff457d421191df7d2973666205453bbb6755214288b1c5527b in / 
# Tue, 23 Aug 2022 01:43:19 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 13:02:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:02:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 13:02:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:03:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e43c24e08caa0d5875ad9b74a9503702850e39637c5dfe8cf2b231adfb60322c`  
		Last Modified: Tue, 23 Aug 2022 01:50:31 GMT  
		Size: 45.9 MB (45914940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:336dc8987db19d66a0f9f594deebb34a07cbdbc58f4ca037260b77716ac3762f`  
		Last Modified: Tue, 23 Aug 2022 13:13:39 GMT  
		Size: 7.1 MB (7145481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d4e661f35fcba3168ad779ef39cc7bbebaea0a1ab6977ea6a07497f64f1545`  
		Last Modified: Tue, 23 Aug 2022 13:13:39 GMT  
		Size: 9.3 MB (9344463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34357d0aae8fbf38566a850196f436a0111c5c9eeb3a27256f78dfcff8ea6981`  
		Last Modified: Tue, 23 Aug 2022 13:14:04 GMT  
		Size: 47.4 MB (47359364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b803711841bad336591ae6cde869b0acee5e53607ac006c3205ce3f2594f71`  
		Last Modified: Tue, 23 Aug 2022 13:14:52 GMT  
		Size: 168.7 MB (168701019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:8b05537816456d43a93b68f81bdf4864538ab9f22e43c3bc67be6e2e5142fe80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.0 MB (302979491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e148476bf876492d4a04bfdec4c4cc661f95bdee63f910dd2a353200c39cff41`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:43 GMT
ADD file:a3ba1802e6680a14c605fbe754f9fb56a642f0799f51ce0010d253cb66c9691f in / 
# Tue, 23 Aug 2022 01:52:44 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:29:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:29:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 02:29:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:30:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3332e5c67ba650c61dbca801cf2739a1f5b6faac33f7b0543f97f4ab1165fe69`  
		Last Modified: Tue, 23 Aug 2022 01:58:23 GMT  
		Size: 49.2 MB (49228066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61dd9df5607d27eb8d7af8db0ec4f1e1634f54db08cd06c03131ac8a25ff710b`  
		Last Modified: Tue, 23 Aug 2022 02:38:02 GMT  
		Size: 7.7 MB (7720187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28122dfd7d7cf006c384197d918567d3d812f94f0030b87104b26c2d2ded69a`  
		Last Modified: Tue, 23 Aug 2022 02:38:02 GMT  
		Size: 9.8 MB (9768739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e3536e0d6df43cb88858e2f77eaa514bd51e583a6d593d494fcb67e03bfda1`  
		Last Modified: Tue, 23 Aug 2022 02:38:21 GMT  
		Size: 52.2 MB (52174764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34806818c453e9a369973b475f26ada73304ea74e3ae1860af58abbe6872a7c`  
		Last Modified: Tue, 23 Aug 2022 02:38:56 GMT  
		Size: 184.1 MB (184087735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; 386

```console
$ docker pull buildpack-deps@sha256:5be2d7d74dcf23d0c9e478b0c6a4210d4af26c55053c9a3f25a7a3ec6f3e3a3d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.8 MB (321826790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef7f83e2174f51cd4b5480254a81d9d5eade013377c85039ee068ab9960f7923`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:51 GMT
ADD file:7ad537f8110f70df174d79a50cbe08fc480933797f0717e94529061bbfd00759 in / 
# Tue, 23 Aug 2022 01:02:52 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:33:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:33:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:33:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:35:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f73bf17b8a4e28cf438c1af60c558d4943ab3fea50a934b856e19e18b2cefc70`  
		Last Modified: Tue, 23 Aug 2022 01:08:52 GMT  
		Size: 51.2 MB (51202934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f552c2f5ee3c58b15814627cdfd5f450b32574510bab9c05fcdcfee72a5937`  
		Last Modified: Tue, 23 Aug 2022 01:41:27 GMT  
		Size: 8.0 MB (8022887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f116e2a9c83bb2f0fa2b290281df8f4dc03cd9f375f5b485cc3811581f843efb`  
		Last Modified: Tue, 23 Aug 2022 01:41:27 GMT  
		Size: 10.1 MB (10123789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8adc65b9373ec90849e46f84946cc18555ee8bd2be22479432d05734cc9738ac`  
		Last Modified: Tue, 23 Aug 2022 01:41:47 GMT  
		Size: 53.4 MB (53443079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0a01d7abbb9d320a302f32c458653f6d3dded4b42a38c0118e8e4ecbd4d4d9`  
		Last Modified: Tue, 23 Aug 2022 01:42:22 GMT  
		Size: 199.0 MB (199034101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:buster-curl`

```console
$ docker pull buildpack-deps@sha256:ac3799eb356b54a0e444ec493fa1b135da74a0dad504461b33d31b24e89af24a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:buster-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:8e5706c8aebcc047d936e740c3c19f0590273be5d60219de6de26931a0b4d300
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68295316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d50e24bcc3757da5bdbefd30f0ac73d015c6924ff9b170bdb884618259d23058`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:00 GMT
ADD file:d420ffdf63082e03517284553796e5a100e425201458860f07b1aa8598c5929a in / 
# Tue, 23 Aug 2022 00:21:00 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:49:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:49:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:76dff75df4d9dbdf29a4459adaec745740bfb476cd915906e33eddd9cd94db93`  
		Last Modified: Tue, 23 Aug 2022 00:25:20 GMT  
		Size: 50.4 MB (50440273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8c90a1c4bb422a88cc9ff532712db3c6a7a8cdc5030af2e60ec51947f2c8aa`  
		Last Modified: Tue, 23 Aug 2022 00:56:49 GMT  
		Size: 7.9 MB (7856913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3662c1050803c4e17c1848dffe636eae5e6e5aafb8f1fffcf82248ccfef21c2`  
		Last Modified: Tue, 23 Aug 2022 00:56:49 GMT  
		Size: 10.0 MB (9998130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:72aea0997fe2f3d263507c131f7c5480bd9bfb889795778b8ce9ebb939ff2015
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62404884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c74b374874b15e1eea9e762b24cc862a89f75413a8c654b76ad75567c76af52`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:18 GMT
ADD file:f02e7759ba5d55ff457d421191df7d2973666205453bbb6755214288b1c5527b in / 
# Tue, 23 Aug 2022 01:43:19 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 13:02:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:02:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e43c24e08caa0d5875ad9b74a9503702850e39637c5dfe8cf2b231adfb60322c`  
		Last Modified: Tue, 23 Aug 2022 01:50:31 GMT  
		Size: 45.9 MB (45914940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:336dc8987db19d66a0f9f594deebb34a07cbdbc58f4ca037260b77716ac3762f`  
		Last Modified: Tue, 23 Aug 2022 13:13:39 GMT  
		Size: 7.1 MB (7145481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d4e661f35fcba3168ad779ef39cc7bbebaea0a1ab6977ea6a07497f64f1545`  
		Last Modified: Tue, 23 Aug 2022 13:13:39 GMT  
		Size: 9.3 MB (9344463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:528364512919c0312fa735c9613c158e8f3f48ad9e975b98c070c5cbaf2169a6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66716992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42ed8e9cb3fefc1dcc0bdf879faa7bce5abc302af284c835bfd67a6270c8e94c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:43 GMT
ADD file:a3ba1802e6680a14c605fbe754f9fb56a642f0799f51ce0010d253cb66c9691f in / 
# Tue, 23 Aug 2022 01:52:44 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:29:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:29:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3332e5c67ba650c61dbca801cf2739a1f5b6faac33f7b0543f97f4ab1165fe69`  
		Last Modified: Tue, 23 Aug 2022 01:58:23 GMT  
		Size: 49.2 MB (49228066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61dd9df5607d27eb8d7af8db0ec4f1e1634f54db08cd06c03131ac8a25ff710b`  
		Last Modified: Tue, 23 Aug 2022 02:38:02 GMT  
		Size: 7.7 MB (7720187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28122dfd7d7cf006c384197d918567d3d812f94f0030b87104b26c2d2ded69a`  
		Last Modified: Tue, 23 Aug 2022 02:38:02 GMT  
		Size: 9.8 MB (9768739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:4545f198fdceaa38ea7eb36df694364dd649e58010fdc8f6e4b1b1a07a31c0aa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.3 MB (69349610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2bbae5151d08a59f94a679035d3279d0bb5385445c5b24a6a49ac9093adacb4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:51 GMT
ADD file:7ad537f8110f70df174d79a50cbe08fc480933797f0717e94529061bbfd00759 in / 
# Tue, 23 Aug 2022 01:02:52 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:33:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:33:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f73bf17b8a4e28cf438c1af60c558d4943ab3fea50a934b856e19e18b2cefc70`  
		Last Modified: Tue, 23 Aug 2022 01:08:52 GMT  
		Size: 51.2 MB (51202934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f552c2f5ee3c58b15814627cdfd5f450b32574510bab9c05fcdcfee72a5937`  
		Last Modified: Tue, 23 Aug 2022 01:41:27 GMT  
		Size: 8.0 MB (8022887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f116e2a9c83bb2f0fa2b290281df8f4dc03cd9f375f5b485cc3811581f843efb`  
		Last Modified: Tue, 23 Aug 2022 01:41:27 GMT  
		Size: 10.1 MB (10123789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:buster-scm`

```console
$ docker pull buildpack-deps@sha256:ef0eccf4ba6e75c9d8ceb8d2163039218338706f9d229ec9210dc786d4f25dbf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:buster-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:003fbe71ab8e0aa49a38abea68017b20ade0244ca7fd112545f34d00e8d93f29
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120139121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d1c17948b08f2ddc164ca234f7b968e456395dba24dca1bebba323717197e8a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:00 GMT
ADD file:d420ffdf63082e03517284553796e5a100e425201458860f07b1aa8598c5929a in / 
# Tue, 23 Aug 2022 00:21:00 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:49:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:49:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 00:49:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76dff75df4d9dbdf29a4459adaec745740bfb476cd915906e33eddd9cd94db93`  
		Last Modified: Tue, 23 Aug 2022 00:25:20 GMT  
		Size: 50.4 MB (50440273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8c90a1c4bb422a88cc9ff532712db3c6a7a8cdc5030af2e60ec51947f2c8aa`  
		Last Modified: Tue, 23 Aug 2022 00:56:49 GMT  
		Size: 7.9 MB (7856913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3662c1050803c4e17c1848dffe636eae5e6e5aafb8f1fffcf82248ccfef21c2`  
		Last Modified: Tue, 23 Aug 2022 00:56:49 GMT  
		Size: 10.0 MB (9998130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5dcb7dd59206e662084addf318ef296595c82800a9107e362439db4c158df9`  
		Last Modified: Tue, 23 Aug 2022 00:57:06 GMT  
		Size: 51.8 MB (51843805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:cf25863e9e2ffa09317a598c2342c471a94d6c51cf58f59a7bf46b54a0851382
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109764248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:158dff8b83e31481d64645d01a2bbf745206bad2d79112ffa570cb67c17ebd69`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:18 GMT
ADD file:f02e7759ba5d55ff457d421191df7d2973666205453bbb6755214288b1c5527b in / 
# Tue, 23 Aug 2022 01:43:19 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 13:02:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:02:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 13:02:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e43c24e08caa0d5875ad9b74a9503702850e39637c5dfe8cf2b231adfb60322c`  
		Last Modified: Tue, 23 Aug 2022 01:50:31 GMT  
		Size: 45.9 MB (45914940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:336dc8987db19d66a0f9f594deebb34a07cbdbc58f4ca037260b77716ac3762f`  
		Last Modified: Tue, 23 Aug 2022 13:13:39 GMT  
		Size: 7.1 MB (7145481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d4e661f35fcba3168ad779ef39cc7bbebaea0a1ab6977ea6a07497f64f1545`  
		Last Modified: Tue, 23 Aug 2022 13:13:39 GMT  
		Size: 9.3 MB (9344463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34357d0aae8fbf38566a850196f436a0111c5c9eeb3a27256f78dfcff8ea6981`  
		Last Modified: Tue, 23 Aug 2022 13:14:04 GMT  
		Size: 47.4 MB (47359364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:687528f9bc5cc2787143f4aa993a59abb154dd027597b4ac853e084bff5f3202
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.9 MB (118891756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b51c54783cb65ffe0a52ebda1f30f9e23ae93f8e0572f8210d6c71bcee8184b9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:43 GMT
ADD file:a3ba1802e6680a14c605fbe754f9fb56a642f0799f51ce0010d253cb66c9691f in / 
# Tue, 23 Aug 2022 01:52:44 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:29:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:29:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 02:29:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3332e5c67ba650c61dbca801cf2739a1f5b6faac33f7b0543f97f4ab1165fe69`  
		Last Modified: Tue, 23 Aug 2022 01:58:23 GMT  
		Size: 49.2 MB (49228066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61dd9df5607d27eb8d7af8db0ec4f1e1634f54db08cd06c03131ac8a25ff710b`  
		Last Modified: Tue, 23 Aug 2022 02:38:02 GMT  
		Size: 7.7 MB (7720187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28122dfd7d7cf006c384197d918567d3d812f94f0030b87104b26c2d2ded69a`  
		Last Modified: Tue, 23 Aug 2022 02:38:02 GMT  
		Size: 9.8 MB (9768739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e3536e0d6df43cb88858e2f77eaa514bd51e583a6d593d494fcb67e03bfda1`  
		Last Modified: Tue, 23 Aug 2022 02:38:21 GMT  
		Size: 52.2 MB (52174764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:1b34deb70dfb8cdc508587152cf0e8400942901fcc8bb73787257dfb00876070
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.8 MB (122792689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d1b8cd3e85526cbf00e64aeb0a2fa39cf32001886e42e38f6ab3d923d2091d6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:51 GMT
ADD file:7ad537f8110f70df174d79a50cbe08fc480933797f0717e94529061bbfd00759 in / 
# Tue, 23 Aug 2022 01:02:52 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:33:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:33:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:33:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f73bf17b8a4e28cf438c1af60c558d4943ab3fea50a934b856e19e18b2cefc70`  
		Last Modified: Tue, 23 Aug 2022 01:08:52 GMT  
		Size: 51.2 MB (51202934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f552c2f5ee3c58b15814627cdfd5f450b32574510bab9c05fcdcfee72a5937`  
		Last Modified: Tue, 23 Aug 2022 01:41:27 GMT  
		Size: 8.0 MB (8022887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f116e2a9c83bb2f0fa2b290281df8f4dc03cd9f375f5b485cc3811581f843efb`  
		Last Modified: Tue, 23 Aug 2022 01:41:27 GMT  
		Size: 10.1 MB (10123789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8adc65b9373ec90849e46f84946cc18555ee8bd2be22479432d05734cc9738ac`  
		Last Modified: Tue, 23 Aug 2022 01:41:47 GMT  
		Size: 53.4 MB (53443079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:curl`

```console
$ docker pull buildpack-deps@sha256:eff18a8892c860c0db39795ed358137ba3216e5d240c912784210b438c28ddd8
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
$ docker pull buildpack-deps@sha256:1188bf8e99d160a3c226aafc7c799a0ad149eb3f6fdb99bddf16d0fc6624aa7c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.0 MB (71047046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3daa7ad5dfdd4bacbfa1c950fe1c68cfd3d10f276bc1218936f710b50c924a5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:40 GMT
ADD file:6944d322f4c04bd2192061822af5cbec8ac0a6b424c461d66174d32aed604972 in / 
# Tue, 23 Aug 2022 00:20:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:48:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:48:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1671565cc8df8c365c9b661d3fbc164e73d01f1b0430c6179588428f99a9da2e`  
		Last Modified: Tue, 23 Aug 2022 00:24:32 GMT  
		Size: 55.0 MB (55007555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e94d13e55e7a4ef17ff21376f57fb95c7e1706931f8704aa99260968d81f6e4`  
		Last Modified: Tue, 23 Aug 2022 00:55:37 GMT  
		Size: 5.2 MB (5163019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9c7528c685216129e8e67bf362a7702e7b1daa585ab85546a41508830657d6`  
		Last Modified: Tue, 23 Aug 2022 00:55:38 GMT  
		Size: 10.9 MB (10876472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:9241cca9693c0372458ebec46ddb886fc0bffe1b9aeee2c7d4dfc0050b1a55d0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.2 MB (68192296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f44e91617f5732bcc2b11f0aa7d00e23d82a7b4f67e4d5a7787a52433fa706df`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:16:51 GMT
ADD file:132abd62c4fa546798c96d5b1f6f409de9ee27242caf6c479d65309b764c3ece in / 
# Tue, 23 Aug 2022 01:16:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 06:19:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 06:19:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1918e2afd901ca723b3483d8d521789daac45ddbaae2bf9fd813933e826f39b4`  
		Last Modified: Tue, 23 Aug 2022 01:22:10 GMT  
		Size: 52.5 MB (52547848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a58d3f469ed5c6be23bbc74a836bceb306e58e8cd5e58e4464c2b23519543a`  
		Last Modified: Tue, 23 Aug 2022 06:26:58 GMT  
		Size: 5.1 MB (5070690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61379bcded34629fad0582d1d42f2cba36b5f418591509e15301773304e7c7c0`  
		Last Modified: Tue, 23 Aug 2022 06:26:59 GMT  
		Size: 10.6 MB (10573758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:56c33d4b477957b573aed7cc5367f95d01459a2a0a6312c42994c79f488b1cdc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65353658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f92c349465773257e5ffe974e22d6a19ca708f3db946ebf552668157b43ba5c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:42:43 GMT
ADD file:21190c24a038c3c9de64b88797bf00e4c4319bd598c7c465cab2ca88d0502416 in / 
# Tue, 23 Aug 2022 01:42:43 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 12:59:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:00:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c715a126a4d5182c28d2d7b1c81de847bfbbacf6851819fef3eb28e3feb7db0e`  
		Last Modified: Tue, 23 Aug 2022 01:49:30 GMT  
		Size: 50.2 MB (50204931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cecc62e275236714359bda7d1f9c8412e8fa8539f3ef682eebd9c77986c927d`  
		Last Modified: Tue, 23 Aug 2022 13:11:58 GMT  
		Size: 4.9 MB (4930827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818eb872fe75602d611beeac0db63da0a4d8a67aee8b909d5114814f76446a5e`  
		Last Modified: Tue, 23 Aug 2022 13:11:59 GMT  
		Size: 10.2 MB (10217900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:224dfb7f5032a11af8748f4e65daa8f50f478612b91b1c9176a7ef035ed374ba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.3 MB (69292452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93d7443e4194085764e49b9d96d081bc973eba35516e6d88b0058b0854b2970e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:16 GMT
ADD file:ce6014a27d18915dc6d46c5c1f0f894f0027d1e41fbebb1599c16371b7bab2f1 in / 
# Tue, 23 Aug 2022 01:52:18 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:27:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:28:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:cd84405c8b9e7a8c3d580c2148d25120dd697ea61e1cb55a62f33e67988b7043`  
		Last Modified: Tue, 23 Aug 2022 01:57:29 GMT  
		Size: 53.7 MB (53690830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d98e120b809269e56de468d2b91569789c521011e4d9b1806e43fd04462de2`  
		Last Modified: Tue, 23 Aug 2022 02:36:44 GMT  
		Size: 4.9 MB (4944180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb6be5911b40ca548e48c10b09cb2312f1698b4c84f09711c69389a94b1a8be`  
		Last Modified: Tue, 23 Aug 2022 02:36:44 GMT  
		Size: 10.7 MB (10657442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:0d9e01a77b19864476557d06dadfb768771a3b89333dbbf3b7c3fd10138e3fa7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.1 MB (72131190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c00fec5790de3e13e4285b83054a6850bd58812ba11a6858bbfc8607533256b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:24 GMT
ADD file:4012c41187a03bdb3d37bec80f6255a1d46582e3ed145b4f313e42196529e524 in / 
# Tue, 23 Aug 2022 01:02:25 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:31:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:31:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6f683b9c66ef80b527ee5e4cb11969c6e0c1400ab69a4f1279af90f5766d70c7`  
		Last Modified: Tue, 23 Aug 2022 01:07:53 GMT  
		Size: 56.0 MB (56012624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f506948c8aa6d2e0693b583a388ce5e10b4393763bd2ea2529af3bfaa07f0c92`  
		Last Modified: Tue, 23 Aug 2022 01:40:01 GMT  
		Size: 5.1 MB (5085725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915cb3138c0c978b1806934d3f979cff24ecaed321fe7e13caa292cf9ca73dcc`  
		Last Modified: Tue, 23 Aug 2022 01:40:01 GMT  
		Size: 11.0 MB (11032841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:b88de28a9b03c3efa219ebe99731c2dcf063299c1769c16ab9fe8fdacf59ff38
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68852548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15015eb73f5ade0114232ff8e03c9c853246f11dd35a7f95196f6c3eef74d820`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:10:38 GMT
ADD file:a55d19f262e8338f932ce871c1cbc1718f9f74a5002212f38fea74f3858460a9 in / 
# Tue, 23 Aug 2022 00:10:43 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 22:24:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 22:24:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5ce438ccc597187e8a0dab5cc8906e6a0ec75a9320e55225ad2ec24765f7c0b4`  
		Last Modified: Tue, 23 Aug 2022 00:18:51 GMT  
		Size: 53.3 MB (53272999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567ecdfd8aa8d0bdcecff06b6b73dfbde6ae5451a3afec2a33aee7ca527b61e9`  
		Last Modified: Tue, 23 Aug 2022 22:49:03 GMT  
		Size: 4.9 MB (4918268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9374a0689765aeaeee15bb1c011bddd8cb323e6002385ceb42952a14d3210410`  
		Last Modified: Tue, 23 Aug 2022 22:49:06 GMT  
		Size: 10.7 MB (10661281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d8b7e1a18e133da0ea19134be7a76cdd22ec4f10fb6a01976563fcbea1555ce0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.0 MB (75950698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d703a630725af8cf9c5a1f40484ae8fc94e5360d191852caf1164235d16cd71`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:24:30 GMT
ADD file:c498f58d8dc50a2a20679642be8f6f43de8b79455438a1c237ef4c94a9ffe34c in / 
# Tue, 23 Aug 2022 01:24:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:58:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:62d01a7bda469557451a05bab1d4de7f53dd936e8032b36635019fd54cd927e4`  
		Last Modified: Tue, 23 Aug 2022 01:29:57 GMT  
		Size: 58.9 MB (58909173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b002340b938f821f3b0978eb9bfc47d2b8fe91b33c50508bd618c3c4b0ffe0`  
		Last Modified: Tue, 23 Aug 2022 02:10:43 GMT  
		Size: 5.4 MB (5412576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c65f43f4fd248e0fd18c35535f21fcafa740bdde05c5c367f32926f478e55f`  
		Last Modified: Tue, 23 Aug 2022 02:10:44 GMT  
		Size: 11.6 MB (11628949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:8d5fc4782913393f45ddd1ea898bcb30f1bb102bcf7d603315f3a6aaec9ea202
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69191840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a21a8727c9bc59c13f1f4b1072ecef25e905519ec56c0235f3a2d399dbdede69`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:53:42 GMT
ADD file:799d2eac4bf12dcb56eca0b771da879e8873a2a81b4d74520db7d6665d448ff6 in / 
# Tue, 23 Aug 2022 00:53:45 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 09:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 09:51:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6e8428caa8cb9dd5cd48266f588e1d935181b0d75e5f4680a9d4d03700d44289`  
		Last Modified: Tue, 23 Aug 2022 01:01:15 GMT  
		Size: 53.3 MB (53279185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b41fe9abb9a7707d3bfd9881e997384ad70ba3f811c4152a16e11585318bd5`  
		Last Modified: Tue, 23 Aug 2022 09:59:58 GMT  
		Size: 5.1 MB (5146782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0215c1024f20ea76e1b536fcf226d87a639e72806443621a0bf52a719c0218fd`  
		Last Modified: Tue, 23 Aug 2022 09:59:59 GMT  
		Size: 10.8 MB (10765873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:focal`

```console
$ docker pull buildpack-deps@sha256:7e46c886cfb15a4bb8d6c337f664f56a107e337264a74f80d9a1d0835b83dd61
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
$ docker pull buildpack-deps@sha256:236275a19f23e22211c79a72f7606ead785500c53780cff18e7ebff5fffdada5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.7 MB (245735269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c377f7b08c01644a3b2aa6f083ce6d4f1812e8652efbc64a7b9b550dbfb08132`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:23:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:23:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 02:24:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:27:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aceaa9f66a60a3695a6348be449df629aed61f57a9cbd55a388bdcfa40cb27b7`  
		Last Modified: Fri, 02 Sep 2022 02:37:25 GMT  
		Size: 7.7 MB (7747479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d69e69900ca0c9eb8762e001879c1e84e29d94a2397e389440b1d8689445e5`  
		Last Modified: Fri, 02 Sep 2022 02:37:24 GMT  
		Size: 3.6 MB (3624451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:035d79e04aad5acedcb6ebd870819e030f0f1cb534d55136ac5f6087b31b39f9`  
		Last Modified: Fri, 02 Sep 2022 02:37:44 GMT  
		Size: 60.7 MB (60738066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f65cb058b8e19392f740a77af749897af039a43730af19d5b986a7de8cc696`  
		Last Modified: Fri, 02 Sep 2022 02:38:15 GMT  
		Size: 145.1 MB (145052588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:6cc83b90351f8ac0223faa87e392c2a9f24157d4f422e588bb779baa01f1ce55
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.8 MB (211783596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:581bfa0c33a65661c95cc0c51eb8e5cebb681ebbee12360daadc798008c4d1ee`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 06:08:22 GMT
ADD file:685f4b5f8c1f11b6389e9f929909e1a667abf29814a7ccfb859aae287dacd7e1 in / 
# Fri, 02 Sep 2022 06:08:22 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 09:31:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 09:32:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 09:32:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 09:33:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:eff72fca8e1d166ddfda6ac6c409e888c95950da6c47d360a088219c0ad7ba05`  
		Last Modified: Fri, 02 Sep 2022 06:10:16 GMT  
		Size: 24.6 MB (24588743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0063ca7d240c073b50b399efe49028199e2fc1671c3d5e69e566b2b36dea9282`  
		Last Modified: Fri, 02 Sep 2022 09:41:04 GMT  
		Size: 6.7 MB (6741254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93ac5277e93cfbfa1f89a828713b7c6314babc86f222357de3141883f92a010`  
		Last Modified: Fri, 02 Sep 2022 09:41:04 GMT  
		Size: 3.1 MB (3104403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ccea48caa3d4856a1e5a5278dfb92e187166e74c5f4226090de64a520ae1f91`  
		Last Modified: Fri, 02 Sep 2022 09:41:27 GMT  
		Size: 55.4 MB (55442260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715d9c57028ba4ae9a65a2fe21da32b16c0d47fed424958a335b6ff470ec3fad`  
		Last Modified: Fri, 02 Sep 2022 09:41:57 GMT  
		Size: 121.9 MB (121906936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:6e21811ff53feb197c55dbcb5913e6167d2f756d5225790d038f9b9b82b31c3e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.5 MB (235507390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8031960c5c0d2a8ef476a475b524c69ce8e35c58b47617ebd56fe13cdd990406`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:38:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:38:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 04:39:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:40:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6667cb55d48ba4971074c7d8aa09e7b2368fb83f8ab6336c1ae53675ef8a5fdc`  
		Last Modified: Fri, 02 Sep 2022 04:46:48 GMT  
		Size: 7.6 MB (7614784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f84ae37056f7e9d12b5c5d6fbf1924cc86999a56dd4adeff2f422552b9edf08`  
		Last Modified: Fri, 02 Sep 2022 04:46:48 GMT  
		Size: 3.4 MB (3387844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8330d23b3e1d0fb7320e653a9dba9018129a28846b4d6cffdc5caa044ceee0`  
		Last Modified: Fri, 02 Sep 2022 04:47:09 GMT  
		Size: 60.8 MB (60803136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131f3a8b3e4894860eeb15da87fb3843ad69cebaa2ea4bb04c6b16240a96eef2`  
		Last Modified: Fri, 02 Sep 2022 04:47:40 GMT  
		Size: 136.5 MB (136509809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:b864ae13cc2a8ce0ee0d8dee4231935012a1f332f708f5e160d746b0e322b543
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.5 MB (269549986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3829078671a39b677798e7ff15db74a35aa34c521d9cdba344014e925803e15d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:49:54 GMT
ADD file:eb82827919ea73f9595d7b0b70fe9aa5ff23e16ea6a87f7f9ef4e1905857b789 in / 
# Thu, 01 Sep 2022 23:49:56 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:34:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:35:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 03:36:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:39:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:891f6400ce611ee5975f04ad6d2c68305c76a8628b846df1b1f9ac7c45b1311c`  
		Last Modified: Thu, 01 Sep 2022 23:52:11 GMT  
		Size: 33.3 MB (33295624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c38e8344eceb4e722b9d2cc7cf0d2cdca38bb2870c652f545c8ea652efa4f6`  
		Last Modified: Fri, 02 Sep 2022 03:55:42 GMT  
		Size: 8.7 MB (8704791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059cb2841292be0e2908a7c8f78a0db3f136154b78b70a9881535c8c1080dc3f`  
		Last Modified: Fri, 02 Sep 2022 03:55:41 GMT  
		Size: 4.5 MB (4456160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cd324c0fe479474378bdfc00b7027887775d4396a082938a08a2b3f8163431`  
		Last Modified: Fri, 02 Sep 2022 03:56:12 GMT  
		Size: 69.5 MB (69529571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845e0c714d38e7d101ce3585817a73b34d9f7e53c5810c5ad7ecc1f8469f0e7b`  
		Last Modified: Fri, 02 Sep 2022 03:57:03 GMT  
		Size: 153.6 MB (153563840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:0983feadc237a384bc35d020091ffbf6b9eb5b8b312f716e301223786fa27dd4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.4 MB (226432077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c4f4a81fad6a7cffcc865b12be1766a3f2d65338bbd923218ff0906b2232f3`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:13 GMT
ADD file:75a78d9ec31ac5486bdde3e48ebfc534089c5f38f14850243c2ab2e632f0bbe5 in / 
# Fri, 02 Sep 2022 01:03:16 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:03:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:04:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 02:04:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:06:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b87ab7b8bb5c2a1f34d9a2e9887fde669c33cea7428fdb048362dfa81eccaa75`  
		Last Modified: Fri, 02 Sep 2022 01:04:49 GMT  
		Size: 27.0 MB (27045282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f81ff7514526202dbe703eab1c9f1a8c08e2fdc2c2d56b949c8d1f90825e908`  
		Last Modified: Fri, 02 Sep 2022 02:15:30 GMT  
		Size: 7.4 MB (7397526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30cf575bc155da8ebabf970fa2716a48bb3789c6a3967d83d0f7583991658942`  
		Last Modified: Fri, 02 Sep 2022 02:15:30 GMT  
		Size: 3.5 MB (3542655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:423b3fa0fb4a3902e95b623da0004da02d690cf894720b6584469c6c7709e39a`  
		Last Modified: Fri, 02 Sep 2022 02:15:48 GMT  
		Size: 60.0 MB (60008998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4036fb36c2cf3563cffaf474016b239dfaed09f13efbeea14c7f35e3027aecfb`  
		Last Modified: Fri, 02 Sep 2022 02:16:12 GMT  
		Size: 128.4 MB (128437616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:focal-curl`

```console
$ docker pull buildpack-deps@sha256:55c8b92c9d110cd78a6118ad40af433837e827a34ea048aea2d9d9a846963ce2
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
$ docker pull buildpack-deps@sha256:859a87863b458751a541038d05e5569e5f62dc78e39091b7b6225a3ea9745a8d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.9 MB (39944615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71654a9ae5f8958dcaa319be61ebc69326d6eb070e287963d83a169357468b2c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:23:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:23:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aceaa9f66a60a3695a6348be449df629aed61f57a9cbd55a388bdcfa40cb27b7`  
		Last Modified: Fri, 02 Sep 2022 02:37:25 GMT  
		Size: 7.7 MB (7747479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d69e69900ca0c9eb8762e001879c1e84e29d94a2397e389440b1d8689445e5`  
		Last Modified: Fri, 02 Sep 2022 02:37:24 GMT  
		Size: 3.6 MB (3624451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:cdcb31c6c524a3dc5e984ae33da46514f4d8e5e660ca81af01394d1a25532bfa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34434400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaa09c1b604887bf598f7cb6368be01387a6cf9daa76e3e9fbedb8b6f152564c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 06:08:22 GMT
ADD file:685f4b5f8c1f11b6389e9f929909e1a667abf29814a7ccfb859aae287dacd7e1 in / 
# Fri, 02 Sep 2022 06:08:22 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 09:31:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 09:32:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:eff72fca8e1d166ddfda6ac6c409e888c95950da6c47d360a088219c0ad7ba05`  
		Last Modified: Fri, 02 Sep 2022 06:10:16 GMT  
		Size: 24.6 MB (24588743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0063ca7d240c073b50b399efe49028199e2fc1671c3d5e69e566b2b36dea9282`  
		Last Modified: Fri, 02 Sep 2022 09:41:04 GMT  
		Size: 6.7 MB (6741254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93ac5277e93cfbfa1f89a828713b7c6314babc86f222357de3141883f92a010`  
		Last Modified: Fri, 02 Sep 2022 09:41:04 GMT  
		Size: 3.1 MB (3104403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7a621cd38afcf8f3d75a8f8dcd631038d460ca67c752870dc041e60595956163
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38194445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84b6a55990e1096425a70e6b907d1ba30b69bbd3131c15a11f2c662b8fe06677`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:38:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:38:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6667cb55d48ba4971074c7d8aa09e7b2368fb83f8ab6336c1ae53675ef8a5fdc`  
		Last Modified: Fri, 02 Sep 2022 04:46:48 GMT  
		Size: 7.6 MB (7614784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f84ae37056f7e9d12b5c5d6fbf1924cc86999a56dd4adeff2f422552b9edf08`  
		Last Modified: Fri, 02 Sep 2022 04:46:48 GMT  
		Size: 3.4 MB (3387844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d47e1f12d9061d2873d9c60f1a8994a2c6caad46a876f0770ecf8e0e76d2f6c9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46456575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:046ee271c995217b16c2b683d8ebb2fd39ceafee110313d8835f9d7e5a71539f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:49:54 GMT
ADD file:eb82827919ea73f9595d7b0b70fe9aa5ff23e16ea6a87f7f9ef4e1905857b789 in / 
# Thu, 01 Sep 2022 23:49:56 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:34:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:35:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:891f6400ce611ee5975f04ad6d2c68305c76a8628b846df1b1f9ac7c45b1311c`  
		Last Modified: Thu, 01 Sep 2022 23:52:11 GMT  
		Size: 33.3 MB (33295624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c38e8344eceb4e722b9d2cc7cf0d2cdca38bb2870c652f545c8ea652efa4f6`  
		Last Modified: Fri, 02 Sep 2022 03:55:42 GMT  
		Size: 8.7 MB (8704791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059cb2841292be0e2908a7c8f78a0db3f136154b78b70a9881535c8c1080dc3f`  
		Last Modified: Fri, 02 Sep 2022 03:55:41 GMT  
		Size: 4.5 MB (4456160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:ab0b4e710273e638ba716aedb8a727f3b67f94ddaa5ad6f5a9d494cf30423b20
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34132358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bbe2f4f13bcb67f1b8b3ba8c4b939fab6dd3106951388314174f8343a01c67f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:09:50 GMT
ADD file:3f3a2d77633db008f6d929f63880dab6bd20eab1e346e715331cc1b32a9d9821 in / 
# Fri, 02 Sep 2022 00:09:51 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 00:59:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 01:00:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6cbb7395a087ad86b87360ff9e4682ac013d19b01b368e0d658aa360440c9e0f`  
		Last Modified: Fri, 02 Sep 2022 00:26:57 GMT  
		Size: 24.2 MB (24243281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da12dcd490d59114c83ba58a7ebb7af8cd20209af19b95285772857279ba9bb3`  
		Last Modified: Fri, 02 Sep 2022 01:48:06 GMT  
		Size: 6.7 MB (6744222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33395e6e037105cb40bc74d80f9d435cd4770ecc1fbeedd173dd4422aaacc2ee`  
		Last Modified: Fri, 02 Sep 2022 01:48:00 GMT  
		Size: 3.1 MB (3144855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:60896cc7f8a1ca84de78ac668cbd48eae132398b8df15d631a211d02450910a6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (37985463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97f45ed43266896cb111d1ed39d77f6d9b84486fac419d2a02bc39d1cd023139`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:13 GMT
ADD file:75a78d9ec31ac5486bdde3e48ebfc534089c5f38f14850243c2ab2e632f0bbe5 in / 
# Fri, 02 Sep 2022 01:03:16 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:03:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:04:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b87ab7b8bb5c2a1f34d9a2e9887fde669c33cea7428fdb048362dfa81eccaa75`  
		Last Modified: Fri, 02 Sep 2022 01:04:49 GMT  
		Size: 27.0 MB (27045282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f81ff7514526202dbe703eab1c9f1a8c08e2fdc2c2d56b949c8d1f90825e908`  
		Last Modified: Fri, 02 Sep 2022 02:15:30 GMT  
		Size: 7.4 MB (7397526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30cf575bc155da8ebabf970fa2716a48bb3789c6a3967d83d0f7583991658942`  
		Last Modified: Fri, 02 Sep 2022 02:15:30 GMT  
		Size: 3.5 MB (3542655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:focal-scm`

```console
$ docker pull buildpack-deps@sha256:7d9bca39517f49994f28884f7b6b3efbde43df5f81d2c79e3397a858a3e137dd
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
$ docker pull buildpack-deps@sha256:cb3b6e80127a63f7e26f56e3796f245ca5a27f11bacd3a78710dd97a7b41f913
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.7 MB (100682681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcc3de2b9eab267855272f14c781d6e663b027167aec279a939c60d01e405d03`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:23:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:23:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 02:24:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aceaa9f66a60a3695a6348be449df629aed61f57a9cbd55a388bdcfa40cb27b7`  
		Last Modified: Fri, 02 Sep 2022 02:37:25 GMT  
		Size: 7.7 MB (7747479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d69e69900ca0c9eb8762e001879c1e84e29d94a2397e389440b1d8689445e5`  
		Last Modified: Fri, 02 Sep 2022 02:37:24 GMT  
		Size: 3.6 MB (3624451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:035d79e04aad5acedcb6ebd870819e030f0f1cb534d55136ac5f6087b31b39f9`  
		Last Modified: Fri, 02 Sep 2022 02:37:44 GMT  
		Size: 60.7 MB (60738066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:5d5e9c111f46caa080bcb19313e1cfe81cfd742fd3e87fec58d352eb998c0d15
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.9 MB (89876660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21de531d01800e4c366ef96d96e2348db60ea1e047073558e5ceaec1bf8d531c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 06:08:22 GMT
ADD file:685f4b5f8c1f11b6389e9f929909e1a667abf29814a7ccfb859aae287dacd7e1 in / 
# Fri, 02 Sep 2022 06:08:22 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 09:31:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 09:32:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 09:32:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:eff72fca8e1d166ddfda6ac6c409e888c95950da6c47d360a088219c0ad7ba05`  
		Last Modified: Fri, 02 Sep 2022 06:10:16 GMT  
		Size: 24.6 MB (24588743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0063ca7d240c073b50b399efe49028199e2fc1671c3d5e69e566b2b36dea9282`  
		Last Modified: Fri, 02 Sep 2022 09:41:04 GMT  
		Size: 6.7 MB (6741254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93ac5277e93cfbfa1f89a828713b7c6314babc86f222357de3141883f92a010`  
		Last Modified: Fri, 02 Sep 2022 09:41:04 GMT  
		Size: 3.1 MB (3104403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ccea48caa3d4856a1e5a5278dfb92e187166e74c5f4226090de64a520ae1f91`  
		Last Modified: Fri, 02 Sep 2022 09:41:27 GMT  
		Size: 55.4 MB (55442260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7a3530d9a72f8520c05cbf988f91c39234580a6c4d96b32ac4d7f8b80a0bafa3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.0 MB (98997581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce2158f16d69616965d544733bd68e5d2ebc2a66c7085ecbded592b9a3749fd9`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:38:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:38:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 04:39:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6667cb55d48ba4971074c7d8aa09e7b2368fb83f8ab6336c1ae53675ef8a5fdc`  
		Last Modified: Fri, 02 Sep 2022 04:46:48 GMT  
		Size: 7.6 MB (7614784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f84ae37056f7e9d12b5c5d6fbf1924cc86999a56dd4adeff2f422552b9edf08`  
		Last Modified: Fri, 02 Sep 2022 04:46:48 GMT  
		Size: 3.4 MB (3387844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8330d23b3e1d0fb7320e653a9dba9018129a28846b4d6cffdc5caa044ceee0`  
		Last Modified: Fri, 02 Sep 2022 04:47:09 GMT  
		Size: 60.8 MB (60803136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:052898d9b635e422c93fc45a17b62462438b35cfdc07758cd359a5bbed03b19c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (115986146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f181b52cc6edd4eede5610b8576eef3449ccc0e871ad1cdb3e3afd78baf6238`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:49:54 GMT
ADD file:eb82827919ea73f9595d7b0b70fe9aa5ff23e16ea6a87f7f9ef4e1905857b789 in / 
# Thu, 01 Sep 2022 23:49:56 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:34:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:35:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 03:36:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:891f6400ce611ee5975f04ad6d2c68305c76a8628b846df1b1f9ac7c45b1311c`  
		Last Modified: Thu, 01 Sep 2022 23:52:11 GMT  
		Size: 33.3 MB (33295624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c38e8344eceb4e722b9d2cc7cf0d2cdca38bb2870c652f545c8ea652efa4f6`  
		Last Modified: Fri, 02 Sep 2022 03:55:42 GMT  
		Size: 8.7 MB (8704791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059cb2841292be0e2908a7c8f78a0db3f136154b78b70a9881535c8c1080dc3f`  
		Last Modified: Fri, 02 Sep 2022 03:55:41 GMT  
		Size: 4.5 MB (4456160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cd324c0fe479474378bdfc00b7027887775d4396a082938a08a2b3f8163431`  
		Last Modified: Fri, 02 Sep 2022 03:56:12 GMT  
		Size: 69.5 MB (69529571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:e73ed015c1915a4a11fb634719de2f5a4f726ae247375b547314696890939979
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.0 MB (97994461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9ccb9a779d53a17e14d373934b36f3ad284f67126d248adf42298fb815e0610`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:13 GMT
ADD file:75a78d9ec31ac5486bdde3e48ebfc534089c5f38f14850243c2ab2e632f0bbe5 in / 
# Fri, 02 Sep 2022 01:03:16 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:03:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:04:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 02:04:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b87ab7b8bb5c2a1f34d9a2e9887fde669c33cea7428fdb048362dfa81eccaa75`  
		Last Modified: Fri, 02 Sep 2022 01:04:49 GMT  
		Size: 27.0 MB (27045282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f81ff7514526202dbe703eab1c9f1a8c08e2fdc2c2d56b949c8d1f90825e908`  
		Last Modified: Fri, 02 Sep 2022 02:15:30 GMT  
		Size: 7.4 MB (7397526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30cf575bc155da8ebabf970fa2716a48bb3789c6a3967d83d0f7583991658942`  
		Last Modified: Fri, 02 Sep 2022 02:15:30 GMT  
		Size: 3.5 MB (3542655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:423b3fa0fb4a3902e95b623da0004da02d690cf894720b6584469c6c7709e39a`  
		Last Modified: Fri, 02 Sep 2022 02:15:48 GMT  
		Size: 60.0 MB (60008998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:jammy`

```console
$ docker pull buildpack-deps@sha256:f5f73722f168030ecf95375fb039e764f70a8766f4ffea76682aa2741c9abbe9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:jammy` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:5ea27ebb2fabdd092d8cb56379f17e558c323730e82c5f47e472d369221608ec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.0 MB (249957836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24b6b43211e8cb703aecf97a92e81db48963dcee1b9fb2ef3692bf22762eeb6c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:27:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:28:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 02:28:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:31:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:728cfcfa2f7739d87ae3efda60d01680593fcb2b55fdb5840721012c19335b9a`  
		Last Modified: Fri, 02 Sep 2022 02:38:25 GMT  
		Size: 3.8 MB (3804276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09eda6154af3733cdc766a287039ebbd0d78265b3a7c64ed165045c8849ba1ce`  
		Last Modified: Fri, 02 Sep 2022 02:38:25 GMT  
		Size: 3.6 MB (3560674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a6e6f57df0f885a7603852f5ee2e183c2961cb80d1785032449ad7a31e61ffe`  
		Last Modified: Fri, 02 Sep 2022 02:38:40 GMT  
		Size: 39.3 MB (39338193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69cee3392ebf3b497e43558b59aa5f76c60fc10b2eaf5409de9a941f6dd42ca`  
		Last Modified: Fri, 02 Sep 2022 02:39:13 GMT  
		Size: 172.8 MB (172827987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:87ee84eb8872003687e4599ccc21153aa24f6b8a8558e31b825ab923a5b0fbbb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.6 MB (216605721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a70dc2d9a61ffa7c73f46bd7f5fc0351a4b4582af1b71a777935419f36329ed`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 06:08:32 GMT
ADD file:8b109e7521f26505639a07128de43f93636fcc05ecf26c6358f893f22df38acd in / 
# Fri, 02 Sep 2022 06:08:32 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 09:33:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 09:34:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 09:34:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 09:35:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:af25ea170fdc3ef953710312fcb7b9706eae0149cf05cd81c8281f1c511208bb`  
		Last Modified: Fri, 02 Sep 2022 06:10:34 GMT  
		Size: 27.0 MB (27016783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9398b18a454e124e1f9b5c08d3b8e75027704cf5d81734f403a4852babda0c9e`  
		Last Modified: Fri, 02 Sep 2022 09:42:10 GMT  
		Size: 3.6 MB (3556228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19d83ea0962e81d21c528b9d3bcf4646473a26fe96198cbc633813df2ce7583`  
		Last Modified: Fri, 02 Sep 2022 09:42:09 GMT  
		Size: 3.7 MB (3713683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:456bac4459d3361e1c563bc2e25e0a8f45ce5407f38a18250e9f40e4286be0f2`  
		Last Modified: Fri, 02 Sep 2022 09:42:29 GMT  
		Size: 41.9 MB (41906676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d843b879ac3e2cefa8c53e242aed65d5707151f67433a317e8f836519a2625`  
		Last Modified: Fri, 02 Sep 2022 09:43:01 GMT  
		Size: 140.4 MB (140412351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:419bb1f78244b8b824e28585007ee5603f88acdc520bae8aa8cfbb0869decf02
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.8 MB (240781696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44bca26c57eec16b1355ce87898fd1e703eac1d052e182d9b44a2ef861fe8fa0`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:40:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:40:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 04:41:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:41:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a5013832a9b04a455a3aed1888a43489d8850d9810b8d8fb64744bf814a1d9d`  
		Last Modified: Fri, 02 Sep 2022 04:47:52 GMT  
		Size: 3.8 MB (3776579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00e6a48d7146e6e81a25ce023cb7fb060f7cc202d4d5a9da4bc632e5ac4e05e`  
		Last Modified: Fri, 02 Sep 2022 04:47:52 GMT  
		Size: 3.3 MB (3320662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb48a8c04a0b3dd9a3bfc932ba13906c14770d53cf3bec49dca7acf27f47e0e`  
		Last Modified: Fri, 02 Sep 2022 04:48:09 GMT  
		Size: 39.2 MB (39242094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd94762a4fff6f6574e2054c323e06d6605fc3b0ac948910a65ca6f4b2c16a6e`  
		Last Modified: Fri, 02 Sep 2022 04:48:43 GMT  
		Size: 166.1 MB (166061021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:4c0eb3540a84187cfb3276069e433ed35064a1ed0fc241449621d528a813847b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.8 MB (271782797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9c1de0666ea737305d554a340f11a9c475745fa6e7a42cb195f6bb15c837b57`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:50:09 GMT
ADD file:39b6fa94f6e1300a6fc4b6094e8250c22ecaa6e7c9f934841765d45b919402c5 in / 
# Thu, 01 Sep 2022 23:50:11 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:40:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:40:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 03:41:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:45:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9ef77d5e46df05bf9f34e5871097fd038295a2aa5e29f1806ac3a96aa2545b5f`  
		Last Modified: Thu, 01 Sep 2022 23:52:34 GMT  
		Size: 35.7 MB (35721187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47f3136401182e4158ce50b7b80ede159c628447df84c97f8d16a1fdef5ca73f`  
		Last Modified: Fri, 02 Sep 2022 03:57:16 GMT  
		Size: 4.3 MB (4276033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed57522d1a954e636dbd623f4d22053a0339d16dbc9ce851739f5318e9fd3ad`  
		Last Modified: Fri, 02 Sep 2022 03:57:16 GMT  
		Size: 4.2 MB (4233890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70892ee50c4d77a318fa001df485f8ea6208582b0aa6835eb223cd0c249d1e05`  
		Last Modified: Fri, 02 Sep 2022 03:57:39 GMT  
		Size: 43.8 MB (43760153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:885ac7b7aa4ea854597160aa477647cfd9dbdcc9c5121b1bf62bb68af66ab142`  
		Last Modified: Fri, 02 Sep 2022 03:58:35 GMT  
		Size: 183.8 MB (183791534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:a3a808d8c587c5bfa6527b3fd76f9931de150a4a5b913a182f85b77df7f610a5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.9 MB (274912769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8375021379599486ff37858cacbc9dbcbecea3af36a87f33f667a9c6c26418e3`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:11:51 GMT
ADD file:8cff03722326c5e90e26ae259bde7ddd223c466edfd0d1cd6335b7b550f8156c in / 
# Fri, 02 Sep 2022 00:11:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 01:02:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 01:03:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 01:07:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 01:13:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f04a8971a8d913388890f40190f4d3935404b38efd860b235cf5d4de20959061`  
		Last Modified: Fri, 02 Sep 2022 00:29:20 GMT  
		Size: 27.7 MB (27744005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c893dcd3d9a55418817428155b89e044a2ebfddfa13d6945d70f0e2830099015`  
		Last Modified: Fri, 02 Sep 2022 01:49:29 GMT  
		Size: 3.6 MB (3615909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8351e367bac61d27e9f493ab2fdd756510203f5c595c3c81d6b96d2ac3214ca`  
		Last Modified: Fri, 02 Sep 2022 01:49:27 GMT  
		Size: 3.8 MB (3778105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78cf99d2fae932ddb826d79cfc1fb3069f811bbf8ec7c13a8c03db4b519f566e`  
		Last Modified: Fri, 02 Sep 2022 01:51:48 GMT  
		Size: 42.1 MB (42110525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643cf35c08de9ab511d3bbe352a3dfc7a6c22bb4b6d9c5ae72acd28c346d4599`  
		Last Modified: Fri, 02 Sep 2022 01:58:56 GMT  
		Size: 197.7 MB (197664225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:fb22e95706a5a0e12f4a5df9d0b4f43e090e63050a62cd6b2f81d9d13cb999db
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.7 MB (223654390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af9e578eb33342a177899cd08037bc3c789443a018966b250d40eb3eb60cc51d`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:25 GMT
ADD file:aabc057fd7b1b1f9b4b729222b6dc90e98f846a65bfee1ee57cc899b6cee5a10 in / 
# Fri, 02 Sep 2022 01:03:28 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:06:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:07:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 02:07:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:09:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a32e6a15a6635185097921b9d08997d505b6b6500b6c142ad8e718d87c45ffad`  
		Last Modified: Fri, 02 Sep 2022 01:05:01 GMT  
		Size: 28.6 MB (28643161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba21c1eef45ab363d5dcc84511ca01cdbbe1e6dfdf54dcd8b108e256251e6e5`  
		Last Modified: Fri, 02 Sep 2022 02:16:20 GMT  
		Size: 3.8 MB (3809432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b26595dd670dde31a9dd83588e0dd3408a0d7f51791314f04652f5117a00332`  
		Last Modified: Fri, 02 Sep 2022 02:16:20 GMT  
		Size: 3.5 MB (3471859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b7719a0d5c7493ffa972e138dfd13f216a4e6bbde7a2e90e46cc1d8e2f365f7`  
		Last Modified: Fri, 02 Sep 2022 02:16:32 GMT  
		Size: 39.3 MB (39294502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f983860f6aa64e4e4ad14f4559ce0d12f350ba744092c39c776c39410f60fd`  
		Last Modified: Fri, 02 Sep 2022 02:16:57 GMT  
		Size: 148.4 MB (148435436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:jammy-curl`

```console
$ docker pull buildpack-deps@sha256:5172cc3839a41474139e50c1d84e15439b41fb3eff707528a28d47ba64f40f73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:jammy-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:8b8f7edeac757b1a514d89c5f6e4082b9f64b1aeb87eeaa31da58dbe9e424ff6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37791656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32d70c81850c25c6f5bf209fbcc9e0b2732e5456ebcaf907d4a139b4e73eb4e7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:27:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:28:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:728cfcfa2f7739d87ae3efda60d01680593fcb2b55fdb5840721012c19335b9a`  
		Last Modified: Fri, 02 Sep 2022 02:38:25 GMT  
		Size: 3.8 MB (3804276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09eda6154af3733cdc766a287039ebbd0d78265b3a7c64ed165045c8849ba1ce`  
		Last Modified: Fri, 02 Sep 2022 02:38:25 GMT  
		Size: 3.6 MB (3560674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:4d5dd081b0038052e395515e2ca6703d1e57c62554368d3d2cb63687fab789ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34286694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca6129cb72bf260d31e0bf82e24d1444ba54d6a83c741657ebeb73c543f11b6c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 06:08:32 GMT
ADD file:8b109e7521f26505639a07128de43f93636fcc05ecf26c6358f893f22df38acd in / 
# Fri, 02 Sep 2022 06:08:32 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 09:33:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 09:34:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:af25ea170fdc3ef953710312fcb7b9706eae0149cf05cd81c8281f1c511208bb`  
		Last Modified: Fri, 02 Sep 2022 06:10:34 GMT  
		Size: 27.0 MB (27016783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9398b18a454e124e1f9b5c08d3b8e75027704cf5d81734f403a4852babda0c9e`  
		Last Modified: Fri, 02 Sep 2022 09:42:10 GMT  
		Size: 3.6 MB (3556228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19d83ea0962e81d21c528b9d3bcf4646473a26fe96198cbc633813df2ce7583`  
		Last Modified: Fri, 02 Sep 2022 09:42:09 GMT  
		Size: 3.7 MB (3713683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:0178fb33c3d226148c4bf4c01d1d7af7995549d4263e44af2da6673ef6604412
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 MB (35478581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9ee4edf34b38bd4fb5d9c8d2833b2f34145eb1ba7fe01817cc0ea98024a9ce7`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:40:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:40:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a5013832a9b04a455a3aed1888a43489d8850d9810b8d8fb64744bf814a1d9d`  
		Last Modified: Fri, 02 Sep 2022 04:47:52 GMT  
		Size: 3.8 MB (3776579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00e6a48d7146e6e81a25ce023cb7fb060f7cc202d4d5a9da4bc632e5ac4e05e`  
		Last Modified: Fri, 02 Sep 2022 04:47:52 GMT  
		Size: 3.3 MB (3320662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:2d7d4ecc910fbb54f4d2d117583d3eaa890cab38b915d426f8af153408db23c8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44231110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e89808adffacf39aa02aa62ead292356f796d3ac914b396422ee1ddad9b1c31e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:50:09 GMT
ADD file:39b6fa94f6e1300a6fc4b6094e8250c22ecaa6e7c9f934841765d45b919402c5 in / 
# Thu, 01 Sep 2022 23:50:11 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:40:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:40:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9ef77d5e46df05bf9f34e5871097fd038295a2aa5e29f1806ac3a96aa2545b5f`  
		Last Modified: Thu, 01 Sep 2022 23:52:34 GMT  
		Size: 35.7 MB (35721187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47f3136401182e4158ce50b7b80ede159c628447df84c97f8d16a1fdef5ca73f`  
		Last Modified: Fri, 02 Sep 2022 03:57:16 GMT  
		Size: 4.3 MB (4276033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed57522d1a954e636dbd623f4d22053a0339d16dbc9ce851739f5318e9fd3ad`  
		Last Modified: Fri, 02 Sep 2022 03:57:16 GMT  
		Size: 4.2 MB (4233890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:37a6e4bfff70a1d2f2343ec0bc7c5b663942e36f797247df635b8586266c5ce8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35138019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:243eb39738059da136ec1fc770b105776ec3d66b623f2e08cb79cfb2b16709fc`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:11:51 GMT
ADD file:8cff03722326c5e90e26ae259bde7ddd223c466edfd0d1cd6335b7b550f8156c in / 
# Fri, 02 Sep 2022 00:11:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 01:02:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 01:03:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f04a8971a8d913388890f40190f4d3935404b38efd860b235cf5d4de20959061`  
		Last Modified: Fri, 02 Sep 2022 00:29:20 GMT  
		Size: 27.7 MB (27744005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c893dcd3d9a55418817428155b89e044a2ebfddfa13d6945d70f0e2830099015`  
		Last Modified: Fri, 02 Sep 2022 01:49:29 GMT  
		Size: 3.6 MB (3615909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8351e367bac61d27e9f493ab2fdd756510203f5c595c3c81d6b96d2ac3214ca`  
		Last Modified: Fri, 02 Sep 2022 01:49:27 GMT  
		Size: 3.8 MB (3778105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:6a7bc5b2496502a65bad30f7cb0b243ced4eed84af1897e94b98cbc971af9aa6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35924452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59742e1d75395c6a6342d0534baf73e19ecec72302e69af41dbd4cf5ac64fe0c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:25 GMT
ADD file:aabc057fd7b1b1f9b4b729222b6dc90e98f846a65bfee1ee57cc899b6cee5a10 in / 
# Fri, 02 Sep 2022 01:03:28 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:06:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:07:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a32e6a15a6635185097921b9d08997d505b6b6500b6c142ad8e718d87c45ffad`  
		Last Modified: Fri, 02 Sep 2022 01:05:01 GMT  
		Size: 28.6 MB (28643161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba21c1eef45ab363d5dcc84511ca01cdbbe1e6dfdf54dcd8b108e256251e6e5`  
		Last Modified: Fri, 02 Sep 2022 02:16:20 GMT  
		Size: 3.8 MB (3809432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b26595dd670dde31a9dd83588e0dd3408a0d7f51791314f04652f5117a00332`  
		Last Modified: Fri, 02 Sep 2022 02:16:20 GMT  
		Size: 3.5 MB (3471859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:jammy-scm`

```console
$ docker pull buildpack-deps@sha256:a284bfd63ad1a58b6343d35d413e96afa505de655ec6837c303aa63ec23aea19
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:jammy-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:69a05e44c60e1a1002f2d9699f0418c640a3eadc89dcdfc9dbe87db7e7d87887
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77129849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bdf3fac9b188e20ef79a7c6f6472d57ed6eaca4b923b16dfef3262552e212d7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:27:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:28:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 02:28:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:728cfcfa2f7739d87ae3efda60d01680593fcb2b55fdb5840721012c19335b9a`  
		Last Modified: Fri, 02 Sep 2022 02:38:25 GMT  
		Size: 3.8 MB (3804276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09eda6154af3733cdc766a287039ebbd0d78265b3a7c64ed165045c8849ba1ce`  
		Last Modified: Fri, 02 Sep 2022 02:38:25 GMT  
		Size: 3.6 MB (3560674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a6e6f57df0f885a7603852f5ee2e183c2961cb80d1785032449ad7a31e61ffe`  
		Last Modified: Fri, 02 Sep 2022 02:38:40 GMT  
		Size: 39.3 MB (39338193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ce48e296266e7664e9555cd5e4797f8677173754ff8dc85cb3a78618d2569708
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76193370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed4f0c06115901299dd49788abb1b9d4e03e89e614c54efd1bf59111e763ef4a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 06:08:32 GMT
ADD file:8b109e7521f26505639a07128de43f93636fcc05ecf26c6358f893f22df38acd in / 
# Fri, 02 Sep 2022 06:08:32 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 09:33:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 09:34:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 09:34:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:af25ea170fdc3ef953710312fcb7b9706eae0149cf05cd81c8281f1c511208bb`  
		Last Modified: Fri, 02 Sep 2022 06:10:34 GMT  
		Size: 27.0 MB (27016783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9398b18a454e124e1f9b5c08d3b8e75027704cf5d81734f403a4852babda0c9e`  
		Last Modified: Fri, 02 Sep 2022 09:42:10 GMT  
		Size: 3.6 MB (3556228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19d83ea0962e81d21c528b9d3bcf4646473a26fe96198cbc633813df2ce7583`  
		Last Modified: Fri, 02 Sep 2022 09:42:09 GMT  
		Size: 3.7 MB (3713683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:456bac4459d3361e1c563bc2e25e0a8f45ce5407f38a18250e9f40e4286be0f2`  
		Last Modified: Fri, 02 Sep 2022 09:42:29 GMT  
		Size: 41.9 MB (41906676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d2a8efb0e4b21c797f51f9d1ba87902b30e30da3360c017a1666d57d2d1309e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74720675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e4a856aa72ace5cd4c58b5b1cd23888c188dc519c8a3c7bb22796e9060f64b6`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:40:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:40:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 04:41:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a5013832a9b04a455a3aed1888a43489d8850d9810b8d8fb64744bf814a1d9d`  
		Last Modified: Fri, 02 Sep 2022 04:47:52 GMT  
		Size: 3.8 MB (3776579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00e6a48d7146e6e81a25ce023cb7fb060f7cc202d4d5a9da4bc632e5ac4e05e`  
		Last Modified: Fri, 02 Sep 2022 04:47:52 GMT  
		Size: 3.3 MB (3320662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb48a8c04a0b3dd9a3bfc932ba13906c14770d53cf3bec49dca7acf27f47e0e`  
		Last Modified: Fri, 02 Sep 2022 04:48:09 GMT  
		Size: 39.2 MB (39242094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:90e3ff6758a960df5271c39810f50ae7a9af8eb2dfbf402f8a895492fd8072f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.0 MB (87991263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd0871440d7a589078f05df8c44937110743203650e4920096ea0ad39d797173`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:50:09 GMT
ADD file:39b6fa94f6e1300a6fc4b6094e8250c22ecaa6e7c9f934841765d45b919402c5 in / 
# Thu, 01 Sep 2022 23:50:11 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:40:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:40:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 03:41:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9ef77d5e46df05bf9f34e5871097fd038295a2aa5e29f1806ac3a96aa2545b5f`  
		Last Modified: Thu, 01 Sep 2022 23:52:34 GMT  
		Size: 35.7 MB (35721187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47f3136401182e4158ce50b7b80ede159c628447df84c97f8d16a1fdef5ca73f`  
		Last Modified: Fri, 02 Sep 2022 03:57:16 GMT  
		Size: 4.3 MB (4276033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed57522d1a954e636dbd623f4d22053a0339d16dbc9ce851739f5318e9fd3ad`  
		Last Modified: Fri, 02 Sep 2022 03:57:16 GMT  
		Size: 4.2 MB (4233890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70892ee50c4d77a318fa001df485f8ea6208582b0aa6835eb223cd0c249d1e05`  
		Last Modified: Fri, 02 Sep 2022 03:57:39 GMT  
		Size: 43.8 MB (43760153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:5d6c843563e30ae575ac4d38b69a11a921fd690206c62ea029269dba3ca3e7d4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77248544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea8ba9156cd9a9c213f1980abf846f422f40340024a3bb644dd0e1debb94b15c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:11:51 GMT
ADD file:8cff03722326c5e90e26ae259bde7ddd223c466edfd0d1cd6335b7b550f8156c in / 
# Fri, 02 Sep 2022 00:11:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 01:02:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 01:03:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 01:07:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f04a8971a8d913388890f40190f4d3935404b38efd860b235cf5d4de20959061`  
		Last Modified: Fri, 02 Sep 2022 00:29:20 GMT  
		Size: 27.7 MB (27744005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c893dcd3d9a55418817428155b89e044a2ebfddfa13d6945d70f0e2830099015`  
		Last Modified: Fri, 02 Sep 2022 01:49:29 GMT  
		Size: 3.6 MB (3615909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8351e367bac61d27e9f493ab2fdd756510203f5c595c3c81d6b96d2ac3214ca`  
		Last Modified: Fri, 02 Sep 2022 01:49:27 GMT  
		Size: 3.8 MB (3778105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78cf99d2fae932ddb826d79cfc1fb3069f811bbf8ec7c13a8c03db4b519f566e`  
		Last Modified: Fri, 02 Sep 2022 01:51:48 GMT  
		Size: 42.1 MB (42110525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b86d03271a7cf19de9a84a6331f9ad93633a9735a1257e88ed26383a7186520f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75218954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2c746b8e411285ae4bd0c49dac958a98fba1bf3ae25edfb828548488cb80e59`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:25 GMT
ADD file:aabc057fd7b1b1f9b4b729222b6dc90e98f846a65bfee1ee57cc899b6cee5a10 in / 
# Fri, 02 Sep 2022 01:03:28 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:06:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:07:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 02:07:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a32e6a15a6635185097921b9d08997d505b6b6500b6c142ad8e718d87c45ffad`  
		Last Modified: Fri, 02 Sep 2022 01:05:01 GMT  
		Size: 28.6 MB (28643161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba21c1eef45ab363d5dcc84511ca01cdbbe1e6dfdf54dcd8b108e256251e6e5`  
		Last Modified: Fri, 02 Sep 2022 02:16:20 GMT  
		Size: 3.8 MB (3809432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b26595dd670dde31a9dd83588e0dd3408a0d7f51791314f04652f5117a00332`  
		Last Modified: Fri, 02 Sep 2022 02:16:20 GMT  
		Size: 3.5 MB (3471859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b7719a0d5c7493ffa972e138dfd13f216a4e6bbde7a2e90e46cc1d8e2f365f7`  
		Last Modified: Fri, 02 Sep 2022 02:16:32 GMT  
		Size: 39.3 MB (39294502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:kinetic`

```console
$ docker pull buildpack-deps@sha256:c24817e44bda6ad8cc19783d2b65814fce5afa3a1b83857359d0e0d22c849e6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:kinetic` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:3c95ad74f79e8e0d742dbf0b70cabffb0135dfa4a377b9191bc38aa416ba6e48
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.4 MB (259350660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d6d2926c4684f01fa0103bb24bdb1b2a93bec0dca4b41885fc0ca5e11f05fd3`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:43 GMT
ADD file:d5de90ac61ee7027aa0900efb669efa73f611463cf73ab2cfdacadf5ab9fee19 in / 
# Thu, 01 Sep 2022 23:46:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:32:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:32:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 02:32:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:35:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0b78030514e08aad79cb596ba84b18b9579e90eac0b8e0c2dec483c3da8dbee8`  
		Last Modified: Thu, 01 Sep 2022 23:48:15 GMT  
		Size: 27.4 MB (27428015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71363ea1301988ddf4ef6039b34a05a19b44a70e1ba2764e95fa0f47b3585c12`  
		Last Modified: Fri, 02 Sep 2022 02:39:23 GMT  
		Size: 6.8 MB (6779788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d261ea038a7743d40031459e01e57001571ca5986a617d9e2d3174c66d98187a`  
		Last Modified: Fri, 02 Sep 2022 02:39:23 GMT  
		Size: 3.6 MB (3633660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dee5c450c1549fab83f54e9138820f82132ebf0b50a52e7ffb97b6074e98c1b`  
		Last Modified: Fri, 02 Sep 2022 02:39:39 GMT  
		Size: 39.7 MB (39729510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf8f5804b753a7685df0f765050b72cb63d67092265ce7d2dacd3391cfa09ace`  
		Last Modified: Fri, 02 Sep 2022 02:40:13 GMT  
		Size: 181.8 MB (181779687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f6c70d3da9e107526ed57d9da0674e7e3bdcd2c3656609d1763abad413898dd8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.3 MB (222315041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76db4726c51f452cfcf90471617a6293cfa2ed57469fa660aa52c3fad7b47eca`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 06:08:44 GMT
ADD file:6fea481ddc80754c10680e7c291055af82ef815eb0fdaf745c49c4f4cdf2afa1 in / 
# Fri, 02 Sep 2022 06:08:44 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 09:35:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 09:35:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 09:36:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 09:36:59 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1f63be4c3b8fca43746377bd8a99dd9b04acdd942d8464feaae1671e6363d920`  
		Last Modified: Fri, 02 Sep 2022 06:10:58 GMT  
		Size: 25.8 MB (25845683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c94aedbe9250aab4e90e8e88c1f2af520548789812f567b90a81f67dc9145e`  
		Last Modified: Fri, 02 Sep 2022 09:43:15 GMT  
		Size: 5.9 MB (5948408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78166495a53038ebe64fd164f5d7e26607173735e8a0e096424b99f947d93cb`  
		Last Modified: Fri, 02 Sep 2022 09:43:14 GMT  
		Size: 3.8 MB (3801422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28471ad57cdb7e9e4d1bd803eae0208867737111fd76d4143f4b6120903361b7`  
		Last Modified: Fri, 02 Sep 2022 09:43:34 GMT  
		Size: 42.6 MB (42593085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd81b6de6e71e74e98034d486ef79416eeab04372473695ef4a57a2dc8dab6b4`  
		Last Modified: Fri, 02 Sep 2022 09:44:07 GMT  
		Size: 144.1 MB (144126443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:bcffca5d2875c3c5e9e2ebbae1682df46d1a2202cc72f8d63670b9e3d68e3503
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.8 MB (246828390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c63411acefb29eac5a58855779b5ce4e65910ca3242fa4cd116d30e28860fa8`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:58:02 GMT
ADD file:1b9e898b22915c14e3d83959e989e2a653148ff82c8e2a1b3dfa8035256219aa in / 
# Fri, 02 Sep 2022 00:58:02 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:42:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:42:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 04:42:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:43:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7c0b344a74c2d365a9a57a618f4a544c4e8e70f341f67973d3a22aee52a267b9`  
		Last Modified: Fri, 02 Sep 2022 01:00:04 GMT  
		Size: 26.7 MB (26663798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21ff0107faab8a809cab0821df6c069bdc690f3cda610960915bb07f0c47780`  
		Last Modified: Fri, 02 Sep 2022 04:48:55 GMT  
		Size: 6.6 MB (6603091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62edf58fe3260c89e551263ca83a26aead51b89196e35322ead3ba9023c23aed`  
		Last Modified: Fri, 02 Sep 2022 04:48:55 GMT  
		Size: 3.4 MB (3390812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df24de8e3685677e98d7d3aea7263fa8e11665eb30549c733d0760b8bdd6a28`  
		Last Modified: Fri, 02 Sep 2022 04:49:12 GMT  
		Size: 39.5 MB (39516416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a7dab39ac145cb27e46bda054f99ccfa338d3b9d323b4053bc8b9bacd5e88c`  
		Last Modified: Fri, 02 Sep 2022 04:49:47 GMT  
		Size: 170.7 MB (170654273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:aacd2841a1e442fc1a51300cf1624bb6f38dffcdff3c27fa7a1e7f942d4a3ebf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.3 MB (282251775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:015622ad1f917fcedd420ed628aa2356b7b6306b47a5885e9a81b47e602f7868`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:50:26 GMT
ADD file:79183abf8a1f4a6d4d04d73bcbe47e66f08bea9796acebd37d515855a459d132 in / 
# Thu, 01 Sep 2022 23:50:28 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:46:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:47:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 03:48:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:51:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ff717d18c49d9ec97ec3efef7dd73fe40829e1902f57d95a91516a42f69a091a`  
		Last Modified: Thu, 01 Sep 2022 23:53:03 GMT  
		Size: 32.1 MB (32082633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76c734e70f580a1e1db27a87020a89cba5ca648c7e9c85068bd42b1e3126ebe`  
		Last Modified: Fri, 02 Sep 2022 03:58:49 GMT  
		Size: 7.8 MB (7750570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09098d7e8658181028c27fff2df2b67293550987d175c5fab78075ddec7dd8ac`  
		Last Modified: Fri, 02 Sep 2022 03:58:48 GMT  
		Size: 4.4 MB (4361359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc897ebe25a803a066f6b1910e20dec6fc0162253745894a729850d1d32c57c8`  
		Last Modified: Fri, 02 Sep 2022 03:59:13 GMT  
		Size: 44.2 MB (44161167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b502c070e035bff4190a1869e54d6a3382719ec5513be9900a64d748b181aaad`  
		Last Modified: Fri, 02 Sep 2022 04:00:12 GMT  
		Size: 193.9 MB (193896046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:73bf7abfabd3ce3f80d631c8b4246bfb77cc7865a6ea4a088e1f1bcd8e898b00
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.8 MB (280785501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86d3e3d306e8b6f9c7a24e537c8ca6080ef2a051ad1d85eeb998da9e2c4ff0b1`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:14:23 GMT
ADD file:7c2ab85ecb4dc221c58ed92c05acad8d0b2ad90e46ec34c0a45fd5a5c3a9f7e2 in / 
# Fri, 02 Sep 2022 00:14:25 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 01:16:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 01:17:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 01:20:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 01:27:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:26010bd634bfca42373b6c36c189031dcce89570ea1226e9462a48d7a684240c`  
		Last Modified: Fri, 02 Sep 2022 00:32:57 GMT  
		Size: 25.6 MB (25594334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0826196a5d14cf0f019090771814dce885e1420c992b36ab31bfed7b28d86cf5`  
		Last Modified: Fri, 02 Sep 2022 02:00:23 GMT  
		Size: 5.9 MB (5930253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add19389e79fd75d5e3421d12568767855677a99cc4cfe5d50d5590034851237`  
		Last Modified: Fri, 02 Sep 2022 02:00:18 GMT  
		Size: 3.9 MB (3881273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f04e7e633bdcb9ab785ebbaa03714ef1fb30b6e9341369572e7eb655916151`  
		Last Modified: Fri, 02 Sep 2022 02:02:44 GMT  
		Size: 42.9 MB (42853430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67eaacb0aa78a362fe9ee225ee0e3ca057354904b8418793e4b7a1511e7aab3`  
		Last Modified: Fri, 02 Sep 2022 02:09:59 GMT  
		Size: 202.5 MB (202526211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a565fb5e9470fccd7e7164a3c87a5b2433fa673dc08c7e1a760184769385eb1c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.8 MB (228802204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfa992f61c6a6e4dbc5ee3ffe027303904613e78c952d7f7192bf0e5b84ed6b4`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:38 GMT
ADD file:61a0b983796cf76453cbc73a44968b8cefb9f90cc922075728432bdbdaaeb854 in / 
# Fri, 02 Sep 2022 01:03:40 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:09:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:10:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 02:10:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:12:16 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a51274124ed15147344e4d31d9378a33521faff1de175e551081c34c14db1b9f`  
		Last Modified: Fri, 02 Sep 2022 01:05:17 GMT  
		Size: 26.0 MB (25995506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a9727cdfe9e4d0ad02573de5f42a04ee40c70d014fcdffb4b684522e06d667`  
		Last Modified: Fri, 02 Sep 2022 02:17:04 GMT  
		Size: 6.5 MB (6470487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd626668509bf2d37bfd328fa211e8e7ad57c719072d9c7f1fc379bc2c187745`  
		Last Modified: Fri, 02 Sep 2022 02:17:04 GMT  
		Size: 3.6 MB (3625387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1947234f2c6685065fd711d09a80a70640e7a9c3b7521b8bbdd0c52afb85d8b5`  
		Last Modified: Fri, 02 Sep 2022 02:17:16 GMT  
		Size: 39.6 MB (39561768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74547493d0510538ad41fae3cfd6a5789215a1d753d5ea8509671d8f743cb2cf`  
		Last Modified: Fri, 02 Sep 2022 02:17:40 GMT  
		Size: 153.1 MB (153149056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:kinetic-curl`

```console
$ docker pull buildpack-deps@sha256:fbadf017868b978bb0f183a345be3b63fb1fe70738386dfc8bb9e93d1effd5f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:kinetic-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:4146f09f2e891abdc1f560cf823df40b6c3f0172adb7bf24edf74d69c22fb9e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37841463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:956194632e135c001d0e90d82f832aa6708b7d8beb963b98e27eacc4a96799bb`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:43 GMT
ADD file:d5de90ac61ee7027aa0900efb669efa73f611463cf73ab2cfdacadf5ab9fee19 in / 
# Thu, 01 Sep 2022 23:46:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:32:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:32:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0b78030514e08aad79cb596ba84b18b9579e90eac0b8e0c2dec483c3da8dbee8`  
		Last Modified: Thu, 01 Sep 2022 23:48:15 GMT  
		Size: 27.4 MB (27428015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71363ea1301988ddf4ef6039b34a05a19b44a70e1ba2764e95fa0f47b3585c12`  
		Last Modified: Fri, 02 Sep 2022 02:39:23 GMT  
		Size: 6.8 MB (6779788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d261ea038a7743d40031459e01e57001571ca5986a617d9e2d3174c66d98187a`  
		Last Modified: Fri, 02 Sep 2022 02:39:23 GMT  
		Size: 3.6 MB (3633660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:fc9add13cbee66aac1a50ef350bb1f7a61fbff4028de3ec5aa3853f52186f69f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.6 MB (35595513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19e80e45169f55fa54c17989c92f2067a23b1748bc1d414f7ad0adcc3be10c10`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 06:08:44 GMT
ADD file:6fea481ddc80754c10680e7c291055af82ef815eb0fdaf745c49c4f4cdf2afa1 in / 
# Fri, 02 Sep 2022 06:08:44 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 09:35:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 09:35:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1f63be4c3b8fca43746377bd8a99dd9b04acdd942d8464feaae1671e6363d920`  
		Last Modified: Fri, 02 Sep 2022 06:10:58 GMT  
		Size: 25.8 MB (25845683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c94aedbe9250aab4e90e8e88c1f2af520548789812f567b90a81f67dc9145e`  
		Last Modified: Fri, 02 Sep 2022 09:43:15 GMT  
		Size: 5.9 MB (5948408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78166495a53038ebe64fd164f5d7e26607173735e8a0e096424b99f947d93cb`  
		Last Modified: Fri, 02 Sep 2022 09:43:14 GMT  
		Size: 3.8 MB (3801422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7a58c082c08baa948c0393745478cfc6a621d44aa9e72c0b3e7e6c7d87fb7249
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.7 MB (36657701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ffef9f110163db57eac2f13cd57c0c78b549e7dbf112862ad7ddbbb3c863bf4`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:58:02 GMT
ADD file:1b9e898b22915c14e3d83959e989e2a653148ff82c8e2a1b3dfa8035256219aa in / 
# Fri, 02 Sep 2022 00:58:02 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:42:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:42:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:7c0b344a74c2d365a9a57a618f4a544c4e8e70f341f67973d3a22aee52a267b9`  
		Last Modified: Fri, 02 Sep 2022 01:00:04 GMT  
		Size: 26.7 MB (26663798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21ff0107faab8a809cab0821df6c069bdc690f3cda610960915bb07f0c47780`  
		Last Modified: Fri, 02 Sep 2022 04:48:55 GMT  
		Size: 6.6 MB (6603091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62edf58fe3260c89e551263ca83a26aead51b89196e35322ead3ba9023c23aed`  
		Last Modified: Fri, 02 Sep 2022 04:48:55 GMT  
		Size: 3.4 MB (3390812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:2f1739c1c6b4eac084c3655fe8a0d1f722d5234020ad66d85af3896252831c9e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44194562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb41d3ac587d6f78add9f6b9380f50796d6ba12866658651392d8f42597772c2`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:50:26 GMT
ADD file:79183abf8a1f4a6d4d04d73bcbe47e66f08bea9796acebd37d515855a459d132 in / 
# Thu, 01 Sep 2022 23:50:28 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:46:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:47:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ff717d18c49d9ec97ec3efef7dd73fe40829e1902f57d95a91516a42f69a091a`  
		Last Modified: Thu, 01 Sep 2022 23:53:03 GMT  
		Size: 32.1 MB (32082633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76c734e70f580a1e1db27a87020a89cba5ca648c7e9c85068bd42b1e3126ebe`  
		Last Modified: Fri, 02 Sep 2022 03:58:49 GMT  
		Size: 7.8 MB (7750570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09098d7e8658181028c27fff2df2b67293550987d175c5fab78075ddec7dd8ac`  
		Last Modified: Fri, 02 Sep 2022 03:58:48 GMT  
		Size: 4.4 MB (4361359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:27a5f062d5475bb7448ee24ce8540657304df8857324a254cab4b5b2f88a6995
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.4 MB (35405860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9316adf029fa960eedaf5a870e8ea5d065e27ffc98ed3823c735853fdfc69086`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:14:23 GMT
ADD file:7c2ab85ecb4dc221c58ed92c05acad8d0b2ad90e46ec34c0a45fd5a5c3a9f7e2 in / 
# Fri, 02 Sep 2022 00:14:25 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 01:16:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 01:17:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:26010bd634bfca42373b6c36c189031dcce89570ea1226e9462a48d7a684240c`  
		Last Modified: Fri, 02 Sep 2022 00:32:57 GMT  
		Size: 25.6 MB (25594334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0826196a5d14cf0f019090771814dce885e1420c992b36ab31bfed7b28d86cf5`  
		Last Modified: Fri, 02 Sep 2022 02:00:23 GMT  
		Size: 5.9 MB (5930253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add19389e79fd75d5e3421d12568767855677a99cc4cfe5d50d5590034851237`  
		Last Modified: Fri, 02 Sep 2022 02:00:18 GMT  
		Size: 3.9 MB (3881273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:1a4280bfe4ba337a4d6823ed783b787f4e47c972297bdc1fb87365481d92e6b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.1 MB (36091380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95fe882ebed7bf4928fe0c8bb698fbd2717de58f157144268dc3bf5a5bf74767`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:38 GMT
ADD file:61a0b983796cf76453cbc73a44968b8cefb9f90cc922075728432bdbdaaeb854 in / 
# Fri, 02 Sep 2022 01:03:40 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:09:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:10:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a51274124ed15147344e4d31d9378a33521faff1de175e551081c34c14db1b9f`  
		Last Modified: Fri, 02 Sep 2022 01:05:17 GMT  
		Size: 26.0 MB (25995506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a9727cdfe9e4d0ad02573de5f42a04ee40c70d014fcdffb4b684522e06d667`  
		Last Modified: Fri, 02 Sep 2022 02:17:04 GMT  
		Size: 6.5 MB (6470487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd626668509bf2d37bfd328fa211e8e7ad57c719072d9c7f1fc379bc2c187745`  
		Last Modified: Fri, 02 Sep 2022 02:17:04 GMT  
		Size: 3.6 MB (3625387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:kinetic-scm`

```console
$ docker pull buildpack-deps@sha256:acb0852335a3ebd50b51b14fbfb92eb19a1b99f55dcc4bdfadb2195e8ee5939c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:kinetic-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:828ba173c64d2b06cfab5015d103cacabaf810768a3edebde3bc29cbdc44e5b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.6 MB (77570973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdf0e5aaa1e96e04823419e7cc270da44b5ef7482b69063331a8f8dc4851ba7f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:43 GMT
ADD file:d5de90ac61ee7027aa0900efb669efa73f611463cf73ab2cfdacadf5ab9fee19 in / 
# Thu, 01 Sep 2022 23:46:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:32:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:32:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 02:32:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0b78030514e08aad79cb596ba84b18b9579e90eac0b8e0c2dec483c3da8dbee8`  
		Last Modified: Thu, 01 Sep 2022 23:48:15 GMT  
		Size: 27.4 MB (27428015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71363ea1301988ddf4ef6039b34a05a19b44a70e1ba2764e95fa0f47b3585c12`  
		Last Modified: Fri, 02 Sep 2022 02:39:23 GMT  
		Size: 6.8 MB (6779788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d261ea038a7743d40031459e01e57001571ca5986a617d9e2d3174c66d98187a`  
		Last Modified: Fri, 02 Sep 2022 02:39:23 GMT  
		Size: 3.6 MB (3633660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dee5c450c1549fab83f54e9138820f82132ebf0b50a52e7ffb97b6074e98c1b`  
		Last Modified: Fri, 02 Sep 2022 02:39:39 GMT  
		Size: 39.7 MB (39729510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:cfd3f516f9db19a7d0a3397bd2a4556f9fe1196d887519954a604ed38c08ae24
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.2 MB (78188598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b6c836955c987cb709f3f744b01bd49e876b7dfdfddb548a7b840351c8452b0`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 06:08:44 GMT
ADD file:6fea481ddc80754c10680e7c291055af82ef815eb0fdaf745c49c4f4cdf2afa1 in / 
# Fri, 02 Sep 2022 06:08:44 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 09:35:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 09:35:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 09:36:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1f63be4c3b8fca43746377bd8a99dd9b04acdd942d8464feaae1671e6363d920`  
		Last Modified: Fri, 02 Sep 2022 06:10:58 GMT  
		Size: 25.8 MB (25845683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c94aedbe9250aab4e90e8e88c1f2af520548789812f567b90a81f67dc9145e`  
		Last Modified: Fri, 02 Sep 2022 09:43:15 GMT  
		Size: 5.9 MB (5948408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78166495a53038ebe64fd164f5d7e26607173735e8a0e096424b99f947d93cb`  
		Last Modified: Fri, 02 Sep 2022 09:43:14 GMT  
		Size: 3.8 MB (3801422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28471ad57cdb7e9e4d1bd803eae0208867737111fd76d4143f4b6120903361b7`  
		Last Modified: Fri, 02 Sep 2022 09:43:34 GMT  
		Size: 42.6 MB (42593085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:e3b5b4e76e7beab59040a6636f56d76d7503606a20e63a3e2f9ea2a8bb6ac29d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76174117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2b653827e5a547aa259b9c8b69823046c120471f9a42d4cb3c39bfce50ac697`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:58:02 GMT
ADD file:1b9e898b22915c14e3d83959e989e2a653148ff82c8e2a1b3dfa8035256219aa in / 
# Fri, 02 Sep 2022 00:58:02 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:42:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:42:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 04:42:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7c0b344a74c2d365a9a57a618f4a544c4e8e70f341f67973d3a22aee52a267b9`  
		Last Modified: Fri, 02 Sep 2022 01:00:04 GMT  
		Size: 26.7 MB (26663798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21ff0107faab8a809cab0821df6c069bdc690f3cda610960915bb07f0c47780`  
		Last Modified: Fri, 02 Sep 2022 04:48:55 GMT  
		Size: 6.6 MB (6603091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62edf58fe3260c89e551263ca83a26aead51b89196e35322ead3ba9023c23aed`  
		Last Modified: Fri, 02 Sep 2022 04:48:55 GMT  
		Size: 3.4 MB (3390812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df24de8e3685677e98d7d3aea7263fa8e11665eb30549c733d0760b8bdd6a28`  
		Last Modified: Fri, 02 Sep 2022 04:49:12 GMT  
		Size: 39.5 MB (39516416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d1a0061871614fa08a0672d33b54065a27d2ac2e6fddb89f4b8d50f90beebb10
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.4 MB (88355729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb4218919910d1defe9ce53d3c83bc3ee4351f723a43693566be868052037c8d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:50:26 GMT
ADD file:79183abf8a1f4a6d4d04d73bcbe47e66f08bea9796acebd37d515855a459d132 in / 
# Thu, 01 Sep 2022 23:50:28 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:46:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:47:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 03:48:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ff717d18c49d9ec97ec3efef7dd73fe40829e1902f57d95a91516a42f69a091a`  
		Last Modified: Thu, 01 Sep 2022 23:53:03 GMT  
		Size: 32.1 MB (32082633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76c734e70f580a1e1db27a87020a89cba5ca648c7e9c85068bd42b1e3126ebe`  
		Last Modified: Fri, 02 Sep 2022 03:58:49 GMT  
		Size: 7.8 MB (7750570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09098d7e8658181028c27fff2df2b67293550987d175c5fab78075ddec7dd8ac`  
		Last Modified: Fri, 02 Sep 2022 03:58:48 GMT  
		Size: 4.4 MB (4361359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc897ebe25a803a066f6b1910e20dec6fc0162253745894a729850d1d32c57c8`  
		Last Modified: Fri, 02 Sep 2022 03:59:13 GMT  
		Size: 44.2 MB (44161167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:0ecd3a16684ad715fdc64797dcb67e50a578b932508e659b89877e29aeb60c31
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78259290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3eebb88c0344c66b13bb1996a4cd968b97228457505a37dac024aed53fc270e0`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:14:23 GMT
ADD file:7c2ab85ecb4dc221c58ed92c05acad8d0b2ad90e46ec34c0a45fd5a5c3a9f7e2 in / 
# Fri, 02 Sep 2022 00:14:25 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 01:16:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 01:17:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 01:20:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:26010bd634bfca42373b6c36c189031dcce89570ea1226e9462a48d7a684240c`  
		Last Modified: Fri, 02 Sep 2022 00:32:57 GMT  
		Size: 25.6 MB (25594334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0826196a5d14cf0f019090771814dce885e1420c992b36ab31bfed7b28d86cf5`  
		Last Modified: Fri, 02 Sep 2022 02:00:23 GMT  
		Size: 5.9 MB (5930253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add19389e79fd75d5e3421d12568767855677a99cc4cfe5d50d5590034851237`  
		Last Modified: Fri, 02 Sep 2022 02:00:18 GMT  
		Size: 3.9 MB (3881273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f04e7e633bdcb9ab785ebbaa03714ef1fb30b6e9341369572e7eb655916151`  
		Last Modified: Fri, 02 Sep 2022 02:02:44 GMT  
		Size: 42.9 MB (42853430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:f129e4299698e3c5c9ab8769330e17dd80fdc69e682f5705ef355e75dfc32ff8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75653148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:505a854970b8539945a41a684cd6895a2b377733c46184f17c584767122c2b75`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:38 GMT
ADD file:61a0b983796cf76453cbc73a44968b8cefb9f90cc922075728432bdbdaaeb854 in / 
# Fri, 02 Sep 2022 01:03:40 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:09:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:10:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 02:10:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a51274124ed15147344e4d31d9378a33521faff1de175e551081c34c14db1b9f`  
		Last Modified: Fri, 02 Sep 2022 01:05:17 GMT  
		Size: 26.0 MB (25995506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a9727cdfe9e4d0ad02573de5f42a04ee40c70d014fcdffb4b684522e06d667`  
		Last Modified: Fri, 02 Sep 2022 02:17:04 GMT  
		Size: 6.5 MB (6470487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd626668509bf2d37bfd328fa211e8e7ad57c719072d9c7f1fc379bc2c187745`  
		Last Modified: Fri, 02 Sep 2022 02:17:04 GMT  
		Size: 3.6 MB (3625387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1947234f2c6685065fd711d09a80a70640e7a9c3b7521b8bbdd0c52afb85d8b5`  
		Last Modified: Fri, 02 Sep 2022 02:17:16 GMT  
		Size: 39.6 MB (39561768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:latest`

```console
$ docker pull buildpack-deps@sha256:872ba70b0805b817db42d9ea75f066b5fe2be82d04d0dab69e41810edd9aa3f9
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
$ docker pull buildpack-deps@sha256:fdd46ac593b0dc4c54497b36e00e54c7759d068d9b9f014bd5b47bed430d4c2f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.4 MB (322416189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1966d2c176635cea14ac52f6a8a1d7d57101cb829eae63a9f3597cdee7a0ef6f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:40 GMT
ADD file:6944d322f4c04bd2192061822af5cbec8ac0a6b424c461d66174d32aed604972 in / 
# Tue, 23 Aug 2022 00:20:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:48:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:48:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 00:48:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:49:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1671565cc8df8c365c9b661d3fbc164e73d01f1b0430c6179588428f99a9da2e`  
		Last Modified: Tue, 23 Aug 2022 00:24:32 GMT  
		Size: 55.0 MB (55007555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e94d13e55e7a4ef17ff21376f57fb95c7e1706931f8704aa99260968d81f6e4`  
		Last Modified: Tue, 23 Aug 2022 00:55:37 GMT  
		Size: 5.2 MB (5163019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9c7528c685216129e8e67bf362a7702e7b1daa585ab85546a41508830657d6`  
		Last Modified: Tue, 23 Aug 2022 00:55:38 GMT  
		Size: 10.9 MB (10876472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ad072f9cd16fc8eb93b182b20e758e11acc0ef60babef0bf1043c08de1901a`  
		Last Modified: Tue, 23 Aug 2022 00:55:57 GMT  
		Size: 54.6 MB (54584135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b983117533b718374f1701ef593dd2afa6613c7908c6553be8e2a150e6448a`  
		Last Modified: Tue, 23 Aug 2022 00:56:35 GMT  
		Size: 196.8 MB (196785008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:48f086404ea033fe19fa0dd18cd1989c0b585f07c7353ff246098068b1075971
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.5 MB (295500312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:543ae8ede83fbb55855cee053b3a548534170a1c9e89ce34e227685abb1a46f2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:16:51 GMT
ADD file:132abd62c4fa546798c96d5b1f6f409de9ee27242caf6c479d65309b764c3ece in / 
# Tue, 23 Aug 2022 01:16:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 06:19:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 06:19:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 06:19:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 06:21:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1918e2afd901ca723b3483d8d521789daac45ddbaae2bf9fd813933e826f39b4`  
		Last Modified: Tue, 23 Aug 2022 01:22:10 GMT  
		Size: 52.5 MB (52547848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a58d3f469ed5c6be23bbc74a836bceb306e58e8cd5e58e4464c2b23519543a`  
		Last Modified: Tue, 23 Aug 2022 06:26:58 GMT  
		Size: 5.1 MB (5070690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61379bcded34629fad0582d1d42f2cba36b5f418591509e15301773304e7c7c0`  
		Last Modified: Tue, 23 Aug 2022 06:26:59 GMT  
		Size: 10.6 MB (10573758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c872e375903a379cc5ab82220655ab6973d82f8b48ab51b42d197a4ab189b6b`  
		Last Modified: Tue, 23 Aug 2022 06:27:30 GMT  
		Size: 52.3 MB (52320330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8993dbe2a09d90eb21f3d73a07f953f77bed210372ca285a9f7d8046891b8aa`  
		Last Modified: Tue, 23 Aug 2022 06:28:23 GMT  
		Size: 175.0 MB (174987686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:520bd48d184d2e1e72a3180fb98d6b1a72b711d77e12bcfb2dba659f40f40cc8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.0 MB (282979755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1d91ec2297d651816190904a39f4d4be0b91a78799a8484ab081b8081bd860d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:42:43 GMT
ADD file:21190c24a038c3c9de64b88797bf00e4c4319bd598c7c465cab2ca88d0502416 in / 
# Tue, 23 Aug 2022 01:42:43 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 12:59:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:00:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 13:00:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:01:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c715a126a4d5182c28d2d7b1c81de847bfbbacf6851819fef3eb28e3feb7db0e`  
		Last Modified: Tue, 23 Aug 2022 01:49:30 GMT  
		Size: 50.2 MB (50204931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cecc62e275236714359bda7d1f9c8412e8fa8539f3ef682eebd9c77986c927d`  
		Last Modified: Tue, 23 Aug 2022 13:11:58 GMT  
		Size: 4.9 MB (4930827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818eb872fe75602d611beeac0db63da0a4d8a67aee8b909d5114814f76446a5e`  
		Last Modified: Tue, 23 Aug 2022 13:11:59 GMT  
		Size: 10.2 MB (10217900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94cbc350f4a21916bb6fe70920c962a4889a5059aee86258e4d8263f0c7afbef`  
		Last Modified: Tue, 23 Aug 2022 13:12:28 GMT  
		Size: 50.3 MB (50342476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfc7e160811f0c470f91fe54fc02b224cb6ccbca07472ffcff55826d15bb26d`  
		Last Modified: Tue, 23 Aug 2022 13:13:20 GMT  
		Size: 167.3 MB (167283621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:6a657d9df2ce6540c05ceccaae91f294cb8ad870d9ea7cbc582a0642a5a8e0e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.7 MB (313684616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c31d31f8a9a1673a5b75dcc8e41518512dc0227c069e4cb4a48a9d45a3ade89`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:16 GMT
ADD file:ce6014a27d18915dc6d46c5c1f0f894f0027d1e41fbebb1599c16371b7bab2f1 in / 
# Tue, 23 Aug 2022 01:52:18 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:27:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:28:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 02:28:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:29:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cd84405c8b9e7a8c3d580c2148d25120dd697ea61e1cb55a62f33e67988b7043`  
		Last Modified: Tue, 23 Aug 2022 01:57:29 GMT  
		Size: 53.7 MB (53690830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d98e120b809269e56de468d2b91569789c521011e4d9b1806e43fd04462de2`  
		Last Modified: Tue, 23 Aug 2022 02:36:44 GMT  
		Size: 4.9 MB (4944180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb6be5911b40ca548e48c10b09cb2312f1698b4c84f09711c69389a94b1a8be`  
		Last Modified: Tue, 23 Aug 2022 02:36:44 GMT  
		Size: 10.7 MB (10657442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db608c3c3ce3568556faf63acbc2069811afe242faf8992ccf0ab1986ee38e4f`  
		Last Modified: Tue, 23 Aug 2022 02:37:07 GMT  
		Size: 54.7 MB (54680886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef10f752bfb9bb5888d549687e75a51ad78e1523ee87958e8b464cbd4dee4bb2`  
		Last Modified: Tue, 23 Aug 2022 02:37:46 GMT  
		Size: 189.7 MB (189711278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; 386

```console
$ docker pull buildpack-deps@sha256:6462b9cedd6360f9ac58ef0a745ed79497259cf4382b330b0a6ade58054037fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.8 MB (327786054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a954a50143d33244bd5b54771fe808f36befea012da728e64638c4f80b3f6b8c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:24 GMT
ADD file:4012c41187a03bdb3d37bec80f6255a1d46582e3ed145b4f313e42196529e524 in / 
# Tue, 23 Aug 2022 01:02:25 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:31:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:31:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:32:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:33:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6f683b9c66ef80b527ee5e4cb11969c6e0c1400ab69a4f1279af90f5766d70c7`  
		Last Modified: Tue, 23 Aug 2022 01:07:53 GMT  
		Size: 56.0 MB (56012624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f506948c8aa6d2e0693b583a388ce5e10b4393763bd2ea2529af3bfaa07f0c92`  
		Last Modified: Tue, 23 Aug 2022 01:40:01 GMT  
		Size: 5.1 MB (5085725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915cb3138c0c978b1806934d3f979cff24ecaed321fe7e13caa292cf9ca73dcc`  
		Last Modified: Tue, 23 Aug 2022 01:40:01 GMT  
		Size: 11.0 MB (11032841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc001487b6a15d61b32ac2dbd4b06bdede894077b8fcd3fa2f3969f98052bc3`  
		Last Modified: Tue, 23 Aug 2022 01:40:24 GMT  
		Size: 55.9 MB (55922719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e27a84eb0ba3a89f9e9e474d9c853c2dc7e9c83ef7d1e7281d208fd866b4c3`  
		Last Modified: Tue, 23 Aug 2022 01:41:12 GMT  
		Size: 199.7 MB (199732145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:a2b9c6b327a9a223c3efa1706bc2b9db685a596067cf19dcdd74613196680350
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.1 MB (301099619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44d5d833b9dcbd729eba0daafec46b29b0f0c91fb9dabc2d09bf20e3ce4d4b07`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:10:38 GMT
ADD file:a55d19f262e8338f932ce871c1cbc1718f9f74a5002212f38fea74f3858460a9 in / 
# Tue, 23 Aug 2022 00:10:43 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 22:24:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 22:24:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 22:26:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 22:33:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5ce438ccc597187e8a0dab5cc8906e6a0ec75a9320e55225ad2ec24765f7c0b4`  
		Last Modified: Tue, 23 Aug 2022 00:18:51 GMT  
		Size: 53.3 MB (53272999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567ecdfd8aa8d0bdcecff06b6b73dfbde6ae5451a3afec2a33aee7ca527b61e9`  
		Last Modified: Tue, 23 Aug 2022 22:49:03 GMT  
		Size: 4.9 MB (4918268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9374a0689765aeaeee15bb1c011bddd8cb323e6002385ceb42952a14d3210410`  
		Last Modified: Tue, 23 Aug 2022 22:49:06 GMT  
		Size: 10.7 MB (10661281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ccffd65aa7de17818aaae93c681cc96ca65baf5ab87b1989328259e139d360d`  
		Last Modified: Tue, 23 Aug 2022 22:49:57 GMT  
		Size: 53.3 MB (53304283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba6ce1b89a90d1ecaf04f415e6b8d8885f95ffc7c0a9357b6ef5545fc5e668e2`  
		Last Modified: Tue, 23 Aug 2022 22:52:01 GMT  
		Size: 178.9 MB (178942788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d26e0e6609eee5d0cc12d24a0e666e615785a20c5f2bcc91b8c39a3a1a85d14f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.0 MB (330981508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4404daf2be9fe8125eb280020678875923138a2f95a6de510414b2979fc8ea78`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:24:30 GMT
ADD file:c498f58d8dc50a2a20679642be8f6f43de8b79455438a1c237ef4c94a9ffe34c in / 
# Tue, 23 Aug 2022 01:24:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:58:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:59:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:01:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:62d01a7bda469557451a05bab1d4de7f53dd936e8032b36635019fd54cd927e4`  
		Last Modified: Tue, 23 Aug 2022 01:29:57 GMT  
		Size: 58.9 MB (58909173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b002340b938f821f3b0978eb9bfc47d2b8fe91b33c50508bd618c3c4b0ffe0`  
		Last Modified: Tue, 23 Aug 2022 02:10:43 GMT  
		Size: 5.4 MB (5412576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c65f43f4fd248e0fd18c35535f21fcafa740bdde05c5c367f32926f478e55f`  
		Last Modified: Tue, 23 Aug 2022 02:10:44 GMT  
		Size: 11.6 MB (11628949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6e7f52d8f52b4e830cdd20f538730eebe893f6c1f11aac1d0457ae132da2e8`  
		Last Modified: Tue, 23 Aug 2022 02:11:16 GMT  
		Size: 58.9 MB (58866219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35fecee5c5cd927c82781b73850d4cbf96c866f08985a8a76ee30c510df49f06`  
		Last Modified: Tue, 23 Aug 2022 02:12:17 GMT  
		Size: 196.2 MB (196164591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:7137006106c6222467d1d066c08b261d2ac29572e757ca58573eb833e89bb865
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.1 MB (296058506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:640e9d9a4e7fd555cdb338b68646231938a22a5a3322a831aa6f652376231080`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:53:42 GMT
ADD file:799d2eac4bf12dcb56eca0b771da879e8873a2a81b4d74520db7d6665d448ff6 in / 
# Tue, 23 Aug 2022 00:53:45 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 09:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 09:51:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 09:51:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 09:52:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e8428caa8cb9dd5cd48266f588e1d935181b0d75e5f4680a9d4d03700d44289`  
		Last Modified: Tue, 23 Aug 2022 01:01:15 GMT  
		Size: 53.3 MB (53279185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b41fe9abb9a7707d3bfd9881e997384ad70ba3f811c4152a16e11585318bd5`  
		Last Modified: Tue, 23 Aug 2022 09:59:58 GMT  
		Size: 5.1 MB (5146782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0215c1024f20ea76e1b536fcf226d87a639e72806443621a0bf52a719c0218fd`  
		Last Modified: Tue, 23 Aug 2022 09:59:59 GMT  
		Size: 10.8 MB (10765873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aeff4b644e5176d180f566f9889b6ed12e443f2fb955b119865cc113d26c3b1`  
		Last Modified: Tue, 23 Aug 2022 10:00:19 GMT  
		Size: 54.1 MB (54054805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e54f765beb5bf3b5c78fed34fddcc79e45dd90b63b47b01505666e38691ce6`  
		Last Modified: Tue, 23 Aug 2022 10:00:47 GMT  
		Size: 172.8 MB (172811861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldstable`

```console
$ docker pull buildpack-deps@sha256:d73ba7863f3958cade1ef32f7620c3751ba5cd9653ff382a1b222ec17906884e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:oldstable` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:54ef455d50cec890ed58b814dd005747a088aeff36543169bc85c99b9ceba5a5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.6 MB (312645189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7f74fbf296e791b18cd52ed04807250ec4ec525b4305015447d0660198477c5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:00 GMT
ADD file:d420ffdf63082e03517284553796e5a100e425201458860f07b1aa8598c5929a in / 
# Tue, 23 Aug 2022 00:21:00 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:49:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:49:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 00:49:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:50:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76dff75df4d9dbdf29a4459adaec745740bfb476cd915906e33eddd9cd94db93`  
		Last Modified: Tue, 23 Aug 2022 00:25:20 GMT  
		Size: 50.4 MB (50440273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8c90a1c4bb422a88cc9ff532712db3c6a7a8cdc5030af2e60ec51947f2c8aa`  
		Last Modified: Tue, 23 Aug 2022 00:56:49 GMT  
		Size: 7.9 MB (7856913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3662c1050803c4e17c1848dffe636eae5e6e5aafb8f1fffcf82248ccfef21c2`  
		Last Modified: Tue, 23 Aug 2022 00:56:49 GMT  
		Size: 10.0 MB (9998130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5dcb7dd59206e662084addf318ef296595c82800a9107e362439db4c158df9`  
		Last Modified: Tue, 23 Aug 2022 00:57:06 GMT  
		Size: 51.8 MB (51843805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa57cc7ce3410dc0507beaaf475eb582c5ffccea2d603d2c024b77a69990aba2`  
		Last Modified: Tue, 23 Aug 2022 00:57:40 GMT  
		Size: 192.5 MB (192506068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:e67231ddffab43682ab5597e54d94ccb319a189890cd39e8ca9627a3ce4b1a78
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.5 MB (278465267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f54ac2d77406431a8ece5e7baf1d11a14105ce733fe737b9be9dd484ec6e41e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:18 GMT
ADD file:f02e7759ba5d55ff457d421191df7d2973666205453bbb6755214288b1c5527b in / 
# Tue, 23 Aug 2022 01:43:19 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 13:02:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:02:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 13:02:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:03:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e43c24e08caa0d5875ad9b74a9503702850e39637c5dfe8cf2b231adfb60322c`  
		Last Modified: Tue, 23 Aug 2022 01:50:31 GMT  
		Size: 45.9 MB (45914940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:336dc8987db19d66a0f9f594deebb34a07cbdbc58f4ca037260b77716ac3762f`  
		Last Modified: Tue, 23 Aug 2022 13:13:39 GMT  
		Size: 7.1 MB (7145481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d4e661f35fcba3168ad779ef39cc7bbebaea0a1ab6977ea6a07497f64f1545`  
		Last Modified: Tue, 23 Aug 2022 13:13:39 GMT  
		Size: 9.3 MB (9344463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34357d0aae8fbf38566a850196f436a0111c5c9eeb3a27256f78dfcff8ea6981`  
		Last Modified: Tue, 23 Aug 2022 13:14:04 GMT  
		Size: 47.4 MB (47359364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b803711841bad336591ae6cde869b0acee5e53607ac006c3205ce3f2594f71`  
		Last Modified: Tue, 23 Aug 2022 13:14:52 GMT  
		Size: 168.7 MB (168701019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:8b05537816456d43a93b68f81bdf4864538ab9f22e43c3bc67be6e2e5142fe80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.0 MB (302979491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e148476bf876492d4a04bfdec4c4cc661f95bdee63f910dd2a353200c39cff41`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:43 GMT
ADD file:a3ba1802e6680a14c605fbe754f9fb56a642f0799f51ce0010d253cb66c9691f in / 
# Tue, 23 Aug 2022 01:52:44 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:29:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:29:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 02:29:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:30:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3332e5c67ba650c61dbca801cf2739a1f5b6faac33f7b0543f97f4ab1165fe69`  
		Last Modified: Tue, 23 Aug 2022 01:58:23 GMT  
		Size: 49.2 MB (49228066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61dd9df5607d27eb8d7af8db0ec4f1e1634f54db08cd06c03131ac8a25ff710b`  
		Last Modified: Tue, 23 Aug 2022 02:38:02 GMT  
		Size: 7.7 MB (7720187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28122dfd7d7cf006c384197d918567d3d812f94f0030b87104b26c2d2ded69a`  
		Last Modified: Tue, 23 Aug 2022 02:38:02 GMT  
		Size: 9.8 MB (9768739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e3536e0d6df43cb88858e2f77eaa514bd51e583a6d593d494fcb67e03bfda1`  
		Last Modified: Tue, 23 Aug 2022 02:38:21 GMT  
		Size: 52.2 MB (52174764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34806818c453e9a369973b475f26ada73304ea74e3ae1860af58abbe6872a7c`  
		Last Modified: Tue, 23 Aug 2022 02:38:56 GMT  
		Size: 184.1 MB (184087735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:5be2d7d74dcf23d0c9e478b0c6a4210d4af26c55053c9a3f25a7a3ec6f3e3a3d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.8 MB (321826790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef7f83e2174f51cd4b5480254a81d9d5eade013377c85039ee068ab9960f7923`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:51 GMT
ADD file:7ad537f8110f70df174d79a50cbe08fc480933797f0717e94529061bbfd00759 in / 
# Tue, 23 Aug 2022 01:02:52 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:33:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:33:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:33:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:35:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f73bf17b8a4e28cf438c1af60c558d4943ab3fea50a934b856e19e18b2cefc70`  
		Last Modified: Tue, 23 Aug 2022 01:08:52 GMT  
		Size: 51.2 MB (51202934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f552c2f5ee3c58b15814627cdfd5f450b32574510bab9c05fcdcfee72a5937`  
		Last Modified: Tue, 23 Aug 2022 01:41:27 GMT  
		Size: 8.0 MB (8022887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f116e2a9c83bb2f0fa2b290281df8f4dc03cd9f375f5b485cc3811581f843efb`  
		Last Modified: Tue, 23 Aug 2022 01:41:27 GMT  
		Size: 10.1 MB (10123789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8adc65b9373ec90849e46f84946cc18555ee8bd2be22479432d05734cc9738ac`  
		Last Modified: Tue, 23 Aug 2022 01:41:47 GMT  
		Size: 53.4 MB (53443079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0a01d7abbb9d320a302f32c458653f6d3dded4b42a38c0118e8e4ecbd4d4d9`  
		Last Modified: Tue, 23 Aug 2022 01:42:22 GMT  
		Size: 199.0 MB (199034101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldstable-curl`

```console
$ docker pull buildpack-deps@sha256:ac3799eb356b54a0e444ec493fa1b135da74a0dad504461b33d31b24e89af24a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:oldstable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:8e5706c8aebcc047d936e740c3c19f0590273be5d60219de6de26931a0b4d300
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68295316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d50e24bcc3757da5bdbefd30f0ac73d015c6924ff9b170bdb884618259d23058`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:00 GMT
ADD file:d420ffdf63082e03517284553796e5a100e425201458860f07b1aa8598c5929a in / 
# Tue, 23 Aug 2022 00:21:00 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:49:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:49:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:76dff75df4d9dbdf29a4459adaec745740bfb476cd915906e33eddd9cd94db93`  
		Last Modified: Tue, 23 Aug 2022 00:25:20 GMT  
		Size: 50.4 MB (50440273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8c90a1c4bb422a88cc9ff532712db3c6a7a8cdc5030af2e60ec51947f2c8aa`  
		Last Modified: Tue, 23 Aug 2022 00:56:49 GMT  
		Size: 7.9 MB (7856913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3662c1050803c4e17c1848dffe636eae5e6e5aafb8f1fffcf82248ccfef21c2`  
		Last Modified: Tue, 23 Aug 2022 00:56:49 GMT  
		Size: 10.0 MB (9998130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:72aea0997fe2f3d263507c131f7c5480bd9bfb889795778b8ce9ebb939ff2015
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62404884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c74b374874b15e1eea9e762b24cc862a89f75413a8c654b76ad75567c76af52`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:18 GMT
ADD file:f02e7759ba5d55ff457d421191df7d2973666205453bbb6755214288b1c5527b in / 
# Tue, 23 Aug 2022 01:43:19 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 13:02:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:02:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e43c24e08caa0d5875ad9b74a9503702850e39637c5dfe8cf2b231adfb60322c`  
		Last Modified: Tue, 23 Aug 2022 01:50:31 GMT  
		Size: 45.9 MB (45914940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:336dc8987db19d66a0f9f594deebb34a07cbdbc58f4ca037260b77716ac3762f`  
		Last Modified: Tue, 23 Aug 2022 13:13:39 GMT  
		Size: 7.1 MB (7145481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d4e661f35fcba3168ad779ef39cc7bbebaea0a1ab6977ea6a07497f64f1545`  
		Last Modified: Tue, 23 Aug 2022 13:13:39 GMT  
		Size: 9.3 MB (9344463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:528364512919c0312fa735c9613c158e8f3f48ad9e975b98c070c5cbaf2169a6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66716992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42ed8e9cb3fefc1dcc0bdf879faa7bce5abc302af284c835bfd67a6270c8e94c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:43 GMT
ADD file:a3ba1802e6680a14c605fbe754f9fb56a642f0799f51ce0010d253cb66c9691f in / 
# Tue, 23 Aug 2022 01:52:44 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:29:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:29:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3332e5c67ba650c61dbca801cf2739a1f5b6faac33f7b0543f97f4ab1165fe69`  
		Last Modified: Tue, 23 Aug 2022 01:58:23 GMT  
		Size: 49.2 MB (49228066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61dd9df5607d27eb8d7af8db0ec4f1e1634f54db08cd06c03131ac8a25ff710b`  
		Last Modified: Tue, 23 Aug 2022 02:38:02 GMT  
		Size: 7.7 MB (7720187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28122dfd7d7cf006c384197d918567d3d812f94f0030b87104b26c2d2ded69a`  
		Last Modified: Tue, 23 Aug 2022 02:38:02 GMT  
		Size: 9.8 MB (9768739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:4545f198fdceaa38ea7eb36df694364dd649e58010fdc8f6e4b1b1a07a31c0aa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.3 MB (69349610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2bbae5151d08a59f94a679035d3279d0bb5385445c5b24a6a49ac9093adacb4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:51 GMT
ADD file:7ad537f8110f70df174d79a50cbe08fc480933797f0717e94529061bbfd00759 in / 
# Tue, 23 Aug 2022 01:02:52 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:33:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:33:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f73bf17b8a4e28cf438c1af60c558d4943ab3fea50a934b856e19e18b2cefc70`  
		Last Modified: Tue, 23 Aug 2022 01:08:52 GMT  
		Size: 51.2 MB (51202934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f552c2f5ee3c58b15814627cdfd5f450b32574510bab9c05fcdcfee72a5937`  
		Last Modified: Tue, 23 Aug 2022 01:41:27 GMT  
		Size: 8.0 MB (8022887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f116e2a9c83bb2f0fa2b290281df8f4dc03cd9f375f5b485cc3811581f843efb`  
		Last Modified: Tue, 23 Aug 2022 01:41:27 GMT  
		Size: 10.1 MB (10123789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldstable-scm`

```console
$ docker pull buildpack-deps@sha256:ef0eccf4ba6e75c9d8ceb8d2163039218338706f9d229ec9210dc786d4f25dbf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:oldstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:003fbe71ab8e0aa49a38abea68017b20ade0244ca7fd112545f34d00e8d93f29
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120139121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d1c17948b08f2ddc164ca234f7b968e456395dba24dca1bebba323717197e8a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:00 GMT
ADD file:d420ffdf63082e03517284553796e5a100e425201458860f07b1aa8598c5929a in / 
# Tue, 23 Aug 2022 00:21:00 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:49:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:49:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 00:49:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76dff75df4d9dbdf29a4459adaec745740bfb476cd915906e33eddd9cd94db93`  
		Last Modified: Tue, 23 Aug 2022 00:25:20 GMT  
		Size: 50.4 MB (50440273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8c90a1c4bb422a88cc9ff532712db3c6a7a8cdc5030af2e60ec51947f2c8aa`  
		Last Modified: Tue, 23 Aug 2022 00:56:49 GMT  
		Size: 7.9 MB (7856913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3662c1050803c4e17c1848dffe636eae5e6e5aafb8f1fffcf82248ccfef21c2`  
		Last Modified: Tue, 23 Aug 2022 00:56:49 GMT  
		Size: 10.0 MB (9998130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5dcb7dd59206e662084addf318ef296595c82800a9107e362439db4c158df9`  
		Last Modified: Tue, 23 Aug 2022 00:57:06 GMT  
		Size: 51.8 MB (51843805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:cf25863e9e2ffa09317a598c2342c471a94d6c51cf58f59a7bf46b54a0851382
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109764248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:158dff8b83e31481d64645d01a2bbf745206bad2d79112ffa570cb67c17ebd69`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:18 GMT
ADD file:f02e7759ba5d55ff457d421191df7d2973666205453bbb6755214288b1c5527b in / 
# Tue, 23 Aug 2022 01:43:19 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 13:02:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:02:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 13:02:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e43c24e08caa0d5875ad9b74a9503702850e39637c5dfe8cf2b231adfb60322c`  
		Last Modified: Tue, 23 Aug 2022 01:50:31 GMT  
		Size: 45.9 MB (45914940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:336dc8987db19d66a0f9f594deebb34a07cbdbc58f4ca037260b77716ac3762f`  
		Last Modified: Tue, 23 Aug 2022 13:13:39 GMT  
		Size: 7.1 MB (7145481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d4e661f35fcba3168ad779ef39cc7bbebaea0a1ab6977ea6a07497f64f1545`  
		Last Modified: Tue, 23 Aug 2022 13:13:39 GMT  
		Size: 9.3 MB (9344463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34357d0aae8fbf38566a850196f436a0111c5c9eeb3a27256f78dfcff8ea6981`  
		Last Modified: Tue, 23 Aug 2022 13:14:04 GMT  
		Size: 47.4 MB (47359364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:687528f9bc5cc2787143f4aa993a59abb154dd027597b4ac853e084bff5f3202
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.9 MB (118891756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b51c54783cb65ffe0a52ebda1f30f9e23ae93f8e0572f8210d6c71bcee8184b9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:43 GMT
ADD file:a3ba1802e6680a14c605fbe754f9fb56a642f0799f51ce0010d253cb66c9691f in / 
# Tue, 23 Aug 2022 01:52:44 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:29:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:29:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 02:29:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3332e5c67ba650c61dbca801cf2739a1f5b6faac33f7b0543f97f4ab1165fe69`  
		Last Modified: Tue, 23 Aug 2022 01:58:23 GMT  
		Size: 49.2 MB (49228066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61dd9df5607d27eb8d7af8db0ec4f1e1634f54db08cd06c03131ac8a25ff710b`  
		Last Modified: Tue, 23 Aug 2022 02:38:02 GMT  
		Size: 7.7 MB (7720187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28122dfd7d7cf006c384197d918567d3d812f94f0030b87104b26c2d2ded69a`  
		Last Modified: Tue, 23 Aug 2022 02:38:02 GMT  
		Size: 9.8 MB (9768739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e3536e0d6df43cb88858e2f77eaa514bd51e583a6d593d494fcb67e03bfda1`  
		Last Modified: Tue, 23 Aug 2022 02:38:21 GMT  
		Size: 52.2 MB (52174764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:1b34deb70dfb8cdc508587152cf0e8400942901fcc8bb73787257dfb00876070
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.8 MB (122792689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d1b8cd3e85526cbf00e64aeb0a2fa39cf32001886e42e38f6ab3d923d2091d6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:51 GMT
ADD file:7ad537f8110f70df174d79a50cbe08fc480933797f0717e94529061bbfd00759 in / 
# Tue, 23 Aug 2022 01:02:52 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:33:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:33:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:33:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f73bf17b8a4e28cf438c1af60c558d4943ab3fea50a934b856e19e18b2cefc70`  
		Last Modified: Tue, 23 Aug 2022 01:08:52 GMT  
		Size: 51.2 MB (51202934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f552c2f5ee3c58b15814627cdfd5f450b32574510bab9c05fcdcfee72a5937`  
		Last Modified: Tue, 23 Aug 2022 01:41:27 GMT  
		Size: 8.0 MB (8022887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f116e2a9c83bb2f0fa2b290281df8f4dc03cd9f375f5b485cc3811581f843efb`  
		Last Modified: Tue, 23 Aug 2022 01:41:27 GMT  
		Size: 10.1 MB (10123789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8adc65b9373ec90849e46f84946cc18555ee8bd2be22479432d05734cc9738ac`  
		Last Modified: Tue, 23 Aug 2022 01:41:47 GMT  
		Size: 53.4 MB (53443079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:scm`

```console
$ docker pull buildpack-deps@sha256:a7a9dbad2a104ca82facdb49ca65421b485045a3a51aad05bd44609b839401a1
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
$ docker pull buildpack-deps@sha256:6c1872f4ea21628b7c323305593b94d6ecc5125852b4a03827c6d38b473835d2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.6 MB (125631181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e73278505bb143c007d79f686483ae493b77ad2ad4f7cadc67deeb86f4dd38e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:40 GMT
ADD file:6944d322f4c04bd2192061822af5cbec8ac0a6b424c461d66174d32aed604972 in / 
# Tue, 23 Aug 2022 00:20:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:48:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:48:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 00:48:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1671565cc8df8c365c9b661d3fbc164e73d01f1b0430c6179588428f99a9da2e`  
		Last Modified: Tue, 23 Aug 2022 00:24:32 GMT  
		Size: 55.0 MB (55007555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e94d13e55e7a4ef17ff21376f57fb95c7e1706931f8704aa99260968d81f6e4`  
		Last Modified: Tue, 23 Aug 2022 00:55:37 GMT  
		Size: 5.2 MB (5163019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9c7528c685216129e8e67bf362a7702e7b1daa585ab85546a41508830657d6`  
		Last Modified: Tue, 23 Aug 2022 00:55:38 GMT  
		Size: 10.9 MB (10876472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ad072f9cd16fc8eb93b182b20e758e11acc0ef60babef0bf1043c08de1901a`  
		Last Modified: Tue, 23 Aug 2022 00:55:57 GMT  
		Size: 54.6 MB (54584135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:f544bf2e62950527f9e904a056de2ffc7f7d57a0051cc0a83f53029d715f2847
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.5 MB (120512626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:254098229367b0e03446fdc4d0858c497972184186719e50d9853daf38a33bb0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:16:51 GMT
ADD file:132abd62c4fa546798c96d5b1f6f409de9ee27242caf6c479d65309b764c3ece in / 
# Tue, 23 Aug 2022 01:16:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 06:19:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 06:19:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 06:19:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1918e2afd901ca723b3483d8d521789daac45ddbaae2bf9fd813933e826f39b4`  
		Last Modified: Tue, 23 Aug 2022 01:22:10 GMT  
		Size: 52.5 MB (52547848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a58d3f469ed5c6be23bbc74a836bceb306e58e8cd5e58e4464c2b23519543a`  
		Last Modified: Tue, 23 Aug 2022 06:26:58 GMT  
		Size: 5.1 MB (5070690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61379bcded34629fad0582d1d42f2cba36b5f418591509e15301773304e7c7c0`  
		Last Modified: Tue, 23 Aug 2022 06:26:59 GMT  
		Size: 10.6 MB (10573758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c872e375903a379cc5ab82220655ab6973d82f8b48ab51b42d197a4ab189b6b`  
		Last Modified: Tue, 23 Aug 2022 06:27:30 GMT  
		Size: 52.3 MB (52320330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:495a7139ac1f0b677a9476288d454f9dfd4763312ef4dc4d467ce3f29c36caed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.7 MB (115696134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e362c69b51c9b48c55b381399fc2b7a49ec81e115a633a60638b43084b817c9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:42:43 GMT
ADD file:21190c24a038c3c9de64b88797bf00e4c4319bd598c7c465cab2ca88d0502416 in / 
# Tue, 23 Aug 2022 01:42:43 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 12:59:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:00:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 13:00:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c715a126a4d5182c28d2d7b1c81de847bfbbacf6851819fef3eb28e3feb7db0e`  
		Last Modified: Tue, 23 Aug 2022 01:49:30 GMT  
		Size: 50.2 MB (50204931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cecc62e275236714359bda7d1f9c8412e8fa8539f3ef682eebd9c77986c927d`  
		Last Modified: Tue, 23 Aug 2022 13:11:58 GMT  
		Size: 4.9 MB (4930827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818eb872fe75602d611beeac0db63da0a4d8a67aee8b909d5114814f76446a5e`  
		Last Modified: Tue, 23 Aug 2022 13:11:59 GMT  
		Size: 10.2 MB (10217900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94cbc350f4a21916bb6fe70920c962a4889a5059aee86258e4d8263f0c7afbef`  
		Last Modified: Tue, 23 Aug 2022 13:12:28 GMT  
		Size: 50.3 MB (50342476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:5156f3bb278fb0dda42cdf0b406331f8809ab19a049e6ea5506665811c002475
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.0 MB (123973338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acf31c8a1856f38bfa1a001f3b72d3e9678c5aadee3ec10352d90f571361e1fe`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:16 GMT
ADD file:ce6014a27d18915dc6d46c5c1f0f894f0027d1e41fbebb1599c16371b7bab2f1 in / 
# Tue, 23 Aug 2022 01:52:18 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:27:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:28:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 02:28:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cd84405c8b9e7a8c3d580c2148d25120dd697ea61e1cb55a62f33e67988b7043`  
		Last Modified: Tue, 23 Aug 2022 01:57:29 GMT  
		Size: 53.7 MB (53690830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d98e120b809269e56de468d2b91569789c521011e4d9b1806e43fd04462de2`  
		Last Modified: Tue, 23 Aug 2022 02:36:44 GMT  
		Size: 4.9 MB (4944180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb6be5911b40ca548e48c10b09cb2312f1698b4c84f09711c69389a94b1a8be`  
		Last Modified: Tue, 23 Aug 2022 02:36:44 GMT  
		Size: 10.7 MB (10657442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db608c3c3ce3568556faf63acbc2069811afe242faf8992ccf0ab1986ee38e4f`  
		Last Modified: Tue, 23 Aug 2022 02:37:07 GMT  
		Size: 54.7 MB (54680886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:1afc200fb3ee2b4b85c5c984fbbc088ff53286077a843588bc04c935cd6b7416
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.1 MB (128053909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bceeed6ce487fd59052390091c5f4300ff05ada27c1650c1dbf83f91a4d9788b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:24 GMT
ADD file:4012c41187a03bdb3d37bec80f6255a1d46582e3ed145b4f313e42196529e524 in / 
# Tue, 23 Aug 2022 01:02:25 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:31:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:31:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:32:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6f683b9c66ef80b527ee5e4cb11969c6e0c1400ab69a4f1279af90f5766d70c7`  
		Last Modified: Tue, 23 Aug 2022 01:07:53 GMT  
		Size: 56.0 MB (56012624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f506948c8aa6d2e0693b583a388ce5e10b4393763bd2ea2529af3bfaa07f0c92`  
		Last Modified: Tue, 23 Aug 2022 01:40:01 GMT  
		Size: 5.1 MB (5085725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915cb3138c0c978b1806934d3f979cff24ecaed321fe7e13caa292cf9ca73dcc`  
		Last Modified: Tue, 23 Aug 2022 01:40:01 GMT  
		Size: 11.0 MB (11032841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc001487b6a15d61b32ac2dbd4b06bdede894077b8fcd3fa2f3969f98052bc3`  
		Last Modified: Tue, 23 Aug 2022 01:40:24 GMT  
		Size: 55.9 MB (55922719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:c8f075c6f8d978558f03a94da80ad547aa3e8af5a92a9b3d461d8db9b40542bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122156831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fdba3c8b6471cc9b1138ee1a4111402f4476b568b1735d38c33912c379db3b3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:10:38 GMT
ADD file:a55d19f262e8338f932ce871c1cbc1718f9f74a5002212f38fea74f3858460a9 in / 
# Tue, 23 Aug 2022 00:10:43 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 22:24:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 22:24:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 22:26:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5ce438ccc597187e8a0dab5cc8906e6a0ec75a9320e55225ad2ec24765f7c0b4`  
		Last Modified: Tue, 23 Aug 2022 00:18:51 GMT  
		Size: 53.3 MB (53272999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567ecdfd8aa8d0bdcecff06b6b73dfbde6ae5451a3afec2a33aee7ca527b61e9`  
		Last Modified: Tue, 23 Aug 2022 22:49:03 GMT  
		Size: 4.9 MB (4918268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9374a0689765aeaeee15bb1c011bddd8cb323e6002385ceb42952a14d3210410`  
		Last Modified: Tue, 23 Aug 2022 22:49:06 GMT  
		Size: 10.7 MB (10661281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ccffd65aa7de17818aaae93c681cc96ca65baf5ab87b1989328259e139d360d`  
		Last Modified: Tue, 23 Aug 2022 22:49:57 GMT  
		Size: 53.3 MB (53304283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:cb31310b3598fc3d3ad9daa40df9a133a6e2e360aee409d29191203c4686d095
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134816917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30881ed3045278b91be936aafc665ff71cd8bc93d39d8b69650de485729b3d02`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:24:30 GMT
ADD file:c498f58d8dc50a2a20679642be8f6f43de8b79455438a1c237ef4c94a9ffe34c in / 
# Tue, 23 Aug 2022 01:24:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:58:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:59:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:62d01a7bda469557451a05bab1d4de7f53dd936e8032b36635019fd54cd927e4`  
		Last Modified: Tue, 23 Aug 2022 01:29:57 GMT  
		Size: 58.9 MB (58909173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b002340b938f821f3b0978eb9bfc47d2b8fe91b33c50508bd618c3c4b0ffe0`  
		Last Modified: Tue, 23 Aug 2022 02:10:43 GMT  
		Size: 5.4 MB (5412576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c65f43f4fd248e0fd18c35535f21fcafa740bdde05c5c367f32926f478e55f`  
		Last Modified: Tue, 23 Aug 2022 02:10:44 GMT  
		Size: 11.6 MB (11628949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6e7f52d8f52b4e830cdd20f538730eebe893f6c1f11aac1d0457ae132da2e8`  
		Last Modified: Tue, 23 Aug 2022 02:11:16 GMT  
		Size: 58.9 MB (58866219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:fe781f689e6f87bbf043328a5546a3c8810e4bb71bf4aace341aa84bc8e2aab4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123246645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd05daa086ec2eb9eb0d8724cfebe627e1a621d31c39e41c49c480e60b4413fd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:53:42 GMT
ADD file:799d2eac4bf12dcb56eca0b771da879e8873a2a81b4d74520db7d6665d448ff6 in / 
# Tue, 23 Aug 2022 00:53:45 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 09:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 09:51:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 09:51:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e8428caa8cb9dd5cd48266f588e1d935181b0d75e5f4680a9d4d03700d44289`  
		Last Modified: Tue, 23 Aug 2022 01:01:15 GMT  
		Size: 53.3 MB (53279185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b41fe9abb9a7707d3bfd9881e997384ad70ba3f811c4152a16e11585318bd5`  
		Last Modified: Tue, 23 Aug 2022 09:59:58 GMT  
		Size: 5.1 MB (5146782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0215c1024f20ea76e1b536fcf226d87a639e72806443621a0bf52a719c0218fd`  
		Last Modified: Tue, 23 Aug 2022 09:59:59 GMT  
		Size: 10.8 MB (10765873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aeff4b644e5176d180f566f9889b6ed12e443f2fb955b119865cc113d26c3b1`  
		Last Modified: Tue, 23 Aug 2022 10:00:19 GMT  
		Size: 54.1 MB (54054805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:sid`

```console
$ docker pull buildpack-deps@sha256:8e69463fa7226b65fb3a87f7f7078af656db7fd85bf186caedee6d2ae574aacb
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
$ docker pull buildpack-deps@sha256:82d0d6d789a9d69e6ccfb63feae242155bb785aabec9d1e662cd8fc14bb54548
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **555.9 MB (555872054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9a609cc81c34f54d9832c5a0065808f39e2800dc81394bbdc99d0e1c4105fc7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:39 GMT
ADD file:0ded1ec762355d6c32b4a9f1eff5fbd5e60d15824d6bde678ef85cbdd03fe0ce in / 
# Tue, 23 Aug 2022 00:21:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:50:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:51:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 00:51:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:52:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6649fedb76d916c1041e321eca86994acdb4cd14cc61ef93b5d2a397c15af4ad`  
		Last Modified: Tue, 23 Aug 2022 00:26:41 GMT  
		Size: 52.8 MB (52768784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52383a4258951f21b40d1c18a5c708ecfd3cc7f76838fc8fbe3c1fa248f7b133`  
		Last Modified: Tue, 23 Aug 2022 00:57:51 GMT  
		Size: 9.3 MB (9302218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b8bf82596b529ddf3a818d599c3bed1bef1e54925ac4df0a1a6bf6467ce1bd2`  
		Last Modified: Tue, 23 Aug 2022 00:57:51 GMT  
		Size: 11.3 MB (11274041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f934be4bad0fbf951546a8aaa20f158e16a48d2a373a3b5cab06448c354bae14`  
		Last Modified: Tue, 23 Aug 2022 00:58:09 GMT  
		Size: 58.1 MB (58057519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a459942b0771eb68ff654a202259ff2306d2ca50d850f5595b425216a794380`  
		Last Modified: Tue, 23 Aug 2022 00:59:13 GMT  
		Size: 424.5 MB (424469492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:ae6debf772cd416d3418020d444b526e6dbb85caf44ec3d847d6ece14fdddbd5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.9 MB (313920314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:346d312be574d74cdc36cf1bba138bd96a787ab9df0c21436f66850af54f9485`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:17:35 GMT
ADD file:dd3257a03b58fae4238ad4fccb1c79ff49c76b1294f5fb6f57ecee4bb748c9ca in / 
# Tue, 23 Aug 2022 01:17:35 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 06:21:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 06:21:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 06:22:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 06:23:24 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4cd09bc891cabc28c38273b3b8e22a810888bfc449c6fd4ec5610c27492b2603`  
		Last Modified: Tue, 23 Aug 2022 01:23:14 GMT  
		Size: 51.9 MB (51911406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f224d9458f88dbd5a7ba922c9cb4a7116b314d234615e7981e233157663a02`  
		Last Modified: Tue, 23 Aug 2022 06:28:49 GMT  
		Size: 9.7 MB (9741837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f3836f63f5d9bf55c4350c9f89c9a7b420aa71f6408278b53d58e61634cb3fa`  
		Last Modified: Tue, 23 Aug 2022 06:28:49 GMT  
		Size: 10.9 MB (10949073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c127ba25c98f2eef6419ecfbb5bb63c8da103c1ea0298e7e61e2103424e530a`  
		Last Modified: Tue, 23 Aug 2022 06:29:16 GMT  
		Size: 55.7 MB (55747826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e249ad29978f097d481f4bfe9ce42ca0c44552bf26944aea2b847496fd0838`  
		Last Modified: Tue, 23 Aug 2022 06:30:09 GMT  
		Size: 185.6 MB (185570172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:fd0b31ddb28465a985e9b4e90815a6fa47d188e9408ecf7c3d5c831fcfc241dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.8 MB (299844414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72da89b2937b052cd65b23069be33ca9069f1824886bb639b596cf2a764aecb3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:44:30 GMT
ADD file:63335401d9730857a474088e836b58820d062d53a4d008379a3f0bab91891ee7 in / 
# Tue, 23 Aug 2022 01:44:30 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 13:04:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:04:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 13:04:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:05:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:abce9a6a026c05f336d24d7c79af29d2f108767252a4737864125c7cd16cb946`  
		Last Modified: Tue, 23 Aug 2022 01:52:08 GMT  
		Size: 49.6 MB (49637416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:789e63ee7b15faa5255a98e78ca57f7b79165de31d27f0d20a810e2e8f2f6fbe`  
		Last Modified: Tue, 23 Aug 2022 13:15:09 GMT  
		Size: 8.4 MB (8404984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866f5f3461f124a4ec2d43c116d5e4f8a2783872d85516deec64b8873fb850ab`  
		Last Modified: Tue, 23 Aug 2022 13:15:09 GMT  
		Size: 10.6 MB (10590651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519438e1fee2b230fe7b1ef7d878f221dfd76d39406a621b5ac5c6a6d9977d8d`  
		Last Modified: Tue, 23 Aug 2022 13:15:36 GMT  
		Size: 53.7 MB (53721931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116396eb184bdf4a369bbff811214de4b5044eb77672394f3d62ce8fd8b07b69`  
		Last Modified: Tue, 23 Aug 2022 13:16:25 GMT  
		Size: 177.5 MB (177489432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:bcb381e04a2732ab250a0bc43cf4a8661b7020a0b532d7bfd5bcfdd5b4366c62
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **545.4 MB (545439369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18475cf95c9af1adee7cf3b17f92a8afed4f8d29ce264fe5b1d9f71f49b05775`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:53:33 GMT
ADD file:03a6abbfc4f7f5b036b595b68d32dab2760788223365adbadd691cc6b97d3f9f in / 
# Tue, 23 Aug 2022 01:53:34 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:30:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:30:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 02:31:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:32:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11a10710f625b85736b19b89ebf063edde4e3f2dedab0a6cc94db39e134d8cfe`  
		Last Modified: Tue, 23 Aug 2022 01:59:52 GMT  
		Size: 53.2 MB (53220635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d52438f7d6f6695685610119446105c5c9522703362332bff254bc8eda29485`  
		Last Modified: Tue, 23 Aug 2022 02:39:08 GMT  
		Size: 9.1 MB (9135715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c781af42aca050a89e2c2b2ae998b642dd1e62096b74d1479568d49d2b43581`  
		Last Modified: Tue, 23 Aug 2022 02:39:08 GMT  
		Size: 11.1 MB (11058895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b655e4c924d786599e6214f6298b4a90d6bb1e4e1bc66096185648662d73d55`  
		Last Modified: Tue, 23 Aug 2022 02:39:29 GMT  
		Size: 57.9 MB (57942074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4468d1c3ff674531ee48a976061d1c38abad49092b9887b6d908ec3376e65abc`  
		Last Modified: Tue, 23 Aug 2022 02:40:35 GMT  
		Size: 414.1 MB (414082050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8cd9f265050b2a89f2b0e789b66ee74878574934646dae66d370dbb1631b95b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.1 MB (349084797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6f5e1d87a25966aa07a6b1a0ddb507d3f52fec56499334037cc0df2fff4cf09`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:03:44 GMT
ADD file:56a765ed5b9c59576a105c4e82da61f928406a2ef950e7cada80b5c269a1acda in / 
# Tue, 23 Aug 2022 01:03:44 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:35:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:35:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:36:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:37:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:05690d5133887cdda89e6ae4808c08e8a92acf2163ce992d8bacbed497b1ddd7`  
		Last Modified: Tue, 23 Aug 2022 01:10:25 GMT  
		Size: 54.1 MB (54133693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6de5521fae7f54e276230f1136f3c889618c53b37f387bcb06db2c09c9ea96`  
		Last Modified: Tue, 23 Aug 2022 01:42:35 GMT  
		Size: 9.5 MB (9480147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1ad46fde87250408a791d37517179cd6427cd46421e84e138f00437a005cc8`  
		Last Modified: Tue, 23 Aug 2022 01:42:35 GMT  
		Size: 11.5 MB (11473735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc96324d4abcfddd315fc320b0f834fa9ab7e220e914962ae1d8af8c95bc0b94`  
		Last Modified: Tue, 23 Aug 2022 01:42:56 GMT  
		Size: 59.7 MB (59690126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3314db2a67edcee49b0f6254dd94eccdab07b0b303150ecab178769c20454ef8`  
		Last Modified: Tue, 23 Aug 2022 01:43:32 GMT  
		Size: 214.3 MB (214307096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:44932d5ac5c7c5b4769849503ca026630ef64ad261f181908e37e315f4a6a562
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.8 MB (321764495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aaf48cd27b846d1c74c094bed63d9fc6bdcad9711050ce213db2592c1f435d3f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:11:52 GMT
ADD file:372730632835dde60a084d1dc5d1d8d7840a118d3aa6413f1568d2a939e39e05 in / 
# Tue, 23 Aug 2022 00:11:58 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 22:34:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 22:34:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 22:36:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 22:42:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f6fdf476c348ab651944f6f008015e5c5184fa9f5620904fc65599b044dd5761`  
		Last Modified: Tue, 23 Aug 2022 00:20:20 GMT  
		Size: 53.2 MB (53216630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f889c0bad3c21c23d5613d840cb6194f047e7bd8b0ab913aa4c3aeb3f22ff6aa`  
		Last Modified: Tue, 23 Aug 2022 22:52:22 GMT  
		Size: 8.7 MB (8666700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e682c1b586301933075fc1a74ded2cb91e71a70eb9e075ab5291aec1d56e833`  
		Last Modified: Tue, 23 Aug 2022 22:52:22 GMT  
		Size: 11.0 MB (11041861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec7b75657e271145b112803a3b136f6eba775667758887ede8d7bf5eea806dd`  
		Last Modified: Tue, 23 Aug 2022 22:53:13 GMT  
		Size: 56.9 MB (56881826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ccde40f554bb70ef53d85d915e58944b5bde8dea04124f47de1cc710a908bde`  
		Last Modified: Tue, 23 Aug 2022 22:55:22 GMT  
		Size: 192.0 MB (191957478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d31682460f32ab995f6123d1861469234e2e9cec6e306c62c4947a3ae5e3d32c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **553.9 MB (553947352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e93f9fd28ad6ce94afa2ae176b65b01afb61979bba69a588a1f8caa26f8dc039`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:25:10 GMT
ADD file:7b8a9c1fc05e75d845ea719c57047ae432cceb7645d270a99b117d0e4e0ffb33 in / 
# Tue, 23 Aug 2022 01:25:13 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:02:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:02:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 02:02:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:05:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:515f00ecba82250b75d6d9987193afd77293c07bfaf7a95ae024c05c73a8cb3a`  
		Last Modified: Tue, 23 Aug 2022 01:31:07 GMT  
		Size: 57.3 MB (57313882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759d55c9749119adb9c0cff41513f89896055da109781a9c493c462426691120`  
		Last Modified: Tue, 23 Aug 2022 02:12:40 GMT  
		Size: 9.9 MB (9892227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419401365d91198049a8c6620087ce51a751ce8891e8a184d06c31216b0773b8`  
		Last Modified: Tue, 23 Aug 2022 02:12:40 GMT  
		Size: 12.1 MB (12081297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e6911c1af381860ef781b5463a576d34cf58ff5ca18e69333ab7d054a1d2a4`  
		Last Modified: Tue, 23 Aug 2022 02:13:10 GMT  
		Size: 62.9 MB (62860983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d3b983d1afeef2ed30145913f73fdca87605ede854ebf973821980ed7bb889`  
		Last Modified: Tue, 23 Aug 2022 02:14:53 GMT  
		Size: 411.8 MB (411798963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:89615e24846bec4e9c2210ffa40781e7fe3b0bb100785fb53d9f3d9771959639
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.2 MB (355224975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64060694992efd7dc9bad5501308cc2bafe39fcf7438d5a09721771171d1ed27`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:12:03 GMT
ADD file:beb3c4d0f1887ccbbe2b266a156b7658d2e1d7d48cbcd416a0410554dfafdf12 in / 
# Tue, 23 Aug 2022 00:12:06 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:58:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:59:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:03:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:12:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11998c1ffc96119253ef35ecbcfd66c2cb0d69f51a294f603a54496ec02d329c`  
		Last Modified: Tue, 23 Aug 2022 00:30:27 GMT  
		Size: 49.3 MB (49268189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237ee2e31cf68d3cd2675680cbf1e3c574c76f74440375dc1b8c1ad1d3d9768e`  
		Last Modified: Tue, 23 Aug 2022 01:41:12 GMT  
		Size: 8.4 MB (8399080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69eb487c5f4d1ba65732a0b11d3a69780177b7ed0357581fce4eb347813a643`  
		Last Modified: Tue, 23 Aug 2022 01:41:12 GMT  
		Size: 10.7 MB (10659901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3572ed314e6c0604916ece49e3a546ec2fcc60391daae870152b56b8fdc14d98`  
		Last Modified: Tue, 23 Aug 2022 01:43:43 GMT  
		Size: 54.0 MB (54034717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a20268cb682347428f2402e200fcf1a6f64026d72fa43eb8b171c47218c4e398`  
		Last Modified: Tue, 23 Aug 2022 01:51:06 GMT  
		Size: 232.9 MB (232863088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3380f5eb469b98e12046ee103b120a9bc84afb65a17f38812751e1b32fd6da22
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **499.2 MB (499173410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76a19518653a77d77c1c607b119f24c614cdd67c4fdc9f27f4385f192cc0ed7a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:54:14 GMT
ADD file:fb4926c73b650f18bc1eb6b58287dc0872251073fd0bc72bcd007f74315f89a5 in / 
# Tue, 23 Aug 2022 00:54:17 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 09:53:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 09:53:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 09:53:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 09:55:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0aaf3bb8cf1626ddbd85331fa1967c48ccf9d314270b99a2a506e53979592f79`  
		Last Modified: Tue, 23 Aug 2022 01:06:53 GMT  
		Size: 51.6 MB (51581993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b9f9f1f0cb3b7d4b45cdcacf5c7c93102c09bc71207f7dcc091136f732a622`  
		Last Modified: Tue, 23 Aug 2022 10:01:01 GMT  
		Size: 8.9 MB (8943771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06f6fca0053787f32630628512d8ae3f948e6ae085840b8a4083d3ac745fa220`  
		Last Modified: Tue, 23 Aug 2022 10:01:01 GMT  
		Size: 11.2 MB (11168320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e0960b87cafae9e1bf612df6c73bfb7680cbb0139fd149d5c6e367e797b282`  
		Last Modified: Tue, 23 Aug 2022 10:01:16 GMT  
		Size: 57.2 MB (57210664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886ef7d8187dc34f74cbea7c999fbf59f6940f6f469d36dc12cf47527ef36d7a`  
		Last Modified: Tue, 23 Aug 2022 10:02:03 GMT  
		Size: 370.3 MB (370268662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:2c2b158aa817c9ae49deea0883bdabc17121d369094e2fed9ee04fc774bf96e8
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
$ docker pull buildpack-deps@sha256:12348240e5db18afa70f6382420fb3e36194a640ffa7f21e5506ded546ce702b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.3 MB (73345043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:801581c78b136e899df5cbff068467129f0d26f6e4add3126d2743694757cdae`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:39 GMT
ADD file:0ded1ec762355d6c32b4a9f1eff5fbd5e60d15824d6bde678ef85cbdd03fe0ce in / 
# Tue, 23 Aug 2022 00:21:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:50:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:51:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6649fedb76d916c1041e321eca86994acdb4cd14cc61ef93b5d2a397c15af4ad`  
		Last Modified: Tue, 23 Aug 2022 00:26:41 GMT  
		Size: 52.8 MB (52768784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52383a4258951f21b40d1c18a5c708ecfd3cc7f76838fc8fbe3c1fa248f7b133`  
		Last Modified: Tue, 23 Aug 2022 00:57:51 GMT  
		Size: 9.3 MB (9302218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b8bf82596b529ddf3a818d599c3bed1bef1e54925ac4df0a1a6bf6467ce1bd2`  
		Last Modified: Tue, 23 Aug 2022 00:57:51 GMT  
		Size: 11.3 MB (11274041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:7e705bb79460fdbd230d3b523f243f8fa47269ea192646175d4ec2f6b702919a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.6 MB (72602316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e605e3949595a62e6b4bf7d42c0fba0c62626c32603d8f5140d390cbf511380`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:17:35 GMT
ADD file:dd3257a03b58fae4238ad4fccb1c79ff49c76b1294f5fb6f57ecee4bb748c9ca in / 
# Tue, 23 Aug 2022 01:17:35 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 06:21:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 06:21:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4cd09bc891cabc28c38273b3b8e22a810888bfc449c6fd4ec5610c27492b2603`  
		Last Modified: Tue, 23 Aug 2022 01:23:14 GMT  
		Size: 51.9 MB (51911406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f224d9458f88dbd5a7ba922c9cb4a7116b314d234615e7981e233157663a02`  
		Last Modified: Tue, 23 Aug 2022 06:28:49 GMT  
		Size: 9.7 MB (9741837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f3836f63f5d9bf55c4350c9f89c9a7b420aa71f6408278b53d58e61634cb3fa`  
		Last Modified: Tue, 23 Aug 2022 06:28:49 GMT  
		Size: 10.9 MB (10949073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f43c56203997827c84a812462131cbcabc3e4c180f62c92a48595e4fcb79d54d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.6 MB (68633051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b20f50e4edf8c204581294078d6e224f677aad50fc3c310742b2ecb5b6bc19d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:44:30 GMT
ADD file:63335401d9730857a474088e836b58820d062d53a4d008379a3f0bab91891ee7 in / 
# Tue, 23 Aug 2022 01:44:30 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 13:04:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:04:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:abce9a6a026c05f336d24d7c79af29d2f108767252a4737864125c7cd16cb946`  
		Last Modified: Tue, 23 Aug 2022 01:52:08 GMT  
		Size: 49.6 MB (49637416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:789e63ee7b15faa5255a98e78ca57f7b79165de31d27f0d20a810e2e8f2f6fbe`  
		Last Modified: Tue, 23 Aug 2022 13:15:09 GMT  
		Size: 8.4 MB (8404984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866f5f3461f124a4ec2d43c116d5e4f8a2783872d85516deec64b8873fb850ab`  
		Last Modified: Tue, 23 Aug 2022 13:15:09 GMT  
		Size: 10.6 MB (10590651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7111671eb5e0eef153034060931fed251bc35454d67eaef764d41b8418bd55ea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.4 MB (73415245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da1f6b44edf551616f54c76b94273bb6cf38ac811641321690130bd55af523ff`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:53:33 GMT
ADD file:03a6abbfc4f7f5b036b595b68d32dab2760788223365adbadd691cc6b97d3f9f in / 
# Tue, 23 Aug 2022 01:53:34 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:30:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:30:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:11a10710f625b85736b19b89ebf063edde4e3f2dedab0a6cc94db39e134d8cfe`  
		Last Modified: Tue, 23 Aug 2022 01:59:52 GMT  
		Size: 53.2 MB (53220635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d52438f7d6f6695685610119446105c5c9522703362332bff254bc8eda29485`  
		Last Modified: Tue, 23 Aug 2022 02:39:08 GMT  
		Size: 9.1 MB (9135715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c781af42aca050a89e2c2b2ae998b642dd1e62096b74d1479568d49d2b43581`  
		Last Modified: Tue, 23 Aug 2022 02:39:08 GMT  
		Size: 11.1 MB (11058895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:b9972c98ff602f317e6304009068bc0bcfd55766be4faadef16a50f2e560ac0c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75087575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be006906138be6be28f63d53b6777210491d213b2fd95065a1fd6ca582699aad`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:03:44 GMT
ADD file:56a765ed5b9c59576a105c4e82da61f928406a2ef950e7cada80b5c269a1acda in / 
# Tue, 23 Aug 2022 01:03:44 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:35:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:35:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:05690d5133887cdda89e6ae4808c08e8a92acf2163ce992d8bacbed497b1ddd7`  
		Last Modified: Tue, 23 Aug 2022 01:10:25 GMT  
		Size: 54.1 MB (54133693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6de5521fae7f54e276230f1136f3c889618c53b37f387bcb06db2c09c9ea96`  
		Last Modified: Tue, 23 Aug 2022 01:42:35 GMT  
		Size: 9.5 MB (9480147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1ad46fde87250408a791d37517179cd6427cd46421e84e138f00437a005cc8`  
		Last Modified: Tue, 23 Aug 2022 01:42:35 GMT  
		Size: 11.5 MB (11473735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:d3bb18f79fd404a72bba015d8e68e173f0847657b212851c7a0f5d1b220fc766
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72925191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19c1d92b28bfc5686ba778c734dd92a01728841f6f7752e82c98666ac2c064eb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:11:52 GMT
ADD file:372730632835dde60a084d1dc5d1d8d7840a118d3aa6413f1568d2a939e39e05 in / 
# Tue, 23 Aug 2022 00:11:58 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 22:34:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 22:34:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f6fdf476c348ab651944f6f008015e5c5184fa9f5620904fc65599b044dd5761`  
		Last Modified: Tue, 23 Aug 2022 00:20:20 GMT  
		Size: 53.2 MB (53216630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f889c0bad3c21c23d5613d840cb6194f047e7bd8b0ab913aa4c3aeb3f22ff6aa`  
		Last Modified: Tue, 23 Aug 2022 22:52:22 GMT  
		Size: 8.7 MB (8666700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e682c1b586301933075fc1a74ded2cb91e71a70eb9e075ab5291aec1d56e833`  
		Last Modified: Tue, 23 Aug 2022 22:52:22 GMT  
		Size: 11.0 MB (11041861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:9976e80bc902f0a0e9be54ffe69853a518388672975e91a0dbca9cc51685422b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.3 MB (79287406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a04e630b9a2c28f96e8087ed577aa1796b005fda82c5be6b82cc21d1cfc58d35`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:25:10 GMT
ADD file:7b8a9c1fc05e75d845ea719c57047ae432cceb7645d270a99b117d0e4e0ffb33 in / 
# Tue, 23 Aug 2022 01:25:13 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:02:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:02:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:515f00ecba82250b75d6d9987193afd77293c07bfaf7a95ae024c05c73a8cb3a`  
		Last Modified: Tue, 23 Aug 2022 01:31:07 GMT  
		Size: 57.3 MB (57313882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759d55c9749119adb9c0cff41513f89896055da109781a9c493c462426691120`  
		Last Modified: Tue, 23 Aug 2022 02:12:40 GMT  
		Size: 9.9 MB (9892227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419401365d91198049a8c6620087ce51a751ce8891e8a184d06c31216b0773b8`  
		Last Modified: Tue, 23 Aug 2022 02:12:40 GMT  
		Size: 12.1 MB (12081297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:7190f1576496c38d326bf20b45a9725d2c7888724774b79fa03f1ad5fdb68d29
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68327170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cbcd3644b4a571e4579adbe4eb08af38c965c5986789fdd1a493de8456457e7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:12:03 GMT
ADD file:beb3c4d0f1887ccbbe2b266a156b7658d2e1d7d48cbcd416a0410554dfafdf12 in / 
# Tue, 23 Aug 2022 00:12:06 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:58:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:59:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:11998c1ffc96119253ef35ecbcfd66c2cb0d69f51a294f603a54496ec02d329c`  
		Last Modified: Tue, 23 Aug 2022 00:30:27 GMT  
		Size: 49.3 MB (49268189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237ee2e31cf68d3cd2675680cbf1e3c574c76f74440375dc1b8c1ad1d3d9768e`  
		Last Modified: Tue, 23 Aug 2022 01:41:12 GMT  
		Size: 8.4 MB (8399080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69eb487c5f4d1ba65732a0b11d3a69780177b7ed0357581fce4eb347813a643`  
		Last Modified: Tue, 23 Aug 2022 01:41:12 GMT  
		Size: 10.7 MB (10659901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:50db63bb1dd307a64611a08c3833204bb5702151e0f7d673c4f54195b8df8703
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.7 MB (71694084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d47eb8f13f6cb432056c3dcae6141ef753599747fb62444f57a70249abe219a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:54:14 GMT
ADD file:fb4926c73b650f18bc1eb6b58287dc0872251073fd0bc72bcd007f74315f89a5 in / 
# Tue, 23 Aug 2022 00:54:17 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 09:53:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 09:53:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0aaf3bb8cf1626ddbd85331fa1967c48ccf9d314270b99a2a506e53979592f79`  
		Last Modified: Tue, 23 Aug 2022 01:06:53 GMT  
		Size: 51.6 MB (51581993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b9f9f1f0cb3b7d4b45cdcacf5c7c93102c09bc71207f7dcc091136f732a622`  
		Last Modified: Tue, 23 Aug 2022 10:01:01 GMT  
		Size: 8.9 MB (8943771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06f6fca0053787f32630628512d8ae3f948e6ae085840b8a4083d3ac745fa220`  
		Last Modified: Tue, 23 Aug 2022 10:01:01 GMT  
		Size: 11.2 MB (11168320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:sid-scm`

```console
$ docker pull buildpack-deps@sha256:25fb1b2c0fe84aea81ddd7f0198b4230e3d91d45d975200e2360f8d7ae5d0299
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
$ docker pull buildpack-deps@sha256:f6ff780ff6d9dd4454e7164151b28d72f3fcf1bba471138ce4e1f431bd71e0fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131402562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc7f6c028fa86c7a1118b95cde5cb96316d9cacaa46a358a82613050902e582f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:39 GMT
ADD file:0ded1ec762355d6c32b4a9f1eff5fbd5e60d15824d6bde678ef85cbdd03fe0ce in / 
# Tue, 23 Aug 2022 00:21:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:50:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:51:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 00:51:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6649fedb76d916c1041e321eca86994acdb4cd14cc61ef93b5d2a397c15af4ad`  
		Last Modified: Tue, 23 Aug 2022 00:26:41 GMT  
		Size: 52.8 MB (52768784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52383a4258951f21b40d1c18a5c708ecfd3cc7f76838fc8fbe3c1fa248f7b133`  
		Last Modified: Tue, 23 Aug 2022 00:57:51 GMT  
		Size: 9.3 MB (9302218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b8bf82596b529ddf3a818d599c3bed1bef1e54925ac4df0a1a6bf6467ce1bd2`  
		Last Modified: Tue, 23 Aug 2022 00:57:51 GMT  
		Size: 11.3 MB (11274041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f934be4bad0fbf951546a8aaa20f158e16a48d2a373a3b5cab06448c354bae14`  
		Last Modified: Tue, 23 Aug 2022 00:58:09 GMT  
		Size: 58.1 MB (58057519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:828273289b0de4086367b7a3b69cf9cc5c9b5626734cbe7a0f443b9cd4a7e17f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128350142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7a2de47491cc492dfcb63ab018b93f64814b3df048f39124c93f004890e9816`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:17:35 GMT
ADD file:dd3257a03b58fae4238ad4fccb1c79ff49c76b1294f5fb6f57ecee4bb748c9ca in / 
# Tue, 23 Aug 2022 01:17:35 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 06:21:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 06:21:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 06:22:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4cd09bc891cabc28c38273b3b8e22a810888bfc449c6fd4ec5610c27492b2603`  
		Last Modified: Tue, 23 Aug 2022 01:23:14 GMT  
		Size: 51.9 MB (51911406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f224d9458f88dbd5a7ba922c9cb4a7116b314d234615e7981e233157663a02`  
		Last Modified: Tue, 23 Aug 2022 06:28:49 GMT  
		Size: 9.7 MB (9741837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f3836f63f5d9bf55c4350c9f89c9a7b420aa71f6408278b53d58e61634cb3fa`  
		Last Modified: Tue, 23 Aug 2022 06:28:49 GMT  
		Size: 10.9 MB (10949073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c127ba25c98f2eef6419ecfbb5bb63c8da103c1ea0298e7e61e2103424e530a`  
		Last Modified: Tue, 23 Aug 2022 06:29:16 GMT  
		Size: 55.7 MB (55747826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:fb4ae2b3214297ac6d789a817eb1f7610877481f6df43185bf978d295af721f2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.4 MB (122354982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:557ea0b235bd6f860583a55f4497eed0f630571ffe0b0f59f2ad807883bdf7fd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:44:30 GMT
ADD file:63335401d9730857a474088e836b58820d062d53a4d008379a3f0bab91891ee7 in / 
# Tue, 23 Aug 2022 01:44:30 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 13:04:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:04:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 13:04:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:abce9a6a026c05f336d24d7c79af29d2f108767252a4737864125c7cd16cb946`  
		Last Modified: Tue, 23 Aug 2022 01:52:08 GMT  
		Size: 49.6 MB (49637416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:789e63ee7b15faa5255a98e78ca57f7b79165de31d27f0d20a810e2e8f2f6fbe`  
		Last Modified: Tue, 23 Aug 2022 13:15:09 GMT  
		Size: 8.4 MB (8404984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866f5f3461f124a4ec2d43c116d5e4f8a2783872d85516deec64b8873fb850ab`  
		Last Modified: Tue, 23 Aug 2022 13:15:09 GMT  
		Size: 10.6 MB (10590651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519438e1fee2b230fe7b1ef7d878f221dfd76d39406a621b5ac5c6a6d9977d8d`  
		Last Modified: Tue, 23 Aug 2022 13:15:36 GMT  
		Size: 53.7 MB (53721931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:5a4db913aac724bda8dd2b3efd88e4f9a857398e53462cf785726255553e308d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131357319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3624daf2816b207400e142ee555d194f1d07f91d0a35b5c3171ebd64b7756427`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:53:33 GMT
ADD file:03a6abbfc4f7f5b036b595b68d32dab2760788223365adbadd691cc6b97d3f9f in / 
# Tue, 23 Aug 2022 01:53:34 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:30:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:30:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 02:31:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11a10710f625b85736b19b89ebf063edde4e3f2dedab0a6cc94db39e134d8cfe`  
		Last Modified: Tue, 23 Aug 2022 01:59:52 GMT  
		Size: 53.2 MB (53220635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d52438f7d6f6695685610119446105c5c9522703362332bff254bc8eda29485`  
		Last Modified: Tue, 23 Aug 2022 02:39:08 GMT  
		Size: 9.1 MB (9135715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c781af42aca050a89e2c2b2ae998b642dd1e62096b74d1479568d49d2b43581`  
		Last Modified: Tue, 23 Aug 2022 02:39:08 GMT  
		Size: 11.1 MB (11058895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b655e4c924d786599e6214f6298b4a90d6bb1e4e1bc66096185648662d73d55`  
		Last Modified: Tue, 23 Aug 2022 02:39:29 GMT  
		Size: 57.9 MB (57942074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:f05820f89144ef9fd4abdfa7b091a362e96a5babc1bd7fdded96cbb6445f5d8a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134777701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6899c125d79e1d6f8e0f13938a0ff7560906f0008d90fe875828e8d43f0015c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:03:44 GMT
ADD file:56a765ed5b9c59576a105c4e82da61f928406a2ef950e7cada80b5c269a1acda in / 
# Tue, 23 Aug 2022 01:03:44 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:35:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:35:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:36:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:05690d5133887cdda89e6ae4808c08e8a92acf2163ce992d8bacbed497b1ddd7`  
		Last Modified: Tue, 23 Aug 2022 01:10:25 GMT  
		Size: 54.1 MB (54133693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6de5521fae7f54e276230f1136f3c889618c53b37f387bcb06db2c09c9ea96`  
		Last Modified: Tue, 23 Aug 2022 01:42:35 GMT  
		Size: 9.5 MB (9480147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1ad46fde87250408a791d37517179cd6427cd46421e84e138f00437a005cc8`  
		Last Modified: Tue, 23 Aug 2022 01:42:35 GMT  
		Size: 11.5 MB (11473735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc96324d4abcfddd315fc320b0f834fa9ab7e220e914962ae1d8af8c95bc0b94`  
		Last Modified: Tue, 23 Aug 2022 01:42:56 GMT  
		Size: 59.7 MB (59690126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:4e25ae1bf979ce1f69096bcd3e8f9ac3b8c550a178e0af25ae5a182daf2b0f54
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.8 MB (129807017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2ddf6775bb37c49535b4cb27950a7b00495f73c343f2e41f1a1a773c7d713b8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:11:52 GMT
ADD file:372730632835dde60a084d1dc5d1d8d7840a118d3aa6413f1568d2a939e39e05 in / 
# Tue, 23 Aug 2022 00:11:58 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 22:34:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 22:34:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 22:36:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f6fdf476c348ab651944f6f008015e5c5184fa9f5620904fc65599b044dd5761`  
		Last Modified: Tue, 23 Aug 2022 00:20:20 GMT  
		Size: 53.2 MB (53216630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f889c0bad3c21c23d5613d840cb6194f047e7bd8b0ab913aa4c3aeb3f22ff6aa`  
		Last Modified: Tue, 23 Aug 2022 22:52:22 GMT  
		Size: 8.7 MB (8666700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e682c1b586301933075fc1a74ded2cb91e71a70eb9e075ab5291aec1d56e833`  
		Last Modified: Tue, 23 Aug 2022 22:52:22 GMT  
		Size: 11.0 MB (11041861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec7b75657e271145b112803a3b136f6eba775667758887ede8d7bf5eea806dd`  
		Last Modified: Tue, 23 Aug 2022 22:53:13 GMT  
		Size: 56.9 MB (56881826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:2b57718c40c4dfbfea62c154561c7314a5707ffbcf1dcc3f8f7974ed65dd3a89
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.1 MB (142148389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb381662ef1287437ee731fea51ff6067edeae2ec813e3a8b51449c3e83feeb5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:25:10 GMT
ADD file:7b8a9c1fc05e75d845ea719c57047ae432cceb7645d270a99b117d0e4e0ffb33 in / 
# Tue, 23 Aug 2022 01:25:13 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:02:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:02:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 02:02:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:515f00ecba82250b75d6d9987193afd77293c07bfaf7a95ae024c05c73a8cb3a`  
		Last Modified: Tue, 23 Aug 2022 01:31:07 GMT  
		Size: 57.3 MB (57313882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759d55c9749119adb9c0cff41513f89896055da109781a9c493c462426691120`  
		Last Modified: Tue, 23 Aug 2022 02:12:40 GMT  
		Size: 9.9 MB (9892227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419401365d91198049a8c6620087ce51a751ce8891e8a184d06c31216b0773b8`  
		Last Modified: Tue, 23 Aug 2022 02:12:40 GMT  
		Size: 12.1 MB (12081297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e6911c1af381860ef781b5463a576d34cf58ff5ca18e69333ab7d054a1d2a4`  
		Last Modified: Tue, 23 Aug 2022 02:13:10 GMT  
		Size: 62.9 MB (62860983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:ef05116e1aa3a68409adae7bc8bacbfc541ba80ea3cf9d4557f97931554d87b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.4 MB (122361887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f5da8a1feed0041190f96478c8ee800f1bd726c679e418e5a63f437c015ba7a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:12:03 GMT
ADD file:beb3c4d0f1887ccbbe2b266a156b7658d2e1d7d48cbcd416a0410554dfafdf12 in / 
# Tue, 23 Aug 2022 00:12:06 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:58:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:59:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:03:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11998c1ffc96119253ef35ecbcfd66c2cb0d69f51a294f603a54496ec02d329c`  
		Last Modified: Tue, 23 Aug 2022 00:30:27 GMT  
		Size: 49.3 MB (49268189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237ee2e31cf68d3cd2675680cbf1e3c574c76f74440375dc1b8c1ad1d3d9768e`  
		Last Modified: Tue, 23 Aug 2022 01:41:12 GMT  
		Size: 8.4 MB (8399080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69eb487c5f4d1ba65732a0b11d3a69780177b7ed0357581fce4eb347813a643`  
		Last Modified: Tue, 23 Aug 2022 01:41:12 GMT  
		Size: 10.7 MB (10659901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3572ed314e6c0604916ece49e3a546ec2fcc60391daae870152b56b8fdc14d98`  
		Last Modified: Tue, 23 Aug 2022 01:43:43 GMT  
		Size: 54.0 MB (54034717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:e90082389e99fc0e36884fc39fd1e58adf5ea389206304aeb314cd3bfcacbdde
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128904748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78d58a2c0b5135494685dd4ff3219ecacf7cdcb28a9f029b266828306d0a71fc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:54:14 GMT
ADD file:fb4926c73b650f18bc1eb6b58287dc0872251073fd0bc72bcd007f74315f89a5 in / 
# Tue, 23 Aug 2022 00:54:17 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 09:53:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 09:53:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 09:53:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0aaf3bb8cf1626ddbd85331fa1967c48ccf9d314270b99a2a506e53979592f79`  
		Last Modified: Tue, 23 Aug 2022 01:06:53 GMT  
		Size: 51.6 MB (51581993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b9f9f1f0cb3b7d4b45cdcacf5c7c93102c09bc71207f7dcc091136f732a622`  
		Last Modified: Tue, 23 Aug 2022 10:01:01 GMT  
		Size: 8.9 MB (8943771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06f6fca0053787f32630628512d8ae3f948e6ae085840b8a4083d3ac745fa220`  
		Last Modified: Tue, 23 Aug 2022 10:01:01 GMT  
		Size: 11.2 MB (11168320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e0960b87cafae9e1bf612df6c73bfb7680cbb0139fd149d5c6e367e797b282`  
		Last Modified: Tue, 23 Aug 2022 10:01:16 GMT  
		Size: 57.2 MB (57210664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stable`

```console
$ docker pull buildpack-deps@sha256:872ba70b0805b817db42d9ea75f066b5fe2be82d04d0dab69e41810edd9aa3f9
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
$ docker pull buildpack-deps@sha256:fdd46ac593b0dc4c54497b36e00e54c7759d068d9b9f014bd5b47bed430d4c2f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.4 MB (322416189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1966d2c176635cea14ac52f6a8a1d7d57101cb829eae63a9f3597cdee7a0ef6f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:40 GMT
ADD file:6944d322f4c04bd2192061822af5cbec8ac0a6b424c461d66174d32aed604972 in / 
# Tue, 23 Aug 2022 00:20:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:48:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:48:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 00:48:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:49:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1671565cc8df8c365c9b661d3fbc164e73d01f1b0430c6179588428f99a9da2e`  
		Last Modified: Tue, 23 Aug 2022 00:24:32 GMT  
		Size: 55.0 MB (55007555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e94d13e55e7a4ef17ff21376f57fb95c7e1706931f8704aa99260968d81f6e4`  
		Last Modified: Tue, 23 Aug 2022 00:55:37 GMT  
		Size: 5.2 MB (5163019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9c7528c685216129e8e67bf362a7702e7b1daa585ab85546a41508830657d6`  
		Last Modified: Tue, 23 Aug 2022 00:55:38 GMT  
		Size: 10.9 MB (10876472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ad072f9cd16fc8eb93b182b20e758e11acc0ef60babef0bf1043c08de1901a`  
		Last Modified: Tue, 23 Aug 2022 00:55:57 GMT  
		Size: 54.6 MB (54584135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b983117533b718374f1701ef593dd2afa6613c7908c6553be8e2a150e6448a`  
		Last Modified: Tue, 23 Aug 2022 00:56:35 GMT  
		Size: 196.8 MB (196785008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:48f086404ea033fe19fa0dd18cd1989c0b585f07c7353ff246098068b1075971
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.5 MB (295500312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:543ae8ede83fbb55855cee053b3a548534170a1c9e89ce34e227685abb1a46f2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:16:51 GMT
ADD file:132abd62c4fa546798c96d5b1f6f409de9ee27242caf6c479d65309b764c3ece in / 
# Tue, 23 Aug 2022 01:16:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 06:19:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 06:19:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 06:19:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 06:21:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1918e2afd901ca723b3483d8d521789daac45ddbaae2bf9fd813933e826f39b4`  
		Last Modified: Tue, 23 Aug 2022 01:22:10 GMT  
		Size: 52.5 MB (52547848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a58d3f469ed5c6be23bbc74a836bceb306e58e8cd5e58e4464c2b23519543a`  
		Last Modified: Tue, 23 Aug 2022 06:26:58 GMT  
		Size: 5.1 MB (5070690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61379bcded34629fad0582d1d42f2cba36b5f418591509e15301773304e7c7c0`  
		Last Modified: Tue, 23 Aug 2022 06:26:59 GMT  
		Size: 10.6 MB (10573758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c872e375903a379cc5ab82220655ab6973d82f8b48ab51b42d197a4ab189b6b`  
		Last Modified: Tue, 23 Aug 2022 06:27:30 GMT  
		Size: 52.3 MB (52320330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8993dbe2a09d90eb21f3d73a07f953f77bed210372ca285a9f7d8046891b8aa`  
		Last Modified: Tue, 23 Aug 2022 06:28:23 GMT  
		Size: 175.0 MB (174987686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:520bd48d184d2e1e72a3180fb98d6b1a72b711d77e12bcfb2dba659f40f40cc8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.0 MB (282979755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1d91ec2297d651816190904a39f4d4be0b91a78799a8484ab081b8081bd860d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:42:43 GMT
ADD file:21190c24a038c3c9de64b88797bf00e4c4319bd598c7c465cab2ca88d0502416 in / 
# Tue, 23 Aug 2022 01:42:43 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 12:59:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:00:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 13:00:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:01:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c715a126a4d5182c28d2d7b1c81de847bfbbacf6851819fef3eb28e3feb7db0e`  
		Last Modified: Tue, 23 Aug 2022 01:49:30 GMT  
		Size: 50.2 MB (50204931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cecc62e275236714359bda7d1f9c8412e8fa8539f3ef682eebd9c77986c927d`  
		Last Modified: Tue, 23 Aug 2022 13:11:58 GMT  
		Size: 4.9 MB (4930827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818eb872fe75602d611beeac0db63da0a4d8a67aee8b909d5114814f76446a5e`  
		Last Modified: Tue, 23 Aug 2022 13:11:59 GMT  
		Size: 10.2 MB (10217900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94cbc350f4a21916bb6fe70920c962a4889a5059aee86258e4d8263f0c7afbef`  
		Last Modified: Tue, 23 Aug 2022 13:12:28 GMT  
		Size: 50.3 MB (50342476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfc7e160811f0c470f91fe54fc02b224cb6ccbca07472ffcff55826d15bb26d`  
		Last Modified: Tue, 23 Aug 2022 13:13:20 GMT  
		Size: 167.3 MB (167283621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:6a657d9df2ce6540c05ceccaae91f294cb8ad870d9ea7cbc582a0642a5a8e0e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.7 MB (313684616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c31d31f8a9a1673a5b75dcc8e41518512dc0227c069e4cb4a48a9d45a3ade89`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:16 GMT
ADD file:ce6014a27d18915dc6d46c5c1f0f894f0027d1e41fbebb1599c16371b7bab2f1 in / 
# Tue, 23 Aug 2022 01:52:18 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:27:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:28:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 02:28:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:29:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cd84405c8b9e7a8c3d580c2148d25120dd697ea61e1cb55a62f33e67988b7043`  
		Last Modified: Tue, 23 Aug 2022 01:57:29 GMT  
		Size: 53.7 MB (53690830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d98e120b809269e56de468d2b91569789c521011e4d9b1806e43fd04462de2`  
		Last Modified: Tue, 23 Aug 2022 02:36:44 GMT  
		Size: 4.9 MB (4944180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb6be5911b40ca548e48c10b09cb2312f1698b4c84f09711c69389a94b1a8be`  
		Last Modified: Tue, 23 Aug 2022 02:36:44 GMT  
		Size: 10.7 MB (10657442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db608c3c3ce3568556faf63acbc2069811afe242faf8992ccf0ab1986ee38e4f`  
		Last Modified: Tue, 23 Aug 2022 02:37:07 GMT  
		Size: 54.7 MB (54680886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef10f752bfb9bb5888d549687e75a51ad78e1523ee87958e8b464cbd4dee4bb2`  
		Last Modified: Tue, 23 Aug 2022 02:37:46 GMT  
		Size: 189.7 MB (189711278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:6462b9cedd6360f9ac58ef0a745ed79497259cf4382b330b0a6ade58054037fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.8 MB (327786054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a954a50143d33244bd5b54771fe808f36befea012da728e64638c4f80b3f6b8c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:24 GMT
ADD file:4012c41187a03bdb3d37bec80f6255a1d46582e3ed145b4f313e42196529e524 in / 
# Tue, 23 Aug 2022 01:02:25 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:31:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:31:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:32:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:33:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6f683b9c66ef80b527ee5e4cb11969c6e0c1400ab69a4f1279af90f5766d70c7`  
		Last Modified: Tue, 23 Aug 2022 01:07:53 GMT  
		Size: 56.0 MB (56012624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f506948c8aa6d2e0693b583a388ce5e10b4393763bd2ea2529af3bfaa07f0c92`  
		Last Modified: Tue, 23 Aug 2022 01:40:01 GMT  
		Size: 5.1 MB (5085725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915cb3138c0c978b1806934d3f979cff24ecaed321fe7e13caa292cf9ca73dcc`  
		Last Modified: Tue, 23 Aug 2022 01:40:01 GMT  
		Size: 11.0 MB (11032841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc001487b6a15d61b32ac2dbd4b06bdede894077b8fcd3fa2f3969f98052bc3`  
		Last Modified: Tue, 23 Aug 2022 01:40:24 GMT  
		Size: 55.9 MB (55922719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e27a84eb0ba3a89f9e9e474d9c853c2dc7e9c83ef7d1e7281d208fd866b4c3`  
		Last Modified: Tue, 23 Aug 2022 01:41:12 GMT  
		Size: 199.7 MB (199732145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:a2b9c6b327a9a223c3efa1706bc2b9db685a596067cf19dcdd74613196680350
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.1 MB (301099619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44d5d833b9dcbd729eba0daafec46b29b0f0c91fb9dabc2d09bf20e3ce4d4b07`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:10:38 GMT
ADD file:a55d19f262e8338f932ce871c1cbc1718f9f74a5002212f38fea74f3858460a9 in / 
# Tue, 23 Aug 2022 00:10:43 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 22:24:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 22:24:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 22:26:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 22:33:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5ce438ccc597187e8a0dab5cc8906e6a0ec75a9320e55225ad2ec24765f7c0b4`  
		Last Modified: Tue, 23 Aug 2022 00:18:51 GMT  
		Size: 53.3 MB (53272999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567ecdfd8aa8d0bdcecff06b6b73dfbde6ae5451a3afec2a33aee7ca527b61e9`  
		Last Modified: Tue, 23 Aug 2022 22:49:03 GMT  
		Size: 4.9 MB (4918268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9374a0689765aeaeee15bb1c011bddd8cb323e6002385ceb42952a14d3210410`  
		Last Modified: Tue, 23 Aug 2022 22:49:06 GMT  
		Size: 10.7 MB (10661281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ccffd65aa7de17818aaae93c681cc96ca65baf5ab87b1989328259e139d360d`  
		Last Modified: Tue, 23 Aug 2022 22:49:57 GMT  
		Size: 53.3 MB (53304283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba6ce1b89a90d1ecaf04f415e6b8d8885f95ffc7c0a9357b6ef5545fc5e668e2`  
		Last Modified: Tue, 23 Aug 2022 22:52:01 GMT  
		Size: 178.9 MB (178942788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d26e0e6609eee5d0cc12d24a0e666e615785a20c5f2bcc91b8c39a3a1a85d14f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.0 MB (330981508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4404daf2be9fe8125eb280020678875923138a2f95a6de510414b2979fc8ea78`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:24:30 GMT
ADD file:c498f58d8dc50a2a20679642be8f6f43de8b79455438a1c237ef4c94a9ffe34c in / 
# Tue, 23 Aug 2022 01:24:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:58:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:59:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:01:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:62d01a7bda469557451a05bab1d4de7f53dd936e8032b36635019fd54cd927e4`  
		Last Modified: Tue, 23 Aug 2022 01:29:57 GMT  
		Size: 58.9 MB (58909173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b002340b938f821f3b0978eb9bfc47d2b8fe91b33c50508bd618c3c4b0ffe0`  
		Last Modified: Tue, 23 Aug 2022 02:10:43 GMT  
		Size: 5.4 MB (5412576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c65f43f4fd248e0fd18c35535f21fcafa740bdde05c5c367f32926f478e55f`  
		Last Modified: Tue, 23 Aug 2022 02:10:44 GMT  
		Size: 11.6 MB (11628949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6e7f52d8f52b4e830cdd20f538730eebe893f6c1f11aac1d0457ae132da2e8`  
		Last Modified: Tue, 23 Aug 2022 02:11:16 GMT  
		Size: 58.9 MB (58866219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35fecee5c5cd927c82781b73850d4cbf96c866f08985a8a76ee30c510df49f06`  
		Last Modified: Tue, 23 Aug 2022 02:12:17 GMT  
		Size: 196.2 MB (196164591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:7137006106c6222467d1d066c08b261d2ac29572e757ca58573eb833e89bb865
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.1 MB (296058506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:640e9d9a4e7fd555cdb338b68646231938a22a5a3322a831aa6f652376231080`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:53:42 GMT
ADD file:799d2eac4bf12dcb56eca0b771da879e8873a2a81b4d74520db7d6665d448ff6 in / 
# Tue, 23 Aug 2022 00:53:45 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 09:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 09:51:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 09:51:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 09:52:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e8428caa8cb9dd5cd48266f588e1d935181b0d75e5f4680a9d4d03700d44289`  
		Last Modified: Tue, 23 Aug 2022 01:01:15 GMT  
		Size: 53.3 MB (53279185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b41fe9abb9a7707d3bfd9881e997384ad70ba3f811c4152a16e11585318bd5`  
		Last Modified: Tue, 23 Aug 2022 09:59:58 GMT  
		Size: 5.1 MB (5146782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0215c1024f20ea76e1b536fcf226d87a639e72806443621a0bf52a719c0218fd`  
		Last Modified: Tue, 23 Aug 2022 09:59:59 GMT  
		Size: 10.8 MB (10765873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aeff4b644e5176d180f566f9889b6ed12e443f2fb955b119865cc113d26c3b1`  
		Last Modified: Tue, 23 Aug 2022 10:00:19 GMT  
		Size: 54.1 MB (54054805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e54f765beb5bf3b5c78fed34fddcc79e45dd90b63b47b01505666e38691ce6`  
		Last Modified: Tue, 23 Aug 2022 10:00:47 GMT  
		Size: 172.8 MB (172811861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stable-curl`

```console
$ docker pull buildpack-deps@sha256:eff18a8892c860c0db39795ed358137ba3216e5d240c912784210b438c28ddd8
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
$ docker pull buildpack-deps@sha256:1188bf8e99d160a3c226aafc7c799a0ad149eb3f6fdb99bddf16d0fc6624aa7c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.0 MB (71047046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3daa7ad5dfdd4bacbfa1c950fe1c68cfd3d10f276bc1218936f710b50c924a5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:40 GMT
ADD file:6944d322f4c04bd2192061822af5cbec8ac0a6b424c461d66174d32aed604972 in / 
# Tue, 23 Aug 2022 00:20:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:48:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:48:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1671565cc8df8c365c9b661d3fbc164e73d01f1b0430c6179588428f99a9da2e`  
		Last Modified: Tue, 23 Aug 2022 00:24:32 GMT  
		Size: 55.0 MB (55007555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e94d13e55e7a4ef17ff21376f57fb95c7e1706931f8704aa99260968d81f6e4`  
		Last Modified: Tue, 23 Aug 2022 00:55:37 GMT  
		Size: 5.2 MB (5163019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9c7528c685216129e8e67bf362a7702e7b1daa585ab85546a41508830657d6`  
		Last Modified: Tue, 23 Aug 2022 00:55:38 GMT  
		Size: 10.9 MB (10876472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:9241cca9693c0372458ebec46ddb886fc0bffe1b9aeee2c7d4dfc0050b1a55d0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.2 MB (68192296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f44e91617f5732bcc2b11f0aa7d00e23d82a7b4f67e4d5a7787a52433fa706df`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:16:51 GMT
ADD file:132abd62c4fa546798c96d5b1f6f409de9ee27242caf6c479d65309b764c3ece in / 
# Tue, 23 Aug 2022 01:16:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 06:19:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 06:19:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1918e2afd901ca723b3483d8d521789daac45ddbaae2bf9fd813933e826f39b4`  
		Last Modified: Tue, 23 Aug 2022 01:22:10 GMT  
		Size: 52.5 MB (52547848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a58d3f469ed5c6be23bbc74a836bceb306e58e8cd5e58e4464c2b23519543a`  
		Last Modified: Tue, 23 Aug 2022 06:26:58 GMT  
		Size: 5.1 MB (5070690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61379bcded34629fad0582d1d42f2cba36b5f418591509e15301773304e7c7c0`  
		Last Modified: Tue, 23 Aug 2022 06:26:59 GMT  
		Size: 10.6 MB (10573758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:56c33d4b477957b573aed7cc5367f95d01459a2a0a6312c42994c79f488b1cdc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65353658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f92c349465773257e5ffe974e22d6a19ca708f3db946ebf552668157b43ba5c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:42:43 GMT
ADD file:21190c24a038c3c9de64b88797bf00e4c4319bd598c7c465cab2ca88d0502416 in / 
# Tue, 23 Aug 2022 01:42:43 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 12:59:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:00:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c715a126a4d5182c28d2d7b1c81de847bfbbacf6851819fef3eb28e3feb7db0e`  
		Last Modified: Tue, 23 Aug 2022 01:49:30 GMT  
		Size: 50.2 MB (50204931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cecc62e275236714359bda7d1f9c8412e8fa8539f3ef682eebd9c77986c927d`  
		Last Modified: Tue, 23 Aug 2022 13:11:58 GMT  
		Size: 4.9 MB (4930827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818eb872fe75602d611beeac0db63da0a4d8a67aee8b909d5114814f76446a5e`  
		Last Modified: Tue, 23 Aug 2022 13:11:59 GMT  
		Size: 10.2 MB (10217900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:224dfb7f5032a11af8748f4e65daa8f50f478612b91b1c9176a7ef035ed374ba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.3 MB (69292452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93d7443e4194085764e49b9d96d081bc973eba35516e6d88b0058b0854b2970e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:16 GMT
ADD file:ce6014a27d18915dc6d46c5c1f0f894f0027d1e41fbebb1599c16371b7bab2f1 in / 
# Tue, 23 Aug 2022 01:52:18 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:27:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:28:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:cd84405c8b9e7a8c3d580c2148d25120dd697ea61e1cb55a62f33e67988b7043`  
		Last Modified: Tue, 23 Aug 2022 01:57:29 GMT  
		Size: 53.7 MB (53690830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d98e120b809269e56de468d2b91569789c521011e4d9b1806e43fd04462de2`  
		Last Modified: Tue, 23 Aug 2022 02:36:44 GMT  
		Size: 4.9 MB (4944180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb6be5911b40ca548e48c10b09cb2312f1698b4c84f09711c69389a94b1a8be`  
		Last Modified: Tue, 23 Aug 2022 02:36:44 GMT  
		Size: 10.7 MB (10657442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:0d9e01a77b19864476557d06dadfb768771a3b89333dbbf3b7c3fd10138e3fa7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.1 MB (72131190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c00fec5790de3e13e4285b83054a6850bd58812ba11a6858bbfc8607533256b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:24 GMT
ADD file:4012c41187a03bdb3d37bec80f6255a1d46582e3ed145b4f313e42196529e524 in / 
# Tue, 23 Aug 2022 01:02:25 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:31:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:31:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6f683b9c66ef80b527ee5e4cb11969c6e0c1400ab69a4f1279af90f5766d70c7`  
		Last Modified: Tue, 23 Aug 2022 01:07:53 GMT  
		Size: 56.0 MB (56012624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f506948c8aa6d2e0693b583a388ce5e10b4393763bd2ea2529af3bfaa07f0c92`  
		Last Modified: Tue, 23 Aug 2022 01:40:01 GMT  
		Size: 5.1 MB (5085725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915cb3138c0c978b1806934d3f979cff24ecaed321fe7e13caa292cf9ca73dcc`  
		Last Modified: Tue, 23 Aug 2022 01:40:01 GMT  
		Size: 11.0 MB (11032841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:b88de28a9b03c3efa219ebe99731c2dcf063299c1769c16ab9fe8fdacf59ff38
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68852548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15015eb73f5ade0114232ff8e03c9c853246f11dd35a7f95196f6c3eef74d820`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:10:38 GMT
ADD file:a55d19f262e8338f932ce871c1cbc1718f9f74a5002212f38fea74f3858460a9 in / 
# Tue, 23 Aug 2022 00:10:43 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 22:24:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 22:24:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5ce438ccc597187e8a0dab5cc8906e6a0ec75a9320e55225ad2ec24765f7c0b4`  
		Last Modified: Tue, 23 Aug 2022 00:18:51 GMT  
		Size: 53.3 MB (53272999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567ecdfd8aa8d0bdcecff06b6b73dfbde6ae5451a3afec2a33aee7ca527b61e9`  
		Last Modified: Tue, 23 Aug 2022 22:49:03 GMT  
		Size: 4.9 MB (4918268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9374a0689765aeaeee15bb1c011bddd8cb323e6002385ceb42952a14d3210410`  
		Last Modified: Tue, 23 Aug 2022 22:49:06 GMT  
		Size: 10.7 MB (10661281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d8b7e1a18e133da0ea19134be7a76cdd22ec4f10fb6a01976563fcbea1555ce0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.0 MB (75950698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d703a630725af8cf9c5a1f40484ae8fc94e5360d191852caf1164235d16cd71`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:24:30 GMT
ADD file:c498f58d8dc50a2a20679642be8f6f43de8b79455438a1c237ef4c94a9ffe34c in / 
# Tue, 23 Aug 2022 01:24:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:58:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:62d01a7bda469557451a05bab1d4de7f53dd936e8032b36635019fd54cd927e4`  
		Last Modified: Tue, 23 Aug 2022 01:29:57 GMT  
		Size: 58.9 MB (58909173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b002340b938f821f3b0978eb9bfc47d2b8fe91b33c50508bd618c3c4b0ffe0`  
		Last Modified: Tue, 23 Aug 2022 02:10:43 GMT  
		Size: 5.4 MB (5412576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c65f43f4fd248e0fd18c35535f21fcafa740bdde05c5c367f32926f478e55f`  
		Last Modified: Tue, 23 Aug 2022 02:10:44 GMT  
		Size: 11.6 MB (11628949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:8d5fc4782913393f45ddd1ea898bcb30f1bb102bcf7d603315f3a6aaec9ea202
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69191840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a21a8727c9bc59c13f1f4b1072ecef25e905519ec56c0235f3a2d399dbdede69`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:53:42 GMT
ADD file:799d2eac4bf12dcb56eca0b771da879e8873a2a81b4d74520db7d6665d448ff6 in / 
# Tue, 23 Aug 2022 00:53:45 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 09:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 09:51:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6e8428caa8cb9dd5cd48266f588e1d935181b0d75e5f4680a9d4d03700d44289`  
		Last Modified: Tue, 23 Aug 2022 01:01:15 GMT  
		Size: 53.3 MB (53279185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b41fe9abb9a7707d3bfd9881e997384ad70ba3f811c4152a16e11585318bd5`  
		Last Modified: Tue, 23 Aug 2022 09:59:58 GMT  
		Size: 5.1 MB (5146782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0215c1024f20ea76e1b536fcf226d87a639e72806443621a0bf52a719c0218fd`  
		Last Modified: Tue, 23 Aug 2022 09:59:59 GMT  
		Size: 10.8 MB (10765873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stable-scm`

```console
$ docker pull buildpack-deps@sha256:a7a9dbad2a104ca82facdb49ca65421b485045a3a51aad05bd44609b839401a1
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
$ docker pull buildpack-deps@sha256:6c1872f4ea21628b7c323305593b94d6ecc5125852b4a03827c6d38b473835d2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.6 MB (125631181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e73278505bb143c007d79f686483ae493b77ad2ad4f7cadc67deeb86f4dd38e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:40 GMT
ADD file:6944d322f4c04bd2192061822af5cbec8ac0a6b424c461d66174d32aed604972 in / 
# Tue, 23 Aug 2022 00:20:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:48:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:48:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 00:48:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1671565cc8df8c365c9b661d3fbc164e73d01f1b0430c6179588428f99a9da2e`  
		Last Modified: Tue, 23 Aug 2022 00:24:32 GMT  
		Size: 55.0 MB (55007555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e94d13e55e7a4ef17ff21376f57fb95c7e1706931f8704aa99260968d81f6e4`  
		Last Modified: Tue, 23 Aug 2022 00:55:37 GMT  
		Size: 5.2 MB (5163019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9c7528c685216129e8e67bf362a7702e7b1daa585ab85546a41508830657d6`  
		Last Modified: Tue, 23 Aug 2022 00:55:38 GMT  
		Size: 10.9 MB (10876472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ad072f9cd16fc8eb93b182b20e758e11acc0ef60babef0bf1043c08de1901a`  
		Last Modified: Tue, 23 Aug 2022 00:55:57 GMT  
		Size: 54.6 MB (54584135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:f544bf2e62950527f9e904a056de2ffc7f7d57a0051cc0a83f53029d715f2847
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.5 MB (120512626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:254098229367b0e03446fdc4d0858c497972184186719e50d9853daf38a33bb0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:16:51 GMT
ADD file:132abd62c4fa546798c96d5b1f6f409de9ee27242caf6c479d65309b764c3ece in / 
# Tue, 23 Aug 2022 01:16:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 06:19:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 06:19:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 06:19:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1918e2afd901ca723b3483d8d521789daac45ddbaae2bf9fd813933e826f39b4`  
		Last Modified: Tue, 23 Aug 2022 01:22:10 GMT  
		Size: 52.5 MB (52547848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a58d3f469ed5c6be23bbc74a836bceb306e58e8cd5e58e4464c2b23519543a`  
		Last Modified: Tue, 23 Aug 2022 06:26:58 GMT  
		Size: 5.1 MB (5070690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61379bcded34629fad0582d1d42f2cba36b5f418591509e15301773304e7c7c0`  
		Last Modified: Tue, 23 Aug 2022 06:26:59 GMT  
		Size: 10.6 MB (10573758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c872e375903a379cc5ab82220655ab6973d82f8b48ab51b42d197a4ab189b6b`  
		Last Modified: Tue, 23 Aug 2022 06:27:30 GMT  
		Size: 52.3 MB (52320330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:495a7139ac1f0b677a9476288d454f9dfd4763312ef4dc4d467ce3f29c36caed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.7 MB (115696134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e362c69b51c9b48c55b381399fc2b7a49ec81e115a633a60638b43084b817c9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:42:43 GMT
ADD file:21190c24a038c3c9de64b88797bf00e4c4319bd598c7c465cab2ca88d0502416 in / 
# Tue, 23 Aug 2022 01:42:43 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 12:59:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:00:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 13:00:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c715a126a4d5182c28d2d7b1c81de847bfbbacf6851819fef3eb28e3feb7db0e`  
		Last Modified: Tue, 23 Aug 2022 01:49:30 GMT  
		Size: 50.2 MB (50204931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cecc62e275236714359bda7d1f9c8412e8fa8539f3ef682eebd9c77986c927d`  
		Last Modified: Tue, 23 Aug 2022 13:11:58 GMT  
		Size: 4.9 MB (4930827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818eb872fe75602d611beeac0db63da0a4d8a67aee8b909d5114814f76446a5e`  
		Last Modified: Tue, 23 Aug 2022 13:11:59 GMT  
		Size: 10.2 MB (10217900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94cbc350f4a21916bb6fe70920c962a4889a5059aee86258e4d8263f0c7afbef`  
		Last Modified: Tue, 23 Aug 2022 13:12:28 GMT  
		Size: 50.3 MB (50342476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:5156f3bb278fb0dda42cdf0b406331f8809ab19a049e6ea5506665811c002475
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.0 MB (123973338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acf31c8a1856f38bfa1a001f3b72d3e9678c5aadee3ec10352d90f571361e1fe`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:16 GMT
ADD file:ce6014a27d18915dc6d46c5c1f0f894f0027d1e41fbebb1599c16371b7bab2f1 in / 
# Tue, 23 Aug 2022 01:52:18 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:27:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:28:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 02:28:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cd84405c8b9e7a8c3d580c2148d25120dd697ea61e1cb55a62f33e67988b7043`  
		Last Modified: Tue, 23 Aug 2022 01:57:29 GMT  
		Size: 53.7 MB (53690830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d98e120b809269e56de468d2b91569789c521011e4d9b1806e43fd04462de2`  
		Last Modified: Tue, 23 Aug 2022 02:36:44 GMT  
		Size: 4.9 MB (4944180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb6be5911b40ca548e48c10b09cb2312f1698b4c84f09711c69389a94b1a8be`  
		Last Modified: Tue, 23 Aug 2022 02:36:44 GMT  
		Size: 10.7 MB (10657442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db608c3c3ce3568556faf63acbc2069811afe242faf8992ccf0ab1986ee38e4f`  
		Last Modified: Tue, 23 Aug 2022 02:37:07 GMT  
		Size: 54.7 MB (54680886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:1afc200fb3ee2b4b85c5c984fbbc088ff53286077a843588bc04c935cd6b7416
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.1 MB (128053909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bceeed6ce487fd59052390091c5f4300ff05ada27c1650c1dbf83f91a4d9788b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:24 GMT
ADD file:4012c41187a03bdb3d37bec80f6255a1d46582e3ed145b4f313e42196529e524 in / 
# Tue, 23 Aug 2022 01:02:25 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:31:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:31:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:32:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6f683b9c66ef80b527ee5e4cb11969c6e0c1400ab69a4f1279af90f5766d70c7`  
		Last Modified: Tue, 23 Aug 2022 01:07:53 GMT  
		Size: 56.0 MB (56012624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f506948c8aa6d2e0693b583a388ce5e10b4393763bd2ea2529af3bfaa07f0c92`  
		Last Modified: Tue, 23 Aug 2022 01:40:01 GMT  
		Size: 5.1 MB (5085725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915cb3138c0c978b1806934d3f979cff24ecaed321fe7e13caa292cf9ca73dcc`  
		Last Modified: Tue, 23 Aug 2022 01:40:01 GMT  
		Size: 11.0 MB (11032841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc001487b6a15d61b32ac2dbd4b06bdede894077b8fcd3fa2f3969f98052bc3`  
		Last Modified: Tue, 23 Aug 2022 01:40:24 GMT  
		Size: 55.9 MB (55922719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:c8f075c6f8d978558f03a94da80ad547aa3e8af5a92a9b3d461d8db9b40542bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122156831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fdba3c8b6471cc9b1138ee1a4111402f4476b568b1735d38c33912c379db3b3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:10:38 GMT
ADD file:a55d19f262e8338f932ce871c1cbc1718f9f74a5002212f38fea74f3858460a9 in / 
# Tue, 23 Aug 2022 00:10:43 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 22:24:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 22:24:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 22:26:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5ce438ccc597187e8a0dab5cc8906e6a0ec75a9320e55225ad2ec24765f7c0b4`  
		Last Modified: Tue, 23 Aug 2022 00:18:51 GMT  
		Size: 53.3 MB (53272999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567ecdfd8aa8d0bdcecff06b6b73dfbde6ae5451a3afec2a33aee7ca527b61e9`  
		Last Modified: Tue, 23 Aug 2022 22:49:03 GMT  
		Size: 4.9 MB (4918268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9374a0689765aeaeee15bb1c011bddd8cb323e6002385ceb42952a14d3210410`  
		Last Modified: Tue, 23 Aug 2022 22:49:06 GMT  
		Size: 10.7 MB (10661281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ccffd65aa7de17818aaae93c681cc96ca65baf5ab87b1989328259e139d360d`  
		Last Modified: Tue, 23 Aug 2022 22:49:57 GMT  
		Size: 53.3 MB (53304283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:cb31310b3598fc3d3ad9daa40df9a133a6e2e360aee409d29191203c4686d095
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134816917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30881ed3045278b91be936aafc665ff71cd8bc93d39d8b69650de485729b3d02`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:24:30 GMT
ADD file:c498f58d8dc50a2a20679642be8f6f43de8b79455438a1c237ef4c94a9ffe34c in / 
# Tue, 23 Aug 2022 01:24:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:58:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:59:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:62d01a7bda469557451a05bab1d4de7f53dd936e8032b36635019fd54cd927e4`  
		Last Modified: Tue, 23 Aug 2022 01:29:57 GMT  
		Size: 58.9 MB (58909173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b002340b938f821f3b0978eb9bfc47d2b8fe91b33c50508bd618c3c4b0ffe0`  
		Last Modified: Tue, 23 Aug 2022 02:10:43 GMT  
		Size: 5.4 MB (5412576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c65f43f4fd248e0fd18c35535f21fcafa740bdde05c5c367f32926f478e55f`  
		Last Modified: Tue, 23 Aug 2022 02:10:44 GMT  
		Size: 11.6 MB (11628949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6e7f52d8f52b4e830cdd20f538730eebe893f6c1f11aac1d0457ae132da2e8`  
		Last Modified: Tue, 23 Aug 2022 02:11:16 GMT  
		Size: 58.9 MB (58866219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:fe781f689e6f87bbf043328a5546a3c8810e4bb71bf4aace341aa84bc8e2aab4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123246645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd05daa086ec2eb9eb0d8724cfebe627e1a621d31c39e41c49c480e60b4413fd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:53:42 GMT
ADD file:799d2eac4bf12dcb56eca0b771da879e8873a2a81b4d74520db7d6665d448ff6 in / 
# Tue, 23 Aug 2022 00:53:45 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 09:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 09:51:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 09:51:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e8428caa8cb9dd5cd48266f588e1d935181b0d75e5f4680a9d4d03700d44289`  
		Last Modified: Tue, 23 Aug 2022 01:01:15 GMT  
		Size: 53.3 MB (53279185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b41fe9abb9a7707d3bfd9881e997384ad70ba3f811c4152a16e11585318bd5`  
		Last Modified: Tue, 23 Aug 2022 09:59:58 GMT  
		Size: 5.1 MB (5146782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0215c1024f20ea76e1b536fcf226d87a639e72806443621a0bf52a719c0218fd`  
		Last Modified: Tue, 23 Aug 2022 09:59:59 GMT  
		Size: 10.8 MB (10765873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aeff4b644e5176d180f566f9889b6ed12e443f2fb955b119865cc113d26c3b1`  
		Last Modified: Tue, 23 Aug 2022 10:00:19 GMT  
		Size: 54.1 MB (54054805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:testing`

```console
$ docker pull buildpack-deps@sha256:3f1c2db6b34ee6bc4359ac8cdbaba18a30caae19e001d8b7bb88a652919765ca
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

### `buildpack-deps:testing` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:c499dd57309b82d2d43be6cd76563d9713b78e09edac66558e8adb44d73140f2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **562.1 MB (562080993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ce38a856ecb08376f79b2d4fd6cca8d215ab17103b6274edcd9aa076032ade5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:15 GMT
ADD file:7507edfdf016128615e9ba278d471fd6d27c96436e543786b691c93b6f94b56b in / 
# Tue, 23 Aug 2022 00:20:16 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:46:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:46:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 00:46:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:47:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5e784af754e1c7855decd29b818520a98b5b539515cd7c199c5dbceb6cc4a45f`  
		Last Modified: Tue, 23 Aug 2022 00:23:57 GMT  
		Size: 52.7 MB (52725730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06352499c53ea1415d7d7121128de838e832cbc465b145c71d05fb7b74a91c0`  
		Last Modified: Tue, 23 Aug 2022 00:54:04 GMT  
		Size: 9.3 MB (9298815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e88fbc1ce3af2aec72e131f3b876f2554849f8d6291840fbaf61b24970e54c3`  
		Last Modified: Tue, 23 Aug 2022 00:54:04 GMT  
		Size: 11.3 MB (11272439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2afebddf0d45a19b246f4ff1ead1dd600b48cc494afd00873819774f29c6f388`  
		Last Modified: Tue, 23 Aug 2022 00:54:22 GMT  
		Size: 57.6 MB (57602962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7909283d0b83eb6d0800ae7c471c60ae0891ef4c36524f7ff60b725616e553ed`  
		Last Modified: Tue, 23 Aug 2022 00:55:27 GMT  
		Size: 431.2 MB (431181047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:97f078f2318ddd0d5e369b26b804cae7895b80a64cfdb38598ed08f09b59de96
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **512.6 MB (512603026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9338cdc62f6d8b5386b6ceae633ea50d5f36bd4d30c72201040efca568d03302`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:16:08 GMT
ADD file:dbc0c48f409cbe73d340bec8639492807b8c28fa6907379a17a958448dca1829 in / 
# Tue, 23 Aug 2022 01:16:08 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 06:16:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 06:16:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 06:16:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 06:18:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3204f8dd2e8fdf47391628664d2c96551393e3e0abd1e471abeb57296519c816`  
		Last Modified: Tue, 23 Aug 2022 01:21:24 GMT  
		Size: 51.8 MB (51814042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2edbed2d89089bed15e37327dce17d68521ccd0390a9172314785a01bb2918c5`  
		Last Modified: Tue, 23 Aug 2022 06:24:42 GMT  
		Size: 8.7 MB (8740375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ead884b6cf02ae26001f7fa32ee0d5127f5b1f36fe6d675bf0ab7b8b81baa00`  
		Last Modified: Tue, 23 Aug 2022 06:24:42 GMT  
		Size: 10.9 MB (10946896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e395af4802fa3dfe5d8dc10a19e4fb9ea0adaa8951ba0595e9c756a12d412bb8`  
		Last Modified: Tue, 23 Aug 2022 06:25:07 GMT  
		Size: 55.3 MB (55284425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509d388565301a498f7b95d89df044727bf2633fd54aacd973fc712a97327789`  
		Last Modified: Tue, 23 Aug 2022 06:26:41 GMT  
		Size: 385.8 MB (385817288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ebbb69050ba98917a5a15e299ba7aa9339f319cd4cdd3156bfebb53cbebf582d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **500.2 MB (500233814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bad6c9a12283cdf877c74e1d905354fcb63b8be182f414c2de79272cd53bf52`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:42:14 GMT
ADD file:590ff1916ed8a15a7a205153d20c2823a242c228573a1868134df4bdd95f10d8 in / 
# Tue, 23 Aug 2022 01:42:14 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 12:57:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 12:57:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 12:58:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 12:59:43 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b4a2cf95b2637a1520aeb527ca7569456a3bcf1d740f72cc418357cbe490704d`  
		Last Modified: Tue, 23 Aug 2022 01:48:45 GMT  
		Size: 49.6 MB (49555090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0a9319f004c20513b7f62d6d76d1b1959183b5ad5b488373ca6330a9d6797b`  
		Last Modified: Tue, 23 Aug 2022 13:09:50 GMT  
		Size: 8.4 MB (8402996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fd63a2d6ab83a6d913419cd2a446fc94d0d9a4c654bf2a3c13dfe3a7116609`  
		Last Modified: Tue, 23 Aug 2022 13:09:49 GMT  
		Size: 10.6 MB (10589855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c7d7ae465211d33c40484e48402566e419669463cab573010f1ab877df64a9`  
		Last Modified: Tue, 23 Aug 2022 13:10:16 GMT  
		Size: 53.3 MB (53323503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ac7c9931aada6b836dce88ec19cd79064ffe2024e95270c239c73860ab7d72`  
		Last Modified: Tue, 23 Aug 2022 13:11:44 GMT  
		Size: 378.4 MB (378362370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:b8074d04677387c84532dbc39903d4a7ba2dbac38fa624956417e4b251024d25
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **551.9 MB (551918652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1473f33d94d3c58cb12b6d618f9cafa967b830841c427a4fa8717f924dd351b2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:51:53 GMT
ADD file:f94a576f262c4fcf5112164145c04850c826787b299878e7e126754d1211a51c in / 
# Tue, 23 Aug 2022 01:51:53 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:25:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:25:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 02:26:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:27:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7dd208a8a7339c037c691e6ace1cd3f94803ee4c17a3211b9ccadf01d1ff2ca9`  
		Last Modified: Tue, 23 Aug 2022 01:56:50 GMT  
		Size: 53.1 MB (53117563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a6d7761ab15abc5f27917ed7e543565cb302e30ac8bd10819c205f079ec603`  
		Last Modified: Tue, 23 Aug 2022 02:35:05 GMT  
		Size: 9.1 MB (9133938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d472709c6f5c8abe91373fba2db77fd3b0946f573269803173452485abc6ff8b`  
		Last Modified: Tue, 23 Aug 2022 02:35:05 GMT  
		Size: 11.1 MB (11062413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247b0fb5989ae9d485d4b97b959d16adfaeb2e92bf9a74bd8b1f677bb7f3e1c5`  
		Last Modified: Tue, 23 Aug 2022 02:35:25 GMT  
		Size: 57.5 MB (57496084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e62402acaffd55bc794eef07b132e4223f8f48067c5d1df8909da8f8de8e39`  
		Last Modified: Tue, 23 Aug 2022 02:36:32 GMT  
		Size: 421.1 MB (421108654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8539ef8ee56afeb586b85e49787586a5111a6de92bc10b9f37ca69bd9309ad13
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.1 MB (355072478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b32f2b395672361202ddd299bd9ee7fb01a3d461778187967fb1f32cdf4a2d82`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:01:59 GMT
ADD file:1c8ebe8b69a2d3c236c8a947162fab2e579f4bf01bff01695a3c46557f6c73f4 in / 
# Tue, 23 Aug 2022 01:02:00 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:28:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:28:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:29:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:31:24 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:29bf8f676853094720e43096224f2ec8a31ffa3752cf7a1e52fb9e72ae069480`  
		Last Modified: Tue, 23 Aug 2022 01:07:13 GMT  
		Size: 54.1 MB (54096938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0426ba96c16ee4ea8eb5b5322685d94b842c455938234d92ca07814c6ae081`  
		Last Modified: Tue, 23 Aug 2022 01:38:51 GMT  
		Size: 9.5 MB (9475146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86201f3e5308e2da4dad080700c08b4d6a0a02c265e56c7a0cdae2889f16b442`  
		Last Modified: Tue, 23 Aug 2022 01:38:51 GMT  
		Size: 11.5 MB (11473600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4eae1a3c8a2b637c155af3a0e81b010eea8632db588e887a59f57d020ad81a8`  
		Last Modified: Tue, 23 Aug 2022 01:39:11 GMT  
		Size: 59.1 MB (59102590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ecd69ec89ab5cbb90df7026e375153b4bae6f2e062807e484c266484a434f19`  
		Last Modified: Tue, 23 Aug 2022 01:39:48 GMT  
		Size: 220.9 MB (220924204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:a33f9fc319310e0dc05df0ac31354c80d3a3752809f776e4531c09131e54f6df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **588.8 MB (588838001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16b0b2ddf00ac1d07da3682f6cfc85609adb6af1836c17a484332e1d9817ccfe`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:09:18 GMT
ADD file:2b4a878ee82590d9ee2da01a2501742d21f6d050a0002f9bd484a4d7c8620d2e in / 
# Tue, 23 Aug 2022 00:09:23 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 22:12:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 22:13:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 22:15:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 22:23:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4b18e364c6342ca1244071a2f94edf42b92a5b7997d16df3b26467139f3f0603`  
		Last Modified: Tue, 23 Aug 2022 00:17:33 GMT  
		Size: 53.1 MB (53119349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5edf0a5e5947b8da11a8b58c48bd00dc43fe37b1375dd57214cc77b72c0bc009`  
		Last Modified: Tue, 23 Aug 2022 22:43:15 GMT  
		Size: 8.7 MB (8660383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd311acb344ec357f0aa8b600c00bac50d5489700c6ec00ff2ec71f10bf3789`  
		Last Modified: Tue, 23 Aug 2022 22:43:14 GMT  
		Size: 11.0 MB (11042106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6304e93b6d685763966db039d84593203f3027de2420ebe4cf0e2865b59ee64d`  
		Last Modified: Tue, 23 Aug 2022 22:44:05 GMT  
		Size: 56.5 MB (56454547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d95aec47b529f681de91b7db74b4fdb10f85a8019db378445bf8e551565e0369`  
		Last Modified: Tue, 23 Aug 2022 22:48:49 GMT  
		Size: 459.6 MB (459561616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:ee2a6c73ac3292db2fa2fbf661eb2e89b0efb41e7d31d177c394eef94afc20fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **561.4 MB (561424552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f377208d9b0ee3a46f734c8e72364e0683ef2f7b1516eaa2a8fc4b2eb0878050`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:23:48 GMT
ADD file:92444ce23c3227ef88446469c37fc41decda1ba975ddfb1be3e1ebb1e694471b in / 
# Tue, 23 Aug 2022 01:23:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:52:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:52:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:53:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:57:32 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a2d2f2c5b4e64eabb8a7632609e67883239433d932129bf478f7614059a9aabe`  
		Last Modified: Tue, 23 Aug 2022 01:29:05 GMT  
		Size: 57.3 MB (57289866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b43c7a1c5614eda4b722aada1632b2b42c7499b945bcd902a405d6811943e66`  
		Last Modified: Tue, 23 Aug 2022 02:08:15 GMT  
		Size: 9.9 MB (9888870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4983e94a7031bdb88baa08be05b8f42254ef49f65245663476650772c95d77`  
		Last Modified: Tue, 23 Aug 2022 02:08:15 GMT  
		Size: 12.1 MB (12083610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea4205d8530bba3b66567e144b76048ea3deb5e2f1d3604690cc87c10af416f`  
		Last Modified: Tue, 23 Aug 2022 02:08:43 GMT  
		Size: 62.4 MB (62419202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e108af90182e1e05955b926792132c93a713e0f0ae2b578251685acee0a56d`  
		Last Modified: Tue, 23 Aug 2022 02:10:29 GMT  
		Size: 419.7 MB (419743004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:8c0ab6fb48d76634a12d5294e8bca9d24a5b9906ced33a933a040932fd7b8c51
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **506.2 MB (506202129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a30d9f47701b1b9e8e1facf3f4c9c146ebb42ad42f38bb07e3be148d38711791`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:53:14 GMT
ADD file:e8167229629003ac0dcc7f0bcc35a939121e9b4a88b67483883c2741f5415634 in / 
# Tue, 23 Aug 2022 00:53:16 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 09:49:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 09:49:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 09:49:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 09:51:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bfa0b60dda37e3a2f71f5d19d0259a51a84ce3f8e9deff107720c9868e69769b`  
		Last Modified: Tue, 23 Aug 2022 00:57:59 GMT  
		Size: 51.6 MB (51559576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9f7dae28c5d2750f7a41520dc8fec8c6914c21a7ced6fbda8b32c01477bc57`  
		Last Modified: Tue, 23 Aug 2022 09:58:50 GMT  
		Size: 8.9 MB (8941068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a871302fe26c06a3669e3a3f80c6e947aba9fbecf2fddb59dfe0739cf8a3f48a`  
		Last Modified: Tue, 23 Aug 2022 09:58:50 GMT  
		Size: 11.2 MB (11166576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f7f08e932daba42246e92ace2e6a7084e92eb623212ae6d100ba95f988439df`  
		Last Modified: Tue, 23 Aug 2022 09:59:04 GMT  
		Size: 56.9 MB (56866268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7411d09609a3404724d2396baedced7c080958509598eeaf565769349ead75`  
		Last Modified: Tue, 23 Aug 2022 09:59:51 GMT  
		Size: 377.7 MB (377668641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:testing-curl`

```console
$ docker pull buildpack-deps@sha256:920db90394b6ae75318c2d0abffd0e57dec63104639684dc07b01dd38a87adf5
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

### `buildpack-deps:testing-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:a2c9bcba0f65768c2f380cdb068c2ea33e88f7186a94142f0a02884cbbecae2d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.3 MB (73296984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96518376d229d3c3d2c3f2977817cd43b1253209b546da45f802bdd6fede1ef5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:15 GMT
ADD file:7507edfdf016128615e9ba278d471fd6d27c96436e543786b691c93b6f94b56b in / 
# Tue, 23 Aug 2022 00:20:16 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:46:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:46:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5e784af754e1c7855decd29b818520a98b5b539515cd7c199c5dbceb6cc4a45f`  
		Last Modified: Tue, 23 Aug 2022 00:23:57 GMT  
		Size: 52.7 MB (52725730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06352499c53ea1415d7d7121128de838e832cbc465b145c71d05fb7b74a91c0`  
		Last Modified: Tue, 23 Aug 2022 00:54:04 GMT  
		Size: 9.3 MB (9298815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e88fbc1ce3af2aec72e131f3b876f2554849f8d6291840fbaf61b24970e54c3`  
		Last Modified: Tue, 23 Aug 2022 00:54:04 GMT  
		Size: 11.3 MB (11272439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:46faed2ba6d4fb76b3258765430464b1a7003b23ed86435d2752c89d397c5b0b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.5 MB (71501313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc2b9a42ac97d4c443a8cd1be847430cb3bd4ea1d867a7f662c15cb1144dc327`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:16:08 GMT
ADD file:dbc0c48f409cbe73d340bec8639492807b8c28fa6907379a17a958448dca1829 in / 
# Tue, 23 Aug 2022 01:16:08 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 06:16:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 06:16:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3204f8dd2e8fdf47391628664d2c96551393e3e0abd1e471abeb57296519c816`  
		Last Modified: Tue, 23 Aug 2022 01:21:24 GMT  
		Size: 51.8 MB (51814042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2edbed2d89089bed15e37327dce17d68521ccd0390a9172314785a01bb2918c5`  
		Last Modified: Tue, 23 Aug 2022 06:24:42 GMT  
		Size: 8.7 MB (8740375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ead884b6cf02ae26001f7fa32ee0d5127f5b1f36fe6d675bf0ab7b8b81baa00`  
		Last Modified: Tue, 23 Aug 2022 06:24:42 GMT  
		Size: 10.9 MB (10946896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:eca2e025d883dc6e53b0bcba83bba2ebbd9180d026142ba402bee57e7e36cb1a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68547941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fdb79dc67924d7dc4d70c832938055d861fd8a72ba69c93b61f05333fb06605`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:42:14 GMT
ADD file:590ff1916ed8a15a7a205153d20c2823a242c228573a1868134df4bdd95f10d8 in / 
# Tue, 23 Aug 2022 01:42:14 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 12:57:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 12:57:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b4a2cf95b2637a1520aeb527ca7569456a3bcf1d740f72cc418357cbe490704d`  
		Last Modified: Tue, 23 Aug 2022 01:48:45 GMT  
		Size: 49.6 MB (49555090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0a9319f004c20513b7f62d6d76d1b1959183b5ad5b488373ca6330a9d6797b`  
		Last Modified: Tue, 23 Aug 2022 13:09:50 GMT  
		Size: 8.4 MB (8402996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fd63a2d6ab83a6d913419cd2a446fc94d0d9a4c654bf2a3c13dfe3a7116609`  
		Last Modified: Tue, 23 Aug 2022 13:09:49 GMT  
		Size: 10.6 MB (10589855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:af43066ded189a6b7e29c63c61133429e2c2b2d43a2e58d2daa76efe5b917bc3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.3 MB (73313914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1d0bb4e26e6776a1c17038201bde02c005f88d7bfa7354e7d0e3218ddf36414`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:51:53 GMT
ADD file:f94a576f262c4fcf5112164145c04850c826787b299878e7e126754d1211a51c in / 
# Tue, 23 Aug 2022 01:51:53 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:25:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:25:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:7dd208a8a7339c037c691e6ace1cd3f94803ee4c17a3211b9ccadf01d1ff2ca9`  
		Last Modified: Tue, 23 Aug 2022 01:56:50 GMT  
		Size: 53.1 MB (53117563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a6d7761ab15abc5f27917ed7e543565cb302e30ac8bd10819c205f079ec603`  
		Last Modified: Tue, 23 Aug 2022 02:35:05 GMT  
		Size: 9.1 MB (9133938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d472709c6f5c8abe91373fba2db77fd3b0946f573269803173452485abc6ff8b`  
		Last Modified: Tue, 23 Aug 2022 02:35:05 GMT  
		Size: 11.1 MB (11062413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:be37277a8a268026b2fabbf0c0d4d77c022a17d6dd095e2cedc7d8f4a4b3cf65
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.0 MB (75045684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6b54df36b64a7450c4db38d1ca99f0ef6f8533945a326f1f4f7ac4e6e9ef983`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:01:59 GMT
ADD file:1c8ebe8b69a2d3c236c8a947162fab2e579f4bf01bff01695a3c46557f6c73f4 in / 
# Tue, 23 Aug 2022 01:02:00 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:28:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:28:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:29bf8f676853094720e43096224f2ec8a31ffa3752cf7a1e52fb9e72ae069480`  
		Last Modified: Tue, 23 Aug 2022 01:07:13 GMT  
		Size: 54.1 MB (54096938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0426ba96c16ee4ea8eb5b5322685d94b842c455938234d92ca07814c6ae081`  
		Last Modified: Tue, 23 Aug 2022 01:38:51 GMT  
		Size: 9.5 MB (9475146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86201f3e5308e2da4dad080700c08b4d6a0a02c265e56c7a0cdae2889f16b442`  
		Last Modified: Tue, 23 Aug 2022 01:38:51 GMT  
		Size: 11.5 MB (11473600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:aab0c69c14ce9ef03205d8e14af84b378de16c95451a791e6e33bb12746a53e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.8 MB (72821838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb89bf0a7e7dccfef6cd4f619698b29111d786ef44c4c96ae76088989fef2bb0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:09:18 GMT
ADD file:2b4a878ee82590d9ee2da01a2501742d21f6d050a0002f9bd484a4d7c8620d2e in / 
# Tue, 23 Aug 2022 00:09:23 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 22:12:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 22:13:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4b18e364c6342ca1244071a2f94edf42b92a5b7997d16df3b26467139f3f0603`  
		Last Modified: Tue, 23 Aug 2022 00:17:33 GMT  
		Size: 53.1 MB (53119349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5edf0a5e5947b8da11a8b58c48bd00dc43fe37b1375dd57214cc77b72c0bc009`  
		Last Modified: Tue, 23 Aug 2022 22:43:15 GMT  
		Size: 8.7 MB (8660383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd311acb344ec357f0aa8b600c00bac50d5489700c6ec00ff2ec71f10bf3789`  
		Last Modified: Tue, 23 Aug 2022 22:43:14 GMT  
		Size: 11.0 MB (11042106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:085f8dcab702213ca234e533f0d7c394b315c6558341fd0d71206dd815305279
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.3 MB (79262346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf0eeff677f73e0eec150a7ebe08f2cbd0fae801a6f253e6709522d4569a6163`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:23:48 GMT
ADD file:92444ce23c3227ef88446469c37fc41decda1ba975ddfb1be3e1ebb1e694471b in / 
# Tue, 23 Aug 2022 01:23:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:52:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:52:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a2d2f2c5b4e64eabb8a7632609e67883239433d932129bf478f7614059a9aabe`  
		Last Modified: Tue, 23 Aug 2022 01:29:05 GMT  
		Size: 57.3 MB (57289866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b43c7a1c5614eda4b722aada1632b2b42c7499b945bcd902a405d6811943e66`  
		Last Modified: Tue, 23 Aug 2022 02:08:15 GMT  
		Size: 9.9 MB (9888870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4983e94a7031bdb88baa08be05b8f42254ef49f65245663476650772c95d77`  
		Last Modified: Tue, 23 Aug 2022 02:08:15 GMT  
		Size: 12.1 MB (12083610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:fb68ac36160a91bfb4682cfdaef3cf44fb33fbf32c01d787a5adee5c5d70ae7c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.7 MB (71667220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca9c5e8d57f49cedaab70bf6f460b53ecd1b779bc00692d82088c8274aac7f3c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:53:14 GMT
ADD file:e8167229629003ac0dcc7f0bcc35a939121e9b4a88b67483883c2741f5415634 in / 
# Tue, 23 Aug 2022 00:53:16 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 09:49:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 09:49:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:bfa0b60dda37e3a2f71f5d19d0259a51a84ce3f8e9deff107720c9868e69769b`  
		Last Modified: Tue, 23 Aug 2022 00:57:59 GMT  
		Size: 51.6 MB (51559576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9f7dae28c5d2750f7a41520dc8fec8c6914c21a7ced6fbda8b32c01477bc57`  
		Last Modified: Tue, 23 Aug 2022 09:58:50 GMT  
		Size: 8.9 MB (8941068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a871302fe26c06a3669e3a3f80c6e947aba9fbecf2fddb59dfe0739cf8a3f48a`  
		Last Modified: Tue, 23 Aug 2022 09:58:50 GMT  
		Size: 11.2 MB (11166576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:testing-scm`

```console
$ docker pull buildpack-deps@sha256:9043c34b103e0c0c1c4e5bb7a18c064a3f5dc3c4823ab73e33c9e688f3e10dd6
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

### `buildpack-deps:testing-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:f679dfea28b543518362ad66cac6b1240302cdfc6f6253e1529bd0c0063f9ccb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.9 MB (130899946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5065f8a27ab438502224d3d8c878db108e01f3cc1d35cb19090300d6ba573049`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:15 GMT
ADD file:7507edfdf016128615e9ba278d471fd6d27c96436e543786b691c93b6f94b56b in / 
# Tue, 23 Aug 2022 00:20:16 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:46:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:46:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 00:46:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5e784af754e1c7855decd29b818520a98b5b539515cd7c199c5dbceb6cc4a45f`  
		Last Modified: Tue, 23 Aug 2022 00:23:57 GMT  
		Size: 52.7 MB (52725730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06352499c53ea1415d7d7121128de838e832cbc465b145c71d05fb7b74a91c0`  
		Last Modified: Tue, 23 Aug 2022 00:54:04 GMT  
		Size: 9.3 MB (9298815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e88fbc1ce3af2aec72e131f3b876f2554849f8d6291840fbaf61b24970e54c3`  
		Last Modified: Tue, 23 Aug 2022 00:54:04 GMT  
		Size: 11.3 MB (11272439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2afebddf0d45a19b246f4ff1ead1dd600b48cc494afd00873819774f29c6f388`  
		Last Modified: Tue, 23 Aug 2022 00:54:22 GMT  
		Size: 57.6 MB (57602962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:dc1c4e9ae95084f819ce284e2799135e73f0749ff86245301b5df7ab70a27a27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.8 MB (126785738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6df0ab6a1f8c5c5224f0b76a13da3b636bf824c3286b34e306e7a71fc9ba6ba0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:16:08 GMT
ADD file:dbc0c48f409cbe73d340bec8639492807b8c28fa6907379a17a958448dca1829 in / 
# Tue, 23 Aug 2022 01:16:08 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 06:16:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 06:16:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 06:16:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3204f8dd2e8fdf47391628664d2c96551393e3e0abd1e471abeb57296519c816`  
		Last Modified: Tue, 23 Aug 2022 01:21:24 GMT  
		Size: 51.8 MB (51814042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2edbed2d89089bed15e37327dce17d68521ccd0390a9172314785a01bb2918c5`  
		Last Modified: Tue, 23 Aug 2022 06:24:42 GMT  
		Size: 8.7 MB (8740375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ead884b6cf02ae26001f7fa32ee0d5127f5b1f36fe6d675bf0ab7b8b81baa00`  
		Last Modified: Tue, 23 Aug 2022 06:24:42 GMT  
		Size: 10.9 MB (10946896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e395af4802fa3dfe5d8dc10a19e4fb9ea0adaa8951ba0595e9c756a12d412bb8`  
		Last Modified: Tue, 23 Aug 2022 06:25:07 GMT  
		Size: 55.3 MB (55284425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:c50fdc3cc8971109d7e2fb62ae7f6e0654628f84a110f1113a842ee045e776ac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.9 MB (121871444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3aaa5ae4912b2de292b9affa365fa17be839dbd9222323714858cc9d901bb30`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:42:14 GMT
ADD file:590ff1916ed8a15a7a205153d20c2823a242c228573a1868134df4bdd95f10d8 in / 
# Tue, 23 Aug 2022 01:42:14 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 12:57:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 12:57:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 12:58:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b4a2cf95b2637a1520aeb527ca7569456a3bcf1d740f72cc418357cbe490704d`  
		Last Modified: Tue, 23 Aug 2022 01:48:45 GMT  
		Size: 49.6 MB (49555090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0a9319f004c20513b7f62d6d76d1b1959183b5ad5b488373ca6330a9d6797b`  
		Last Modified: Tue, 23 Aug 2022 13:09:50 GMT  
		Size: 8.4 MB (8402996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fd63a2d6ab83a6d913419cd2a446fc94d0d9a4c654bf2a3c13dfe3a7116609`  
		Last Modified: Tue, 23 Aug 2022 13:09:49 GMT  
		Size: 10.6 MB (10589855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c7d7ae465211d33c40484e48402566e419669463cab573010f1ab877df64a9`  
		Last Modified: Tue, 23 Aug 2022 13:10:16 GMT  
		Size: 53.3 MB (53323503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:0155117db9306b41c236e921e5f76a0bd743851a0ef03fdd0375580ad644862f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.8 MB (130809998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5866f5d0d44278637ed443b0e5d5a0e8b808d2c70c50503fc468ffa7d2bf8b13`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:51:53 GMT
ADD file:f94a576f262c4fcf5112164145c04850c826787b299878e7e126754d1211a51c in / 
# Tue, 23 Aug 2022 01:51:53 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:25:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:25:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 02:26:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7dd208a8a7339c037c691e6ace1cd3f94803ee4c17a3211b9ccadf01d1ff2ca9`  
		Last Modified: Tue, 23 Aug 2022 01:56:50 GMT  
		Size: 53.1 MB (53117563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a6d7761ab15abc5f27917ed7e543565cb302e30ac8bd10819c205f079ec603`  
		Last Modified: Tue, 23 Aug 2022 02:35:05 GMT  
		Size: 9.1 MB (9133938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d472709c6f5c8abe91373fba2db77fd3b0946f573269803173452485abc6ff8b`  
		Last Modified: Tue, 23 Aug 2022 02:35:05 GMT  
		Size: 11.1 MB (11062413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247b0fb5989ae9d485d4b97b959d16adfaeb2e92bf9a74bd8b1f677bb7f3e1c5`  
		Last Modified: Tue, 23 Aug 2022 02:35:25 GMT  
		Size: 57.5 MB (57496084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:1a6e04486d701fe9f175abed959a5794adb184ded2d14ea520fda84aa445ba9c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.1 MB (134148274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8346a4ca2444870e8bb65aff75d4d4cf6711229035f48bacd81de5aee6ec3ee`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:01:59 GMT
ADD file:1c8ebe8b69a2d3c236c8a947162fab2e579f4bf01bff01695a3c46557f6c73f4 in / 
# Tue, 23 Aug 2022 01:02:00 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:28:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:28:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:29:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:29bf8f676853094720e43096224f2ec8a31ffa3752cf7a1e52fb9e72ae069480`  
		Last Modified: Tue, 23 Aug 2022 01:07:13 GMT  
		Size: 54.1 MB (54096938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0426ba96c16ee4ea8eb5b5322685d94b842c455938234d92ca07814c6ae081`  
		Last Modified: Tue, 23 Aug 2022 01:38:51 GMT  
		Size: 9.5 MB (9475146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86201f3e5308e2da4dad080700c08b4d6a0a02c265e56c7a0cdae2889f16b442`  
		Last Modified: Tue, 23 Aug 2022 01:38:51 GMT  
		Size: 11.5 MB (11473600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4eae1a3c8a2b637c155af3a0e81b010eea8632db588e887a59f57d020ad81a8`  
		Last Modified: Tue, 23 Aug 2022 01:39:11 GMT  
		Size: 59.1 MB (59102590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:eeced580e9256e37c10c45f4f3ba1068a3eea3bb6380d105192d70491e16f28f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.3 MB (129276385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:955ae09e149c1e982f8e43e476d7d60341fcfcfc48248c24ef4c5b84e97d70be`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:09:18 GMT
ADD file:2b4a878ee82590d9ee2da01a2501742d21f6d050a0002f9bd484a4d7c8620d2e in / 
# Tue, 23 Aug 2022 00:09:23 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 22:12:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 22:13:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 22:15:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4b18e364c6342ca1244071a2f94edf42b92a5b7997d16df3b26467139f3f0603`  
		Last Modified: Tue, 23 Aug 2022 00:17:33 GMT  
		Size: 53.1 MB (53119349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5edf0a5e5947b8da11a8b58c48bd00dc43fe37b1375dd57214cc77b72c0bc009`  
		Last Modified: Tue, 23 Aug 2022 22:43:15 GMT  
		Size: 8.7 MB (8660383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd311acb344ec357f0aa8b600c00bac50d5489700c6ec00ff2ec71f10bf3789`  
		Last Modified: Tue, 23 Aug 2022 22:43:14 GMT  
		Size: 11.0 MB (11042106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6304e93b6d685763966db039d84593203f3027de2420ebe4cf0e2865b59ee64d`  
		Last Modified: Tue, 23 Aug 2022 22:44:05 GMT  
		Size: 56.5 MB (56454547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:1ae72a86df0538f6c86e6177acda8b42ac2b5bc5b16f91d75bd6dff1d570c92c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.7 MB (141681548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f9e0dbaf8822ad89bf60827cb4b2f3927b1784af8cc2d1ff24f2e790d144376`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:23:48 GMT
ADD file:92444ce23c3227ef88446469c37fc41decda1ba975ddfb1be3e1ebb1e694471b in / 
# Tue, 23 Aug 2022 01:23:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:52:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:52:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:53:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a2d2f2c5b4e64eabb8a7632609e67883239433d932129bf478f7614059a9aabe`  
		Last Modified: Tue, 23 Aug 2022 01:29:05 GMT  
		Size: 57.3 MB (57289866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b43c7a1c5614eda4b722aada1632b2b42c7499b945bcd902a405d6811943e66`  
		Last Modified: Tue, 23 Aug 2022 02:08:15 GMT  
		Size: 9.9 MB (9888870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4983e94a7031bdb88baa08be05b8f42254ef49f65245663476650772c95d77`  
		Last Modified: Tue, 23 Aug 2022 02:08:15 GMT  
		Size: 12.1 MB (12083610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea4205d8530bba3b66567e144b76048ea3deb5e2f1d3604690cc87c10af416f`  
		Last Modified: Tue, 23 Aug 2022 02:08:43 GMT  
		Size: 62.4 MB (62419202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a35ea6986151b6a9cfa303d6c7b88d34eb1efbdda23f410a313539d54216369d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.5 MB (128533488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49e0602dc9c0c8d0c36a03cf960026a77c297d6572bb13d8c27894d283bde270`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:53:14 GMT
ADD file:e8167229629003ac0dcc7f0bcc35a939121e9b4a88b67483883c2741f5415634 in / 
# Tue, 23 Aug 2022 00:53:16 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 09:49:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 09:49:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 09:49:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bfa0b60dda37e3a2f71f5d19d0259a51a84ce3f8e9deff107720c9868e69769b`  
		Last Modified: Tue, 23 Aug 2022 00:57:59 GMT  
		Size: 51.6 MB (51559576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9f7dae28c5d2750f7a41520dc8fec8c6914c21a7ced6fbda8b32c01477bc57`  
		Last Modified: Tue, 23 Aug 2022 09:58:50 GMT  
		Size: 8.9 MB (8941068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a871302fe26c06a3669e3a3f80c6e947aba9fbecf2fddb59dfe0739cf8a3f48a`  
		Last Modified: Tue, 23 Aug 2022 09:58:50 GMT  
		Size: 11.2 MB (11166576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f7f08e932daba42246e92ace2e6a7084e92eb623212ae6d100ba95f988439df`  
		Last Modified: Tue, 23 Aug 2022 09:59:04 GMT  
		Size: 56.9 MB (56866268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:unstable`

```console
$ docker pull buildpack-deps@sha256:8e69463fa7226b65fb3a87f7f7078af656db7fd85bf186caedee6d2ae574aacb
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
$ docker pull buildpack-deps@sha256:82d0d6d789a9d69e6ccfb63feae242155bb785aabec9d1e662cd8fc14bb54548
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **555.9 MB (555872054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9a609cc81c34f54d9832c5a0065808f39e2800dc81394bbdc99d0e1c4105fc7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:39 GMT
ADD file:0ded1ec762355d6c32b4a9f1eff5fbd5e60d15824d6bde678ef85cbdd03fe0ce in / 
# Tue, 23 Aug 2022 00:21:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:50:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:51:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 00:51:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:52:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6649fedb76d916c1041e321eca86994acdb4cd14cc61ef93b5d2a397c15af4ad`  
		Last Modified: Tue, 23 Aug 2022 00:26:41 GMT  
		Size: 52.8 MB (52768784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52383a4258951f21b40d1c18a5c708ecfd3cc7f76838fc8fbe3c1fa248f7b133`  
		Last Modified: Tue, 23 Aug 2022 00:57:51 GMT  
		Size: 9.3 MB (9302218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b8bf82596b529ddf3a818d599c3bed1bef1e54925ac4df0a1a6bf6467ce1bd2`  
		Last Modified: Tue, 23 Aug 2022 00:57:51 GMT  
		Size: 11.3 MB (11274041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f934be4bad0fbf951546a8aaa20f158e16a48d2a373a3b5cab06448c354bae14`  
		Last Modified: Tue, 23 Aug 2022 00:58:09 GMT  
		Size: 58.1 MB (58057519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a459942b0771eb68ff654a202259ff2306d2ca50d850f5595b425216a794380`  
		Last Modified: Tue, 23 Aug 2022 00:59:13 GMT  
		Size: 424.5 MB (424469492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:ae6debf772cd416d3418020d444b526e6dbb85caf44ec3d847d6ece14fdddbd5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.9 MB (313920314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:346d312be574d74cdc36cf1bba138bd96a787ab9df0c21436f66850af54f9485`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:17:35 GMT
ADD file:dd3257a03b58fae4238ad4fccb1c79ff49c76b1294f5fb6f57ecee4bb748c9ca in / 
# Tue, 23 Aug 2022 01:17:35 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 06:21:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 06:21:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 06:22:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 06:23:24 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4cd09bc891cabc28c38273b3b8e22a810888bfc449c6fd4ec5610c27492b2603`  
		Last Modified: Tue, 23 Aug 2022 01:23:14 GMT  
		Size: 51.9 MB (51911406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f224d9458f88dbd5a7ba922c9cb4a7116b314d234615e7981e233157663a02`  
		Last Modified: Tue, 23 Aug 2022 06:28:49 GMT  
		Size: 9.7 MB (9741837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f3836f63f5d9bf55c4350c9f89c9a7b420aa71f6408278b53d58e61634cb3fa`  
		Last Modified: Tue, 23 Aug 2022 06:28:49 GMT  
		Size: 10.9 MB (10949073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c127ba25c98f2eef6419ecfbb5bb63c8da103c1ea0298e7e61e2103424e530a`  
		Last Modified: Tue, 23 Aug 2022 06:29:16 GMT  
		Size: 55.7 MB (55747826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e249ad29978f097d481f4bfe9ce42ca0c44552bf26944aea2b847496fd0838`  
		Last Modified: Tue, 23 Aug 2022 06:30:09 GMT  
		Size: 185.6 MB (185570172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:fd0b31ddb28465a985e9b4e90815a6fa47d188e9408ecf7c3d5c831fcfc241dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.8 MB (299844414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72da89b2937b052cd65b23069be33ca9069f1824886bb639b596cf2a764aecb3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:44:30 GMT
ADD file:63335401d9730857a474088e836b58820d062d53a4d008379a3f0bab91891ee7 in / 
# Tue, 23 Aug 2022 01:44:30 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 13:04:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:04:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 13:04:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:05:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:abce9a6a026c05f336d24d7c79af29d2f108767252a4737864125c7cd16cb946`  
		Last Modified: Tue, 23 Aug 2022 01:52:08 GMT  
		Size: 49.6 MB (49637416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:789e63ee7b15faa5255a98e78ca57f7b79165de31d27f0d20a810e2e8f2f6fbe`  
		Last Modified: Tue, 23 Aug 2022 13:15:09 GMT  
		Size: 8.4 MB (8404984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866f5f3461f124a4ec2d43c116d5e4f8a2783872d85516deec64b8873fb850ab`  
		Last Modified: Tue, 23 Aug 2022 13:15:09 GMT  
		Size: 10.6 MB (10590651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519438e1fee2b230fe7b1ef7d878f221dfd76d39406a621b5ac5c6a6d9977d8d`  
		Last Modified: Tue, 23 Aug 2022 13:15:36 GMT  
		Size: 53.7 MB (53721931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116396eb184bdf4a369bbff811214de4b5044eb77672394f3d62ce8fd8b07b69`  
		Last Modified: Tue, 23 Aug 2022 13:16:25 GMT  
		Size: 177.5 MB (177489432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:bcb381e04a2732ab250a0bc43cf4a8661b7020a0b532d7bfd5bcfdd5b4366c62
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **545.4 MB (545439369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18475cf95c9af1adee7cf3b17f92a8afed4f8d29ce264fe5b1d9f71f49b05775`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:53:33 GMT
ADD file:03a6abbfc4f7f5b036b595b68d32dab2760788223365adbadd691cc6b97d3f9f in / 
# Tue, 23 Aug 2022 01:53:34 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:30:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:30:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 02:31:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:32:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11a10710f625b85736b19b89ebf063edde4e3f2dedab0a6cc94db39e134d8cfe`  
		Last Modified: Tue, 23 Aug 2022 01:59:52 GMT  
		Size: 53.2 MB (53220635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d52438f7d6f6695685610119446105c5c9522703362332bff254bc8eda29485`  
		Last Modified: Tue, 23 Aug 2022 02:39:08 GMT  
		Size: 9.1 MB (9135715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c781af42aca050a89e2c2b2ae998b642dd1e62096b74d1479568d49d2b43581`  
		Last Modified: Tue, 23 Aug 2022 02:39:08 GMT  
		Size: 11.1 MB (11058895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b655e4c924d786599e6214f6298b4a90d6bb1e4e1bc66096185648662d73d55`  
		Last Modified: Tue, 23 Aug 2022 02:39:29 GMT  
		Size: 57.9 MB (57942074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4468d1c3ff674531ee48a976061d1c38abad49092b9887b6d908ec3376e65abc`  
		Last Modified: Tue, 23 Aug 2022 02:40:35 GMT  
		Size: 414.1 MB (414082050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8cd9f265050b2a89f2b0e789b66ee74878574934646dae66d370dbb1631b95b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.1 MB (349084797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6f5e1d87a25966aa07a6b1a0ddb507d3f52fec56499334037cc0df2fff4cf09`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:03:44 GMT
ADD file:56a765ed5b9c59576a105c4e82da61f928406a2ef950e7cada80b5c269a1acda in / 
# Tue, 23 Aug 2022 01:03:44 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:35:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:35:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:36:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:37:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:05690d5133887cdda89e6ae4808c08e8a92acf2163ce992d8bacbed497b1ddd7`  
		Last Modified: Tue, 23 Aug 2022 01:10:25 GMT  
		Size: 54.1 MB (54133693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6de5521fae7f54e276230f1136f3c889618c53b37f387bcb06db2c09c9ea96`  
		Last Modified: Tue, 23 Aug 2022 01:42:35 GMT  
		Size: 9.5 MB (9480147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1ad46fde87250408a791d37517179cd6427cd46421e84e138f00437a005cc8`  
		Last Modified: Tue, 23 Aug 2022 01:42:35 GMT  
		Size: 11.5 MB (11473735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc96324d4abcfddd315fc320b0f834fa9ab7e220e914962ae1d8af8c95bc0b94`  
		Last Modified: Tue, 23 Aug 2022 01:42:56 GMT  
		Size: 59.7 MB (59690126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3314db2a67edcee49b0f6254dd94eccdab07b0b303150ecab178769c20454ef8`  
		Last Modified: Tue, 23 Aug 2022 01:43:32 GMT  
		Size: 214.3 MB (214307096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:44932d5ac5c7c5b4769849503ca026630ef64ad261f181908e37e315f4a6a562
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.8 MB (321764495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aaf48cd27b846d1c74c094bed63d9fc6bdcad9711050ce213db2592c1f435d3f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:11:52 GMT
ADD file:372730632835dde60a084d1dc5d1d8d7840a118d3aa6413f1568d2a939e39e05 in / 
# Tue, 23 Aug 2022 00:11:58 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 22:34:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 22:34:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 22:36:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 22:42:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f6fdf476c348ab651944f6f008015e5c5184fa9f5620904fc65599b044dd5761`  
		Last Modified: Tue, 23 Aug 2022 00:20:20 GMT  
		Size: 53.2 MB (53216630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f889c0bad3c21c23d5613d840cb6194f047e7bd8b0ab913aa4c3aeb3f22ff6aa`  
		Last Modified: Tue, 23 Aug 2022 22:52:22 GMT  
		Size: 8.7 MB (8666700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e682c1b586301933075fc1a74ded2cb91e71a70eb9e075ab5291aec1d56e833`  
		Last Modified: Tue, 23 Aug 2022 22:52:22 GMT  
		Size: 11.0 MB (11041861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec7b75657e271145b112803a3b136f6eba775667758887ede8d7bf5eea806dd`  
		Last Modified: Tue, 23 Aug 2022 22:53:13 GMT  
		Size: 56.9 MB (56881826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ccde40f554bb70ef53d85d915e58944b5bde8dea04124f47de1cc710a908bde`  
		Last Modified: Tue, 23 Aug 2022 22:55:22 GMT  
		Size: 192.0 MB (191957478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d31682460f32ab995f6123d1861469234e2e9cec6e306c62c4947a3ae5e3d32c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **553.9 MB (553947352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e93f9fd28ad6ce94afa2ae176b65b01afb61979bba69a588a1f8caa26f8dc039`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:25:10 GMT
ADD file:7b8a9c1fc05e75d845ea719c57047ae432cceb7645d270a99b117d0e4e0ffb33 in / 
# Tue, 23 Aug 2022 01:25:13 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:02:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:02:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 02:02:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:05:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:515f00ecba82250b75d6d9987193afd77293c07bfaf7a95ae024c05c73a8cb3a`  
		Last Modified: Tue, 23 Aug 2022 01:31:07 GMT  
		Size: 57.3 MB (57313882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759d55c9749119adb9c0cff41513f89896055da109781a9c493c462426691120`  
		Last Modified: Tue, 23 Aug 2022 02:12:40 GMT  
		Size: 9.9 MB (9892227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419401365d91198049a8c6620087ce51a751ce8891e8a184d06c31216b0773b8`  
		Last Modified: Tue, 23 Aug 2022 02:12:40 GMT  
		Size: 12.1 MB (12081297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e6911c1af381860ef781b5463a576d34cf58ff5ca18e69333ab7d054a1d2a4`  
		Last Modified: Tue, 23 Aug 2022 02:13:10 GMT  
		Size: 62.9 MB (62860983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d3b983d1afeef2ed30145913f73fdca87605ede854ebf973821980ed7bb889`  
		Last Modified: Tue, 23 Aug 2022 02:14:53 GMT  
		Size: 411.8 MB (411798963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:89615e24846bec4e9c2210ffa40781e7fe3b0bb100785fb53d9f3d9771959639
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.2 MB (355224975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64060694992efd7dc9bad5501308cc2bafe39fcf7438d5a09721771171d1ed27`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:12:03 GMT
ADD file:beb3c4d0f1887ccbbe2b266a156b7658d2e1d7d48cbcd416a0410554dfafdf12 in / 
# Tue, 23 Aug 2022 00:12:06 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:58:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:59:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:03:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:12:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11998c1ffc96119253ef35ecbcfd66c2cb0d69f51a294f603a54496ec02d329c`  
		Last Modified: Tue, 23 Aug 2022 00:30:27 GMT  
		Size: 49.3 MB (49268189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237ee2e31cf68d3cd2675680cbf1e3c574c76f74440375dc1b8c1ad1d3d9768e`  
		Last Modified: Tue, 23 Aug 2022 01:41:12 GMT  
		Size: 8.4 MB (8399080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69eb487c5f4d1ba65732a0b11d3a69780177b7ed0357581fce4eb347813a643`  
		Last Modified: Tue, 23 Aug 2022 01:41:12 GMT  
		Size: 10.7 MB (10659901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3572ed314e6c0604916ece49e3a546ec2fcc60391daae870152b56b8fdc14d98`  
		Last Modified: Tue, 23 Aug 2022 01:43:43 GMT  
		Size: 54.0 MB (54034717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a20268cb682347428f2402e200fcf1a6f64026d72fa43eb8b171c47218c4e398`  
		Last Modified: Tue, 23 Aug 2022 01:51:06 GMT  
		Size: 232.9 MB (232863088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3380f5eb469b98e12046ee103b120a9bc84afb65a17f38812751e1b32fd6da22
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **499.2 MB (499173410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76a19518653a77d77c1c607b119f24c614cdd67c4fdc9f27f4385f192cc0ed7a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:54:14 GMT
ADD file:fb4926c73b650f18bc1eb6b58287dc0872251073fd0bc72bcd007f74315f89a5 in / 
# Tue, 23 Aug 2022 00:54:17 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 09:53:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 09:53:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 09:53:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 09:55:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0aaf3bb8cf1626ddbd85331fa1967c48ccf9d314270b99a2a506e53979592f79`  
		Last Modified: Tue, 23 Aug 2022 01:06:53 GMT  
		Size: 51.6 MB (51581993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b9f9f1f0cb3b7d4b45cdcacf5c7c93102c09bc71207f7dcc091136f732a622`  
		Last Modified: Tue, 23 Aug 2022 10:01:01 GMT  
		Size: 8.9 MB (8943771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06f6fca0053787f32630628512d8ae3f948e6ae085840b8a4083d3ac745fa220`  
		Last Modified: Tue, 23 Aug 2022 10:01:01 GMT  
		Size: 11.2 MB (11168320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e0960b87cafae9e1bf612df6c73bfb7680cbb0139fd149d5c6e367e797b282`  
		Last Modified: Tue, 23 Aug 2022 10:01:16 GMT  
		Size: 57.2 MB (57210664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886ef7d8187dc34f74cbea7c999fbf59f6940f6f469d36dc12cf47527ef36d7a`  
		Last Modified: Tue, 23 Aug 2022 10:02:03 GMT  
		Size: 370.3 MB (370268662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:unstable-curl`

```console
$ docker pull buildpack-deps@sha256:2c2b158aa817c9ae49deea0883bdabc17121d369094e2fed9ee04fc774bf96e8
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
$ docker pull buildpack-deps@sha256:12348240e5db18afa70f6382420fb3e36194a640ffa7f21e5506ded546ce702b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.3 MB (73345043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:801581c78b136e899df5cbff068467129f0d26f6e4add3126d2743694757cdae`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:39 GMT
ADD file:0ded1ec762355d6c32b4a9f1eff5fbd5e60d15824d6bde678ef85cbdd03fe0ce in / 
# Tue, 23 Aug 2022 00:21:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:50:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:51:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6649fedb76d916c1041e321eca86994acdb4cd14cc61ef93b5d2a397c15af4ad`  
		Last Modified: Tue, 23 Aug 2022 00:26:41 GMT  
		Size: 52.8 MB (52768784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52383a4258951f21b40d1c18a5c708ecfd3cc7f76838fc8fbe3c1fa248f7b133`  
		Last Modified: Tue, 23 Aug 2022 00:57:51 GMT  
		Size: 9.3 MB (9302218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b8bf82596b529ddf3a818d599c3bed1bef1e54925ac4df0a1a6bf6467ce1bd2`  
		Last Modified: Tue, 23 Aug 2022 00:57:51 GMT  
		Size: 11.3 MB (11274041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:7e705bb79460fdbd230d3b523f243f8fa47269ea192646175d4ec2f6b702919a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.6 MB (72602316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e605e3949595a62e6b4bf7d42c0fba0c62626c32603d8f5140d390cbf511380`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:17:35 GMT
ADD file:dd3257a03b58fae4238ad4fccb1c79ff49c76b1294f5fb6f57ecee4bb748c9ca in / 
# Tue, 23 Aug 2022 01:17:35 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 06:21:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 06:21:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4cd09bc891cabc28c38273b3b8e22a810888bfc449c6fd4ec5610c27492b2603`  
		Last Modified: Tue, 23 Aug 2022 01:23:14 GMT  
		Size: 51.9 MB (51911406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f224d9458f88dbd5a7ba922c9cb4a7116b314d234615e7981e233157663a02`  
		Last Modified: Tue, 23 Aug 2022 06:28:49 GMT  
		Size: 9.7 MB (9741837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f3836f63f5d9bf55c4350c9f89c9a7b420aa71f6408278b53d58e61634cb3fa`  
		Last Modified: Tue, 23 Aug 2022 06:28:49 GMT  
		Size: 10.9 MB (10949073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f43c56203997827c84a812462131cbcabc3e4c180f62c92a48595e4fcb79d54d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.6 MB (68633051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b20f50e4edf8c204581294078d6e224f677aad50fc3c310742b2ecb5b6bc19d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:44:30 GMT
ADD file:63335401d9730857a474088e836b58820d062d53a4d008379a3f0bab91891ee7 in / 
# Tue, 23 Aug 2022 01:44:30 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 13:04:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:04:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:abce9a6a026c05f336d24d7c79af29d2f108767252a4737864125c7cd16cb946`  
		Last Modified: Tue, 23 Aug 2022 01:52:08 GMT  
		Size: 49.6 MB (49637416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:789e63ee7b15faa5255a98e78ca57f7b79165de31d27f0d20a810e2e8f2f6fbe`  
		Last Modified: Tue, 23 Aug 2022 13:15:09 GMT  
		Size: 8.4 MB (8404984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866f5f3461f124a4ec2d43c116d5e4f8a2783872d85516deec64b8873fb850ab`  
		Last Modified: Tue, 23 Aug 2022 13:15:09 GMT  
		Size: 10.6 MB (10590651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7111671eb5e0eef153034060931fed251bc35454d67eaef764d41b8418bd55ea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.4 MB (73415245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da1f6b44edf551616f54c76b94273bb6cf38ac811641321690130bd55af523ff`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:53:33 GMT
ADD file:03a6abbfc4f7f5b036b595b68d32dab2760788223365adbadd691cc6b97d3f9f in / 
# Tue, 23 Aug 2022 01:53:34 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:30:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:30:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:11a10710f625b85736b19b89ebf063edde4e3f2dedab0a6cc94db39e134d8cfe`  
		Last Modified: Tue, 23 Aug 2022 01:59:52 GMT  
		Size: 53.2 MB (53220635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d52438f7d6f6695685610119446105c5c9522703362332bff254bc8eda29485`  
		Last Modified: Tue, 23 Aug 2022 02:39:08 GMT  
		Size: 9.1 MB (9135715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c781af42aca050a89e2c2b2ae998b642dd1e62096b74d1479568d49d2b43581`  
		Last Modified: Tue, 23 Aug 2022 02:39:08 GMT  
		Size: 11.1 MB (11058895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:b9972c98ff602f317e6304009068bc0bcfd55766be4faadef16a50f2e560ac0c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75087575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be006906138be6be28f63d53b6777210491d213b2fd95065a1fd6ca582699aad`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:03:44 GMT
ADD file:56a765ed5b9c59576a105c4e82da61f928406a2ef950e7cada80b5c269a1acda in / 
# Tue, 23 Aug 2022 01:03:44 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:35:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:35:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:05690d5133887cdda89e6ae4808c08e8a92acf2163ce992d8bacbed497b1ddd7`  
		Last Modified: Tue, 23 Aug 2022 01:10:25 GMT  
		Size: 54.1 MB (54133693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6de5521fae7f54e276230f1136f3c889618c53b37f387bcb06db2c09c9ea96`  
		Last Modified: Tue, 23 Aug 2022 01:42:35 GMT  
		Size: 9.5 MB (9480147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1ad46fde87250408a791d37517179cd6427cd46421e84e138f00437a005cc8`  
		Last Modified: Tue, 23 Aug 2022 01:42:35 GMT  
		Size: 11.5 MB (11473735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:d3bb18f79fd404a72bba015d8e68e173f0847657b212851c7a0f5d1b220fc766
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72925191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19c1d92b28bfc5686ba778c734dd92a01728841f6f7752e82c98666ac2c064eb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:11:52 GMT
ADD file:372730632835dde60a084d1dc5d1d8d7840a118d3aa6413f1568d2a939e39e05 in / 
# Tue, 23 Aug 2022 00:11:58 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 22:34:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 22:34:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f6fdf476c348ab651944f6f008015e5c5184fa9f5620904fc65599b044dd5761`  
		Last Modified: Tue, 23 Aug 2022 00:20:20 GMT  
		Size: 53.2 MB (53216630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f889c0bad3c21c23d5613d840cb6194f047e7bd8b0ab913aa4c3aeb3f22ff6aa`  
		Last Modified: Tue, 23 Aug 2022 22:52:22 GMT  
		Size: 8.7 MB (8666700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e682c1b586301933075fc1a74ded2cb91e71a70eb9e075ab5291aec1d56e833`  
		Last Modified: Tue, 23 Aug 2022 22:52:22 GMT  
		Size: 11.0 MB (11041861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:9976e80bc902f0a0e9be54ffe69853a518388672975e91a0dbca9cc51685422b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.3 MB (79287406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a04e630b9a2c28f96e8087ed577aa1796b005fda82c5be6b82cc21d1cfc58d35`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:25:10 GMT
ADD file:7b8a9c1fc05e75d845ea719c57047ae432cceb7645d270a99b117d0e4e0ffb33 in / 
# Tue, 23 Aug 2022 01:25:13 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:02:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:02:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:515f00ecba82250b75d6d9987193afd77293c07bfaf7a95ae024c05c73a8cb3a`  
		Last Modified: Tue, 23 Aug 2022 01:31:07 GMT  
		Size: 57.3 MB (57313882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759d55c9749119adb9c0cff41513f89896055da109781a9c493c462426691120`  
		Last Modified: Tue, 23 Aug 2022 02:12:40 GMT  
		Size: 9.9 MB (9892227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419401365d91198049a8c6620087ce51a751ce8891e8a184d06c31216b0773b8`  
		Last Modified: Tue, 23 Aug 2022 02:12:40 GMT  
		Size: 12.1 MB (12081297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:7190f1576496c38d326bf20b45a9725d2c7888724774b79fa03f1ad5fdb68d29
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68327170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cbcd3644b4a571e4579adbe4eb08af38c965c5986789fdd1a493de8456457e7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:12:03 GMT
ADD file:beb3c4d0f1887ccbbe2b266a156b7658d2e1d7d48cbcd416a0410554dfafdf12 in / 
# Tue, 23 Aug 2022 00:12:06 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:58:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:59:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:11998c1ffc96119253ef35ecbcfd66c2cb0d69f51a294f603a54496ec02d329c`  
		Last Modified: Tue, 23 Aug 2022 00:30:27 GMT  
		Size: 49.3 MB (49268189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237ee2e31cf68d3cd2675680cbf1e3c574c76f74440375dc1b8c1ad1d3d9768e`  
		Last Modified: Tue, 23 Aug 2022 01:41:12 GMT  
		Size: 8.4 MB (8399080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69eb487c5f4d1ba65732a0b11d3a69780177b7ed0357581fce4eb347813a643`  
		Last Modified: Tue, 23 Aug 2022 01:41:12 GMT  
		Size: 10.7 MB (10659901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:50db63bb1dd307a64611a08c3833204bb5702151e0f7d673c4f54195b8df8703
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.7 MB (71694084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d47eb8f13f6cb432056c3dcae6141ef753599747fb62444f57a70249abe219a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:54:14 GMT
ADD file:fb4926c73b650f18bc1eb6b58287dc0872251073fd0bc72bcd007f74315f89a5 in / 
# Tue, 23 Aug 2022 00:54:17 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 09:53:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 09:53:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0aaf3bb8cf1626ddbd85331fa1967c48ccf9d314270b99a2a506e53979592f79`  
		Last Modified: Tue, 23 Aug 2022 01:06:53 GMT  
		Size: 51.6 MB (51581993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b9f9f1f0cb3b7d4b45cdcacf5c7c93102c09bc71207f7dcc091136f732a622`  
		Last Modified: Tue, 23 Aug 2022 10:01:01 GMT  
		Size: 8.9 MB (8943771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06f6fca0053787f32630628512d8ae3f948e6ae085840b8a4083d3ac745fa220`  
		Last Modified: Tue, 23 Aug 2022 10:01:01 GMT  
		Size: 11.2 MB (11168320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:unstable-scm`

```console
$ docker pull buildpack-deps@sha256:25fb1b2c0fe84aea81ddd7f0198b4230e3d91d45d975200e2360f8d7ae5d0299
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
$ docker pull buildpack-deps@sha256:f6ff780ff6d9dd4454e7164151b28d72f3fcf1bba471138ce4e1f431bd71e0fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131402562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc7f6c028fa86c7a1118b95cde5cb96316d9cacaa46a358a82613050902e582f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:39 GMT
ADD file:0ded1ec762355d6c32b4a9f1eff5fbd5e60d15824d6bde678ef85cbdd03fe0ce in / 
# Tue, 23 Aug 2022 00:21:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:50:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:51:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 00:51:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6649fedb76d916c1041e321eca86994acdb4cd14cc61ef93b5d2a397c15af4ad`  
		Last Modified: Tue, 23 Aug 2022 00:26:41 GMT  
		Size: 52.8 MB (52768784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52383a4258951f21b40d1c18a5c708ecfd3cc7f76838fc8fbe3c1fa248f7b133`  
		Last Modified: Tue, 23 Aug 2022 00:57:51 GMT  
		Size: 9.3 MB (9302218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b8bf82596b529ddf3a818d599c3bed1bef1e54925ac4df0a1a6bf6467ce1bd2`  
		Last Modified: Tue, 23 Aug 2022 00:57:51 GMT  
		Size: 11.3 MB (11274041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f934be4bad0fbf951546a8aaa20f158e16a48d2a373a3b5cab06448c354bae14`  
		Last Modified: Tue, 23 Aug 2022 00:58:09 GMT  
		Size: 58.1 MB (58057519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:828273289b0de4086367b7a3b69cf9cc5c9b5626734cbe7a0f443b9cd4a7e17f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128350142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7a2de47491cc492dfcb63ab018b93f64814b3df048f39124c93f004890e9816`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:17:35 GMT
ADD file:dd3257a03b58fae4238ad4fccb1c79ff49c76b1294f5fb6f57ecee4bb748c9ca in / 
# Tue, 23 Aug 2022 01:17:35 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 06:21:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 06:21:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 06:22:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4cd09bc891cabc28c38273b3b8e22a810888bfc449c6fd4ec5610c27492b2603`  
		Last Modified: Tue, 23 Aug 2022 01:23:14 GMT  
		Size: 51.9 MB (51911406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f224d9458f88dbd5a7ba922c9cb4a7116b314d234615e7981e233157663a02`  
		Last Modified: Tue, 23 Aug 2022 06:28:49 GMT  
		Size: 9.7 MB (9741837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f3836f63f5d9bf55c4350c9f89c9a7b420aa71f6408278b53d58e61634cb3fa`  
		Last Modified: Tue, 23 Aug 2022 06:28:49 GMT  
		Size: 10.9 MB (10949073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c127ba25c98f2eef6419ecfbb5bb63c8da103c1ea0298e7e61e2103424e530a`  
		Last Modified: Tue, 23 Aug 2022 06:29:16 GMT  
		Size: 55.7 MB (55747826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:fb4ae2b3214297ac6d789a817eb1f7610877481f6df43185bf978d295af721f2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.4 MB (122354982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:557ea0b235bd6f860583a55f4497eed0f630571ffe0b0f59f2ad807883bdf7fd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:44:30 GMT
ADD file:63335401d9730857a474088e836b58820d062d53a4d008379a3f0bab91891ee7 in / 
# Tue, 23 Aug 2022 01:44:30 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 13:04:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:04:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 13:04:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:abce9a6a026c05f336d24d7c79af29d2f108767252a4737864125c7cd16cb946`  
		Last Modified: Tue, 23 Aug 2022 01:52:08 GMT  
		Size: 49.6 MB (49637416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:789e63ee7b15faa5255a98e78ca57f7b79165de31d27f0d20a810e2e8f2f6fbe`  
		Last Modified: Tue, 23 Aug 2022 13:15:09 GMT  
		Size: 8.4 MB (8404984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866f5f3461f124a4ec2d43c116d5e4f8a2783872d85516deec64b8873fb850ab`  
		Last Modified: Tue, 23 Aug 2022 13:15:09 GMT  
		Size: 10.6 MB (10590651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519438e1fee2b230fe7b1ef7d878f221dfd76d39406a621b5ac5c6a6d9977d8d`  
		Last Modified: Tue, 23 Aug 2022 13:15:36 GMT  
		Size: 53.7 MB (53721931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:5a4db913aac724bda8dd2b3efd88e4f9a857398e53462cf785726255553e308d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131357319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3624daf2816b207400e142ee555d194f1d07f91d0a35b5c3171ebd64b7756427`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:53:33 GMT
ADD file:03a6abbfc4f7f5b036b595b68d32dab2760788223365adbadd691cc6b97d3f9f in / 
# Tue, 23 Aug 2022 01:53:34 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:30:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:30:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 02:31:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11a10710f625b85736b19b89ebf063edde4e3f2dedab0a6cc94db39e134d8cfe`  
		Last Modified: Tue, 23 Aug 2022 01:59:52 GMT  
		Size: 53.2 MB (53220635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d52438f7d6f6695685610119446105c5c9522703362332bff254bc8eda29485`  
		Last Modified: Tue, 23 Aug 2022 02:39:08 GMT  
		Size: 9.1 MB (9135715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c781af42aca050a89e2c2b2ae998b642dd1e62096b74d1479568d49d2b43581`  
		Last Modified: Tue, 23 Aug 2022 02:39:08 GMT  
		Size: 11.1 MB (11058895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b655e4c924d786599e6214f6298b4a90d6bb1e4e1bc66096185648662d73d55`  
		Last Modified: Tue, 23 Aug 2022 02:39:29 GMT  
		Size: 57.9 MB (57942074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:f05820f89144ef9fd4abdfa7b091a362e96a5babc1bd7fdded96cbb6445f5d8a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134777701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6899c125d79e1d6f8e0f13938a0ff7560906f0008d90fe875828e8d43f0015c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:03:44 GMT
ADD file:56a765ed5b9c59576a105c4e82da61f928406a2ef950e7cada80b5c269a1acda in / 
# Tue, 23 Aug 2022 01:03:44 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:35:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:35:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:36:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:05690d5133887cdda89e6ae4808c08e8a92acf2163ce992d8bacbed497b1ddd7`  
		Last Modified: Tue, 23 Aug 2022 01:10:25 GMT  
		Size: 54.1 MB (54133693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6de5521fae7f54e276230f1136f3c889618c53b37f387bcb06db2c09c9ea96`  
		Last Modified: Tue, 23 Aug 2022 01:42:35 GMT  
		Size: 9.5 MB (9480147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1ad46fde87250408a791d37517179cd6427cd46421e84e138f00437a005cc8`  
		Last Modified: Tue, 23 Aug 2022 01:42:35 GMT  
		Size: 11.5 MB (11473735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc96324d4abcfddd315fc320b0f834fa9ab7e220e914962ae1d8af8c95bc0b94`  
		Last Modified: Tue, 23 Aug 2022 01:42:56 GMT  
		Size: 59.7 MB (59690126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:4e25ae1bf979ce1f69096bcd3e8f9ac3b8c550a178e0af25ae5a182daf2b0f54
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.8 MB (129807017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2ddf6775bb37c49535b4cb27950a7b00495f73c343f2e41f1a1a773c7d713b8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:11:52 GMT
ADD file:372730632835dde60a084d1dc5d1d8d7840a118d3aa6413f1568d2a939e39e05 in / 
# Tue, 23 Aug 2022 00:11:58 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 22:34:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 22:34:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 22:36:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f6fdf476c348ab651944f6f008015e5c5184fa9f5620904fc65599b044dd5761`  
		Last Modified: Tue, 23 Aug 2022 00:20:20 GMT  
		Size: 53.2 MB (53216630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f889c0bad3c21c23d5613d840cb6194f047e7bd8b0ab913aa4c3aeb3f22ff6aa`  
		Last Modified: Tue, 23 Aug 2022 22:52:22 GMT  
		Size: 8.7 MB (8666700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e682c1b586301933075fc1a74ded2cb91e71a70eb9e075ab5291aec1d56e833`  
		Last Modified: Tue, 23 Aug 2022 22:52:22 GMT  
		Size: 11.0 MB (11041861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec7b75657e271145b112803a3b136f6eba775667758887ede8d7bf5eea806dd`  
		Last Modified: Tue, 23 Aug 2022 22:53:13 GMT  
		Size: 56.9 MB (56881826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:2b57718c40c4dfbfea62c154561c7314a5707ffbcf1dcc3f8f7974ed65dd3a89
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.1 MB (142148389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb381662ef1287437ee731fea51ff6067edeae2ec813e3a8b51449c3e83feeb5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:25:10 GMT
ADD file:7b8a9c1fc05e75d845ea719c57047ae432cceb7645d270a99b117d0e4e0ffb33 in / 
# Tue, 23 Aug 2022 01:25:13 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:02:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:02:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 02:02:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:515f00ecba82250b75d6d9987193afd77293c07bfaf7a95ae024c05c73a8cb3a`  
		Last Modified: Tue, 23 Aug 2022 01:31:07 GMT  
		Size: 57.3 MB (57313882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759d55c9749119adb9c0cff41513f89896055da109781a9c493c462426691120`  
		Last Modified: Tue, 23 Aug 2022 02:12:40 GMT  
		Size: 9.9 MB (9892227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419401365d91198049a8c6620087ce51a751ce8891e8a184d06c31216b0773b8`  
		Last Modified: Tue, 23 Aug 2022 02:12:40 GMT  
		Size: 12.1 MB (12081297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e6911c1af381860ef781b5463a576d34cf58ff5ca18e69333ab7d054a1d2a4`  
		Last Modified: Tue, 23 Aug 2022 02:13:10 GMT  
		Size: 62.9 MB (62860983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:ef05116e1aa3a68409adae7bc8bacbfc541ba80ea3cf9d4557f97931554d87b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.4 MB (122361887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f5da8a1feed0041190f96478c8ee800f1bd726c679e418e5a63f437c015ba7a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:12:03 GMT
ADD file:beb3c4d0f1887ccbbe2b266a156b7658d2e1d7d48cbcd416a0410554dfafdf12 in / 
# Tue, 23 Aug 2022 00:12:06 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:58:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:59:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:03:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11998c1ffc96119253ef35ecbcfd66c2cb0d69f51a294f603a54496ec02d329c`  
		Last Modified: Tue, 23 Aug 2022 00:30:27 GMT  
		Size: 49.3 MB (49268189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237ee2e31cf68d3cd2675680cbf1e3c574c76f74440375dc1b8c1ad1d3d9768e`  
		Last Modified: Tue, 23 Aug 2022 01:41:12 GMT  
		Size: 8.4 MB (8399080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69eb487c5f4d1ba65732a0b11d3a69780177b7ed0357581fce4eb347813a643`  
		Last Modified: Tue, 23 Aug 2022 01:41:12 GMT  
		Size: 10.7 MB (10659901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3572ed314e6c0604916ece49e3a546ec2fcc60391daae870152b56b8fdc14d98`  
		Last Modified: Tue, 23 Aug 2022 01:43:43 GMT  
		Size: 54.0 MB (54034717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:e90082389e99fc0e36884fc39fd1e58adf5ea389206304aeb314cd3bfcacbdde
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128904748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78d58a2c0b5135494685dd4ff3219ecacf7cdcb28a9f029b266828306d0a71fc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:54:14 GMT
ADD file:fb4926c73b650f18bc1eb6b58287dc0872251073fd0bc72bcd007f74315f89a5 in / 
# Tue, 23 Aug 2022 00:54:17 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 09:53:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 09:53:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 09:53:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0aaf3bb8cf1626ddbd85331fa1967c48ccf9d314270b99a2a506e53979592f79`  
		Last Modified: Tue, 23 Aug 2022 01:06:53 GMT  
		Size: 51.6 MB (51581993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b9f9f1f0cb3b7d4b45cdcacf5c7c93102c09bc71207f7dcc091136f732a622`  
		Last Modified: Tue, 23 Aug 2022 10:01:01 GMT  
		Size: 8.9 MB (8943771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06f6fca0053787f32630628512d8ae3f948e6ae085840b8a4083d3ac745fa220`  
		Last Modified: Tue, 23 Aug 2022 10:01:01 GMT  
		Size: 11.2 MB (11168320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e0960b87cafae9e1bf612df6c73bfb7680cbb0139fd149d5c6e367e797b282`  
		Last Modified: Tue, 23 Aug 2022 10:01:16 GMT  
		Size: 57.2 MB (57210664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:xenial`

```console
$ docker pull buildpack-deps@sha256:efffef05dadcc74834c6b4eb5c916ee03a62d315e1a38b0d52e2e442ac55d119
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
$ docker pull buildpack-deps@sha256:324cae93bc58f79fb9a0ce73a3f358bb214f120bf4b20b1605f4d363cd84e71c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.4 MB (202397646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f9369fe76ef4d2ec8e85f2b5f60d860dcaec95b99b6a95200bbc1bd1e4fed6d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:41:46 GMT
ADD file:294a94a081de785c730003a440a0530a85add2bcb60c0f5bc4ce7ee17867ac4e in / 
# Tue, 02 Aug 2022 01:41:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 02 Aug 2022 01:41:48 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:41:49 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 02 Aug 2022 01:41:49 GMT
CMD ["/bin/bash"]
# Tue, 02 Aug 2022 02:03:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 02:03:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 02:04:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 02:05:16 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b95ba076a26b98e98eac4b43596b59c20d1e61a36bcaf2afae3aeebadc8844cf`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 40.3 MB (40312250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c9df55506368eeeb59c5f56bf5d6f9ef4476a6b1e43154eebe32e436e60d7a`  
		Last Modified: Tue, 02 Aug 2022 01:44:42 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60aa30d82c4849b80da22554e0006d9c23c68a807fcb795b2f35ac6c02549eca`  
		Last Modified: Tue, 02 Aug 2022 01:44:42 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61b5d5a768deb5e021d74947bacf44422a006a3495d70395a7d745e07fab3f3`  
		Last Modified: Tue, 02 Aug 2022 01:44:42 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5302476a417ee0052e99816026f14bd6111e868aff0afed105038f5bf2c6ef`  
		Last Modified: Tue, 02 Aug 2022 02:19:12 GMT  
		Size: 6.6 MB (6631595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6ffa599dded0e2d5396a2e5b5cf1c7bef210b53ab5bc8863068549c1ce6bdd`  
		Last Modified: Tue, 02 Aug 2022 02:19:35 GMT  
		Size: 38.2 MB (38162222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c764bf569c904be4755c19d16f88022c4cf1f489d57580e028ade4294cca72`  
		Last Modified: Tue, 02 Aug 2022 02:20:14 GMT  
		Size: 117.3 MB (117290043 bytes)  
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
$ docker pull buildpack-deps@sha256:1e1e74caf2e0e8989c33f3170baddfc3ae848e6b26269fb543dc00053f8c6ec4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.5 MB (236450829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aeeafa7909c0b22a7bbacfb11c178ef12c0ca3d20420f976fa215dd87ccbf58f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:39:28 GMT
ADD file:a4ae521feddf8357667e9361bdd972a69ed945f3857cc8c534652592e432575d in / 
# Tue, 05 Apr 2022 22:39:29 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Apr 2022 22:39:30 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 22:39:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Apr 2022 22:39:32 GMT
CMD ["/bin/bash"]
# Tue, 05 Apr 2022 23:06:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:06:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 05 Apr 2022 23:07:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:09:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1335d7ebdbbb7325d434cf945bcb54cb20f7288e1ca2a1cf140ae02b324646e6`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 45.8 MB (45816182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa6a227af79fa98ebbd1d2da516e2b7ce1cea5519a760cd0f6688738fbdb951`  
		Last Modified: Tue, 05 Apr 2022 22:40:40 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3928723c2c34ecd7264ce4e195ddda11403213b1c93d02e8efcd11de4b07a1`  
		Last Modified: Tue, 05 Apr 2022 22:40:40 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e468001dd2f338d54f47d062d65db61c754f09897744d97084afa15cee021200`  
		Last Modified: Tue, 05 Apr 2022 22:40:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abf8b8634fb64c0b6634daaf98b0d89d01420d22a01f63010623587194cfc7c`  
		Last Modified: Tue, 05 Apr 2022 23:13:08 GMT  
		Size: 7.9 MB (7932551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6d144d968e58673ed441d100257197c971e98922fc325d2b9d2726c37b1669`  
		Last Modified: Tue, 05 Apr 2022 23:13:29 GMT  
		Size: 42.9 MB (42898142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86384a05f478f2b7db7a8e5697851efe9ced94315317560ef2f7b936575f407b`  
		Last Modified: Tue, 05 Apr 2022 23:13:57 GMT  
		Size: 139.8 MB (139802417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:xenial` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:bdf5504d8fad9d8f2637b7afa429d9008f8290629078eec62b30b79581cbab25
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.5 MB (245528509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b86fb1b9cf83165573abf6e47221fa430546b66ca9c4e2a7fbb9014405d52f66`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:32:03 GMT
ADD file:c84969ed4d4e336ec5996e26e35261f683b36f1af7a978df587296ef5e7a2627 in / 
# Tue, 02 Aug 2022 01:32:06 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 02 Aug 2022 01:32:07 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:32:08 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 02 Aug 2022 01:32:08 GMT
CMD ["/bin/bash"]
# Tue, 02 Aug 2022 03:04:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 03:05:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 03:06:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 03:09:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5057452c10cfe2216f39949f909f3cd83002d256d1bbd564ae242352a5460fe2`  
		Last Modified: Sun, 08 Aug 2021 01:00:30 GMT  
		Size: 47.5 MB (47522137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72bced789eccb5759f541a5b15b9a3031c06cc54bdbff1a553cc0ef29ddad2bc`  
		Last Modified: Tue, 02 Aug 2022 01:36:22 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11a61259761ffe18601a628413443ccb5dee06a185a81c902220dfc070801c3`  
		Last Modified: Tue, 02 Aug 2022 01:35:56 GMT  
		Size: 483.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3272460dff18ff8fd96d33337b0ff5cc5d9d2e7f158c662273e1bb760c7f9722`  
		Last Modified: Tue, 02 Aug 2022 01:36:06 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65fd76771481bd61ed3539bc027b95c72e82ceebe357d2d960463332e3348c73`  
		Last Modified: Tue, 02 Aug 2022 03:26:11 GMT  
		Size: 7.7 MB (7693686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6157fa0cdd9af85bd373614103144ea737420e95c79b68ad61350c0104479e7`  
		Last Modified: Tue, 02 Aug 2022 03:26:35 GMT  
		Size: 45.1 MB (45147297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c247b2dc61cdf98e47d6c87cb26414dacc0cbef9f98b918e0900bbbb02d1d34f`  
		Last Modified: Tue, 02 Aug 2022 03:27:21 GMT  
		Size: 145.2 MB (145163883 bytes)  
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
$ docker pull buildpack-deps@sha256:487da0d43010692cb89ce7866ea622e8c2b8a4e6f2b7f5c6fdbf13d68b270890
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
$ docker pull buildpack-deps@sha256:b8906d491e9ea82d98e9a32a481e5ac8dd954ebd450ef51b66dd81d58e2c7758
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46945381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3ccbb2329fe1cdc286597d9fe720ae166a6ae78a42d285f218bdc868a849009`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:41:46 GMT
ADD file:294a94a081de785c730003a440a0530a85add2bcb60c0f5bc4ce7ee17867ac4e in / 
# Tue, 02 Aug 2022 01:41:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 02 Aug 2022 01:41:48 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:41:49 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 02 Aug 2022 01:41:49 GMT
CMD ["/bin/bash"]
# Tue, 02 Aug 2022 02:03:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 02:03:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b95ba076a26b98e98eac4b43596b59c20d1e61a36bcaf2afae3aeebadc8844cf`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 40.3 MB (40312250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c9df55506368eeeb59c5f56bf5d6f9ef4476a6b1e43154eebe32e436e60d7a`  
		Last Modified: Tue, 02 Aug 2022 01:44:42 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60aa30d82c4849b80da22554e0006d9c23c68a807fcb795b2f35ac6c02549eca`  
		Last Modified: Tue, 02 Aug 2022 01:44:42 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61b5d5a768deb5e021d74947bacf44422a006a3495d70395a7d745e07fab3f3`  
		Last Modified: Tue, 02 Aug 2022 01:44:42 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5302476a417ee0052e99816026f14bd6111e868aff0afed105038f5bf2c6ef`  
		Last Modified: Tue, 02 Aug 2022 02:19:12 GMT  
		Size: 6.6 MB (6631595 bytes)  
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
$ docker pull buildpack-deps@sha256:e2aa06904b7f5534f1de9f786e7d2bd4a9b18bc0965bac97a554ae93995a7081
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.8 MB (53750270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaaa97755201d055ca11812e12f2141e4fb1f55691aa21b2670756b6c564781c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:39:28 GMT
ADD file:a4ae521feddf8357667e9361bdd972a69ed945f3857cc8c534652592e432575d in / 
# Tue, 05 Apr 2022 22:39:29 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Apr 2022 22:39:30 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 22:39:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Apr 2022 22:39:32 GMT
CMD ["/bin/bash"]
# Tue, 05 Apr 2022 23:06:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:06:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1335d7ebdbbb7325d434cf945bcb54cb20f7288e1ca2a1cf140ae02b324646e6`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 45.8 MB (45816182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa6a227af79fa98ebbd1d2da516e2b7ce1cea5519a760cd0f6688738fbdb951`  
		Last Modified: Tue, 05 Apr 2022 22:40:40 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3928723c2c34ecd7264ce4e195ddda11403213b1c93d02e8efcd11de4b07a1`  
		Last Modified: Tue, 05 Apr 2022 22:40:40 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e468001dd2f338d54f47d062d65db61c754f09897744d97084afa15cee021200`  
		Last Modified: Tue, 05 Apr 2022 22:40:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abf8b8634fb64c0b6634daaf98b0d89d01420d22a01f63010623587194cfc7c`  
		Last Modified: Tue, 05 Apr 2022 23:13:08 GMT  
		Size: 7.9 MB (7932551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:xenial-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:78a48a34b1b38f960afab1bd4f452bfdf661eed3c719f377a8ea9afb7e96108f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.2 MB (55217329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbbd4191e342ab25bd0eea23323187f991a7f54697f813d022fbddaa02078c96`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:32:03 GMT
ADD file:c84969ed4d4e336ec5996e26e35261f683b36f1af7a978df587296ef5e7a2627 in / 
# Tue, 02 Aug 2022 01:32:06 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 02 Aug 2022 01:32:07 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:32:08 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 02 Aug 2022 01:32:08 GMT
CMD ["/bin/bash"]
# Tue, 02 Aug 2022 03:04:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 03:05:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5057452c10cfe2216f39949f909f3cd83002d256d1bbd564ae242352a5460fe2`  
		Last Modified: Sun, 08 Aug 2021 01:00:30 GMT  
		Size: 47.5 MB (47522137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72bced789eccb5759f541a5b15b9a3031c06cc54bdbff1a553cc0ef29ddad2bc`  
		Last Modified: Tue, 02 Aug 2022 01:36:22 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11a61259761ffe18601a628413443ccb5dee06a185a81c902220dfc070801c3`  
		Last Modified: Tue, 02 Aug 2022 01:35:56 GMT  
		Size: 483.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3272460dff18ff8fd96d33337b0ff5cc5d9d2e7f158c662273e1bb760c7f9722`  
		Last Modified: Tue, 02 Aug 2022 01:36:06 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65fd76771481bd61ed3539bc027b95c72e82ceebe357d2d960463332e3348c73`  
		Last Modified: Tue, 02 Aug 2022 03:26:11 GMT  
		Size: 7.7 MB (7693686 bytes)  
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
$ docker pull buildpack-deps@sha256:c65c40098f64bb19e2428d8d8bfa9a43fe88883acd39102ab9a88b43a421b67e
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
$ docker pull buildpack-deps@sha256:2e7f9d96fec289bb930857a48be7081ba0eb7cb06ac2b78e7f04b88f11e1ce75
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.1 MB (85107603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e970a2a3afffcff7f5e7d40b9772810da49015165b970887e44198ce39742ebd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:41:46 GMT
ADD file:294a94a081de785c730003a440a0530a85add2bcb60c0f5bc4ce7ee17867ac4e in / 
# Tue, 02 Aug 2022 01:41:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 02 Aug 2022 01:41:48 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:41:49 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 02 Aug 2022 01:41:49 GMT
CMD ["/bin/bash"]
# Tue, 02 Aug 2022 02:03:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 02:03:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 02:04:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b95ba076a26b98e98eac4b43596b59c20d1e61a36bcaf2afae3aeebadc8844cf`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 40.3 MB (40312250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c9df55506368eeeb59c5f56bf5d6f9ef4476a6b1e43154eebe32e436e60d7a`  
		Last Modified: Tue, 02 Aug 2022 01:44:42 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60aa30d82c4849b80da22554e0006d9c23c68a807fcb795b2f35ac6c02549eca`  
		Last Modified: Tue, 02 Aug 2022 01:44:42 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61b5d5a768deb5e021d74947bacf44422a006a3495d70395a7d745e07fab3f3`  
		Last Modified: Tue, 02 Aug 2022 01:44:42 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5302476a417ee0052e99816026f14bd6111e868aff0afed105038f5bf2c6ef`  
		Last Modified: Tue, 02 Aug 2022 02:19:12 GMT  
		Size: 6.6 MB (6631595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6ffa599dded0e2d5396a2e5b5cf1c7bef210b53ab5bc8863068549c1ce6bdd`  
		Last Modified: Tue, 02 Aug 2022 02:19:35 GMT  
		Size: 38.2 MB (38162222 bytes)  
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
$ docker pull buildpack-deps@sha256:69d52d4e7c9933b441c84db18e6de0103a2137a9117d289ad5358e21ffbce4b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.6 MB (96648412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7df7e0761688a883d92971b15cde9c5bf0036a95ca1ab2e035171fd5867c14b2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:39:28 GMT
ADD file:a4ae521feddf8357667e9361bdd972a69ed945f3857cc8c534652592e432575d in / 
# Tue, 05 Apr 2022 22:39:29 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Apr 2022 22:39:30 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 22:39:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Apr 2022 22:39:32 GMT
CMD ["/bin/bash"]
# Tue, 05 Apr 2022 23:06:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:06:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 05 Apr 2022 23:07:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1335d7ebdbbb7325d434cf945bcb54cb20f7288e1ca2a1cf140ae02b324646e6`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 45.8 MB (45816182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa6a227af79fa98ebbd1d2da516e2b7ce1cea5519a760cd0f6688738fbdb951`  
		Last Modified: Tue, 05 Apr 2022 22:40:40 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3928723c2c34ecd7264ce4e195ddda11403213b1c93d02e8efcd11de4b07a1`  
		Last Modified: Tue, 05 Apr 2022 22:40:40 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e468001dd2f338d54f47d062d65db61c754f09897744d97084afa15cee021200`  
		Last Modified: Tue, 05 Apr 2022 22:40:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abf8b8634fb64c0b6634daaf98b0d89d01420d22a01f63010623587194cfc7c`  
		Last Modified: Tue, 05 Apr 2022 23:13:08 GMT  
		Size: 7.9 MB (7932551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6d144d968e58673ed441d100257197c971e98922fc325d2b9d2726c37b1669`  
		Last Modified: Tue, 05 Apr 2022 23:13:29 GMT  
		Size: 42.9 MB (42898142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:xenial-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:ec195c6680999f436dcaac43ecb2f433c12e294279f4457108cc09461edf2636
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.4 MB (100364626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54097dd529c992a5b4db8428a52ab66f609f66f1a118b2626a87128df3c5a414`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:32:03 GMT
ADD file:c84969ed4d4e336ec5996e26e35261f683b36f1af7a978df587296ef5e7a2627 in / 
# Tue, 02 Aug 2022 01:32:06 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 02 Aug 2022 01:32:07 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:32:08 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 02 Aug 2022 01:32:08 GMT
CMD ["/bin/bash"]
# Tue, 02 Aug 2022 03:04:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 03:05:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 03:06:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5057452c10cfe2216f39949f909f3cd83002d256d1bbd564ae242352a5460fe2`  
		Last Modified: Sun, 08 Aug 2021 01:00:30 GMT  
		Size: 47.5 MB (47522137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72bced789eccb5759f541a5b15b9a3031c06cc54bdbff1a553cc0ef29ddad2bc`  
		Last Modified: Tue, 02 Aug 2022 01:36:22 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11a61259761ffe18601a628413443ccb5dee06a185a81c902220dfc070801c3`  
		Last Modified: Tue, 02 Aug 2022 01:35:56 GMT  
		Size: 483.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3272460dff18ff8fd96d33337b0ff5cc5d9d2e7f158c662273e1bb760c7f9722`  
		Last Modified: Tue, 02 Aug 2022 01:36:06 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65fd76771481bd61ed3539bc027b95c72e82ceebe357d2d960463332e3348c73`  
		Last Modified: Tue, 02 Aug 2022 03:26:11 GMT  
		Size: 7.7 MB (7693686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6157fa0cdd9af85bd373614103144ea737420e95c79b68ad61350c0104479e7`  
		Last Modified: Tue, 02 Aug 2022 03:26:35 GMT  
		Size: 45.1 MB (45147297 bytes)  
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
