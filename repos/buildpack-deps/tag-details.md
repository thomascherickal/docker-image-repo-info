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
$ docker pull buildpack-deps@sha256:9f3239283e1eb80449f823d8e18a8a94b2e766adaa92a29b9f2f48b964674dd5
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
$ docker pull buildpack-deps@sha256:a76fa2851a818bd9e17282587a14ab6a70f87bc50ad71aa4194dd68193d0c5e3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.1 MB (210145871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:150729efc1f801b3c41dad5c9402bedd2cc631f5f40eae14367bd776664701b4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:55:17 GMT
ADD file:3c6dc937cb7b4c81b42126f377d23320ec1d0a8ca34d38e7c45871f1d08dac43 in / 
# Tue, 25 Oct 2022 05:55:18 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 25 Oct 2022 05:55:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:55:19 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 25 Oct 2022 05:55:19 GMT
CMD ["/bin/bash"]
# Tue, 25 Oct 2022 08:24:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:24:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:24:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:28:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:828b35a09f0b2f3d1dead43aa2468ff5eba6c463423b3fff7ee6d150f6fd1b6b`  
		Last Modified: Thu, 05 Aug 2021 00:25:09 GMT  
		Size: 41.2 MB (41239253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66927c6d1d3d2e9321c4893f7f2105b7cd23dfb082853d97ec08f188e271e612`  
		Last Modified: Tue, 25 Oct 2022 05:57:02 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000560be91651dcbf476ebacb8bf1f1339694a3327f8e6da2519e0b29b33eb5d`  
		Last Modified: Tue, 25 Oct 2022 05:57:02 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6225a0253717abdc2ee23ea211c1c439c93b84231ec0a4f1c74762a205ba7234`  
		Last Modified: Tue, 25 Oct 2022 05:57:02 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e6d65f936039d0e2af7dd447344ff1a4f3d1987e1cf2628011285c9492be94`  
		Last Modified: Tue, 25 Oct 2022 08:36:56 GMT  
		Size: 6.8 MB (6838703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5c22d5e41e5c25f365fc9199c3648c8fe1b7819614ce763b3dbc00fa6e0242`  
		Last Modified: Tue, 25 Oct 2022 08:37:11 GMT  
		Size: 39.8 MB (39808282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0bcb2fc5c488536f3c7fb6acf7cfdf7815783a88e34de08f2e3ab3b05a7a9a`  
		Last Modified: Tue, 25 Oct 2022 08:37:34 GMT  
		Size: 122.3 MB (122258127 bytes)  
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
$ docker pull buildpack-deps@sha256:1f96d9808e87659130e067e8dd0f04514541dcf5ba5f26c01f361595bec5eb39
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
$ docker pull buildpack-deps@sha256:9729b711e909d53c0dcac87e152741034c35987034110ec2df03fef0c182419c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48079462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:950208a6f6157f0c26f5634bd58c369a0072c83b7f568b430e84c66224f18dbe`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:55:17 GMT
ADD file:3c6dc937cb7b4c81b42126f377d23320ec1d0a8ca34d38e7c45871f1d08dac43 in / 
# Tue, 25 Oct 2022 05:55:18 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 25 Oct 2022 05:55:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:55:19 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 25 Oct 2022 05:55:19 GMT
CMD ["/bin/bash"]
# Tue, 25 Oct 2022 08:24:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:24:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:828b35a09f0b2f3d1dead43aa2468ff5eba6c463423b3fff7ee6d150f6fd1b6b`  
		Last Modified: Thu, 05 Aug 2021 00:25:09 GMT  
		Size: 41.2 MB (41239253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66927c6d1d3d2e9321c4893f7f2105b7cd23dfb082853d97ec08f188e271e612`  
		Last Modified: Tue, 25 Oct 2022 05:57:02 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000560be91651dcbf476ebacb8bf1f1339694a3327f8e6da2519e0b29b33eb5d`  
		Last Modified: Tue, 25 Oct 2022 05:57:02 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6225a0253717abdc2ee23ea211c1c439c93b84231ec0a4f1c74762a205ba7234`  
		Last Modified: Tue, 25 Oct 2022 05:57:02 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e6d65f936039d0e2af7dd447344ff1a4f3d1987e1cf2628011285c9492be94`  
		Last Modified: Tue, 25 Oct 2022 08:36:56 GMT  
		Size: 6.8 MB (6838703 bytes)  
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
$ docker pull buildpack-deps@sha256:03039fe25cc2845bf8e249b2eca46ae5937e884ddabb6548d8f1cb296f2e5b17
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
$ docker pull buildpack-deps@sha256:d02144ab71a36dd5357661276ef23395a32022382a53294d6681cfd442327547
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.9 MB (87887744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:067fd097536acda8a5a5cc26b969443e4a156dc464664ce5692a72466ca48caa`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:55:17 GMT
ADD file:3c6dc937cb7b4c81b42126f377d23320ec1d0a8ca34d38e7c45871f1d08dac43 in / 
# Tue, 25 Oct 2022 05:55:18 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 25 Oct 2022 05:55:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:55:19 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 25 Oct 2022 05:55:19 GMT
CMD ["/bin/bash"]
# Tue, 25 Oct 2022 08:24:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:24:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:24:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:828b35a09f0b2f3d1dead43aa2468ff5eba6c463423b3fff7ee6d150f6fd1b6b`  
		Last Modified: Thu, 05 Aug 2021 00:25:09 GMT  
		Size: 41.2 MB (41239253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66927c6d1d3d2e9321c4893f7f2105b7cd23dfb082853d97ec08f188e271e612`  
		Last Modified: Tue, 25 Oct 2022 05:57:02 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000560be91651dcbf476ebacb8bf1f1339694a3327f8e6da2519e0b29b33eb5d`  
		Last Modified: Tue, 25 Oct 2022 05:57:02 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6225a0253717abdc2ee23ea211c1c439c93b84231ec0a4f1c74762a205ba7234`  
		Last Modified: Tue, 25 Oct 2022 05:57:02 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e6d65f936039d0e2af7dd447344ff1a4f3d1987e1cf2628011285c9492be94`  
		Last Modified: Tue, 25 Oct 2022 08:36:56 GMT  
		Size: 6.8 MB (6838703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5c22d5e41e5c25f365fc9199c3648c8fe1b7819614ce763b3dbc00fa6e0242`  
		Last Modified: Tue, 25 Oct 2022 08:37:11 GMT  
		Size: 39.8 MB (39808282 bytes)  
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
$ docker pull buildpack-deps@sha256:9fd1bd60ef4fb6123e4e4c8874cac211e0d563dad6b188f64574e33eed1094bc
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
$ docker pull buildpack-deps@sha256:8e193981b35a706985cdc98b60c03e5542e213ee488587b2d9958940c84561d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.4 MB (221393894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2608fa2156d0a642f6ac431b67743a605276f1e936f72ecc653a3da10b792ea4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:04 GMT
ADD file:ed601c56cf74241eeb1971b24ed969fb855cd2b9330276d3c5779ecdb0b28364 in / 
# Tue, 04 Oct 2022 23:35:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:00:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:00:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:01:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:04:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e706e0a9f42365312b366bf4caa22f3cdd8fc7fd8f6f49b4dd3782711f66aca7`  
		Last Modified: Tue, 04 Oct 2022 11:37:26 GMT  
		Size: 26.7 MB (26711852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14bb308d0caa16e5231c4d889948a8b0c06b9e2c461919c74887b27e349d490`  
		Last Modified: Wed, 05 Oct 2022 01:22:33 GMT  
		Size: 6.6 MB (6631019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd853d7120feb9f81650bf7bc95fac3a301e6f7fb667e27ff0c44f05fc3bd84`  
		Last Modified: Wed, 05 Oct 2022 01:22:33 GMT  
		Size: 3.0 MB (3023747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e261a80722021da4732449560d09c9be0f3a45bc7cd83a11ec75216c88d19d8`  
		Last Modified: Wed, 05 Oct 2022 01:22:50 GMT  
		Size: 45.5 MB (45498303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f4264228ed8e7647983ec917c22f259b84a520ddaee10cd3d968f9c68bff1ac`  
		Last Modified: Wed, 05 Oct 2022 01:23:19 GMT  
		Size: 139.5 MB (139528973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:8c42ce93b617d12c423261ac5d8a9b5949385d3ee604c85ab12add1f2354b260
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.6 MB (189554619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fd4e33dc0507b376b73e9f97cafb185f57745359d69c95771a51290fe3c978a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:31 GMT
ADD file:20e0d71059d38b1e18636b9db71f534d7297c3f571d73d45a75b4b8d3cac86c7 in / 
# Wed, 05 Oct 2022 00:13:32 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:40:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:40:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:41:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:42:24 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:91bb9a9844d67fd31f07ebd74dc8a4f4f18e2f959d3aa2166aca86ae57f353c6`  
		Last Modified: Wed, 05 Oct 2022 00:15:26 GMT  
		Size: 22.3 MB (22305721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5da5c18a3ec9c91b23737d7223b602b070f7de605771c25aadd8092545e561`  
		Last Modified: Wed, 05 Oct 2022 00:57:59 GMT  
		Size: 5.7 MB (5697196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327d003e6583d861f4c3df07410a51c18c3b7f4a0649fbfde6aab1ec77b4b110`  
		Last Modified: Wed, 05 Oct 2022 00:57:58 GMT  
		Size: 2.6 MB (2585088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdc6a2f528031e62d90580aa8ccad6d2351f1de9a49f1ebeed4945a07ffeed3`  
		Last Modified: Wed, 05 Oct 2022 00:58:23 GMT  
		Size: 40.7 MB (40690856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dbc06c808278c578a9ebcf12b02c2e632f8eb0c39fa50538a9faf7483bd4953`  
		Last Modified: Wed, 05 Oct 2022 00:59:02 GMT  
		Size: 118.3 MB (118275758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3e79fc3dd3b14b9bb575350832102635634b50d09fc0e17787f8ab9461363820
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.0 MB (205988599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:307ed33f4f8918cc97443f064b1a80b4169652a8a5830856adc59899d807e672`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:56 GMT
ADD file:585011162da73734395f2ef251ad89b72cfed0101c7da2435fac55061f99b516 in / 
# Tue, 25 Oct 2022 05:54:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:03:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:04:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:04:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:08:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a217cb16e35b382d60a7ab454a8c4db0fbe5e0aeec4b4c346e51eb1e77d34f8c`  
		Last Modified: Tue, 25 Oct 2022 05:55:45 GMT  
		Size: 23.7 MB (23735856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296237f400b08de0ee2566d1d70f0c0fa8e7334ec80823903e2aaf4904c5a49d`  
		Last Modified: Tue, 25 Oct 2022 08:33:20 GMT  
		Size: 6.1 MB (6074795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82de00773434d5186afe917dba4d4a8e731ffb220b4b8b348628c4df9f9e773e`  
		Last Modified: Tue, 25 Oct 2022 08:33:20 GMT  
		Size: 2.8 MB (2790789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ead073af2bd060ee0645628a8ca9a37e4f01b5c89e089690cff894da4eb30b`  
		Last Modified: Tue, 25 Oct 2022 08:33:34 GMT  
		Size: 43.3 MB (43296375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ac6f110046b149cfabf2ddff78dd4a130eeac7523196ddbe458ecf807d0656`  
		Last Modified: Tue, 25 Oct 2022 08:34:01 GMT  
		Size: 130.1 MB (130090784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04` - linux; 386

```console
$ docker pull buildpack-deps@sha256:88842772446e48882fcdf20872ab09cd43f8fcb75681fa5f61b926dc8644445f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.2 MB (218240056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0daef8c85d992fa89d4cc85af6ebe982b049919dd5c9fd4465b81a65a9cd2bd9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:34:56 GMT
ADD file:40406c12653f21504e334fcfb19c00ee9eed94dbaa2eb7c7bfdb293677697aa6 in / 
# Tue, 25 Oct 2022 02:34:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:20:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:21:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 05:21:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:24:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1beb66ce54f29e44b5005bf3e2d004424176aa3361ee8e602a9ae10a8ee447cf`  
		Last Modified: Tue, 25 Oct 2022 02:35:33 GMT  
		Size: 27.2 MB (27166059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196f1fa30db3bbf53093b5c7d1d2add129bf1974ce53a6e094f0f0795c7881e7`  
		Last Modified: Tue, 25 Oct 2022 05:31:10 GMT  
		Size: 6.9 MB (6921884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f025677e2376712e8fb9824f1fcfefa2d3005ebe8cebe43324e65b6d2f3a106`  
		Last Modified: Tue, 25 Oct 2022 05:31:09 GMT  
		Size: 3.0 MB (3042023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5439394181cf9e8ac2e0b446f62199582c04aa5f5903de80e9b8474a01ca5c24`  
		Last Modified: Tue, 25 Oct 2022 05:31:28 GMT  
		Size: 47.1 MB (47083490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb1497899c9f48cc0c773769e863fb5f587546a5831104b7ee048453a776aebe`  
		Last Modified: Tue, 25 Oct 2022 05:31:56 GMT  
		Size: 134.0 MB (134026600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:443a00cd3f35125ff2856e16c19720e7963f64acd7ca5955fed24d8763ebaffa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.4 MB (246426888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70f27d2f9478275b6a5a2a4b9587a5ceea77a4af2af4a05be63e9ee1adb3ce8d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:34 GMT
ADD file:254e11be9bc865d645aba7c16a39a04f5ce227b7aa4280f7a42baec47b0c6ee0 in / 
# Tue, 25 Oct 2022 03:25:36 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:20:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:21:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:22:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:27:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:21b8f46bc1957ff60412d81678134500cf7a4f0e7f198ba384fedb2e5747d847`  
		Last Modified: Tue, 25 Oct 2022 03:27:21 GMT  
		Size: 30.4 MB (30443225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7a73c0177bc0907d9770e0863fb7f6949a870d385b401421a0817a32cd56be`  
		Last Modified: Tue, 25 Oct 2022 06:52:33 GMT  
		Size: 7.1 MB (7051025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f82d4b01549cae8ea6c3b7e9f210d370b148dd8004af19925715e43994e9ff`  
		Last Modified: Tue, 25 Oct 2022 06:52:32 GMT  
		Size: 3.7 MB (3740646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc5edd6bb0a218e937aacff2efa004bac7b35909a1d19740f14acbae1df7b87`  
		Last Modified: Tue, 25 Oct 2022 06:52:59 GMT  
		Size: 53.7 MB (53741147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600501f491d899f441f91702b04e48dda009fb613806254ab578645e5cc0307f`  
		Last Modified: Tue, 25 Oct 2022 06:53:48 GMT  
		Size: 151.5 MB (151450845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:16eceed169fc7d8e7dd3f213936244ab45f5e6ec0e5090ecd3f9a8f04e0f9e4c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.8 MB (205759274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ab91687893f8d5e47036caf530ff156ea86a4d93a7b61bf9ad5037e833453cf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:02 GMT
ADD file:0843e89b8865a30626cece7a42cf27708a86422aadb28029168b2f159a8768fa in / 
# Tue, 25 Oct 2022 01:23:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:34:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:34:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 02:35:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:37:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4cd692a206d359f66e10c4f4f2a37009c4162f022df78a9bb8e8c24def290167`  
		Last Modified: Tue, 25 Oct 2022 01:24:23 GMT  
		Size: 25.4 MB (25371461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1872edbfc35ad376faca8b8da8bfdde0ac95f27652b1188c2036672466ab8233`  
		Last Modified: Tue, 25 Oct 2022 02:51:21 GMT  
		Size: 6.3 MB (6326364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5dda90dab707bb33111b66abdc094ed182c70b7a83b6844b6b316ba93a0f779`  
		Last Modified: Tue, 25 Oct 2022 02:51:21 GMT  
		Size: 3.0 MB (2976628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feacbe49c2940d688c7c8200c29c610e8a5a65180c8b6d67c78b193f408418a7`  
		Last Modified: Tue, 25 Oct 2022 02:51:34 GMT  
		Size: 45.0 MB (45044933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74da665a3988b61dbc1e55c52dc97c4d3fcf3b2c58feb3f9664d6b471d420d91`  
		Last Modified: Tue, 25 Oct 2022 02:51:56 GMT  
		Size: 126.0 MB (126039888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:18.04-curl`

```console
$ docker pull buildpack-deps@sha256:437c0a65f1a0597bc2aea93d7ed8c38b6209d7768299cb9af858a074be32277e
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
$ docker pull buildpack-deps@sha256:c4539563e222d7175a071977335bfbb5a52887b403295e6bede505e11a183e63
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36366618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b86072004a7e51f50a4f9308592351b5df03fbcf3569269d2aded7b6d06f5141`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:04 GMT
ADD file:ed601c56cf74241eeb1971b24ed969fb855cd2b9330276d3c5779ecdb0b28364 in / 
# Tue, 04 Oct 2022 23:35:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:00:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:00:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e706e0a9f42365312b366bf4caa22f3cdd8fc7fd8f6f49b4dd3782711f66aca7`  
		Last Modified: Tue, 04 Oct 2022 11:37:26 GMT  
		Size: 26.7 MB (26711852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14bb308d0caa16e5231c4d889948a8b0c06b9e2c461919c74887b27e349d490`  
		Last Modified: Wed, 05 Oct 2022 01:22:33 GMT  
		Size: 6.6 MB (6631019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd853d7120feb9f81650bf7bc95fac3a301e6f7fb667e27ff0c44f05fc3bd84`  
		Last Modified: Wed, 05 Oct 2022 01:22:33 GMT  
		Size: 3.0 MB (3023747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:64eb7b3da5d316eb2ccb73ac59d267a9e931c6a22c3ccfb92ca219eac156b3e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30588005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faa01cb702a2d7c8668373897fe036b5e3a9734a7731883f831ee6232ef49e5d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:31 GMT
ADD file:20e0d71059d38b1e18636b9db71f534d7297c3f571d73d45a75b4b8d3cac86c7 in / 
# Wed, 05 Oct 2022 00:13:32 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:40:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:40:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:91bb9a9844d67fd31f07ebd74dc8a4f4f18e2f959d3aa2166aca86ae57f353c6`  
		Last Modified: Wed, 05 Oct 2022 00:15:26 GMT  
		Size: 22.3 MB (22305721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5da5c18a3ec9c91b23737d7223b602b070f7de605771c25aadd8092545e561`  
		Last Modified: Wed, 05 Oct 2022 00:57:59 GMT  
		Size: 5.7 MB (5697196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327d003e6583d861f4c3df07410a51c18c3b7f4a0649fbfde6aab1ec77b4b110`  
		Last Modified: Wed, 05 Oct 2022 00:57:58 GMT  
		Size: 2.6 MB (2585088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:4a7fb4ce2c117e99998cdeef7a19e67cc71055fe3a3e73e8aa9c33ffb9c67d3b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.6 MB (32601440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ed643d0aed22b28551913f89b4c72639e5b8faaae70ba0f4501439d38584433`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:56 GMT
ADD file:585011162da73734395f2ef251ad89b72cfed0101c7da2435fac55061f99b516 in / 
# Tue, 25 Oct 2022 05:54:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:03:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:04:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a217cb16e35b382d60a7ab454a8c4db0fbe5e0aeec4b4c346e51eb1e77d34f8c`  
		Last Modified: Tue, 25 Oct 2022 05:55:45 GMT  
		Size: 23.7 MB (23735856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296237f400b08de0ee2566d1d70f0c0fa8e7334ec80823903e2aaf4904c5a49d`  
		Last Modified: Tue, 25 Oct 2022 08:33:20 GMT  
		Size: 6.1 MB (6074795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82de00773434d5186afe917dba4d4a8e731ffb220b4b8b348628c4df9f9e773e`  
		Last Modified: Tue, 25 Oct 2022 08:33:20 GMT  
		Size: 2.8 MB (2790789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:f9d7810c1b79a2b1c2979e85b4ec6d5fcc001703c2e12449627f1aad25218640
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37129966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dda5cb77527fbe9d18b28b41ea7c3b6c7ae3fd43336a9b9cbf26b6f9e7194841`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:34:56 GMT
ADD file:40406c12653f21504e334fcfb19c00ee9eed94dbaa2eb7c7bfdb293677697aa6 in / 
# Tue, 25 Oct 2022 02:34:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:20:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:21:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1beb66ce54f29e44b5005bf3e2d004424176aa3361ee8e602a9ae10a8ee447cf`  
		Last Modified: Tue, 25 Oct 2022 02:35:33 GMT  
		Size: 27.2 MB (27166059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196f1fa30db3bbf53093b5c7d1d2add129bf1974ce53a6e094f0f0795c7881e7`  
		Last Modified: Tue, 25 Oct 2022 05:31:10 GMT  
		Size: 6.9 MB (6921884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f025677e2376712e8fb9824f1fcfefa2d3005ebe8cebe43324e65b6d2f3a106`  
		Last Modified: Tue, 25 Oct 2022 05:31:09 GMT  
		Size: 3.0 MB (3042023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:45c832bf6c3088da7c40d8e5205cdf1f8357326d9ad8840ddc61343237447345
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41234896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a774524b743b63f11381672077399dd0cdf35bb59695140dc3f5f7e3b3f523b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:34 GMT
ADD file:254e11be9bc865d645aba7c16a39a04f5ce227b7aa4280f7a42baec47b0c6ee0 in / 
# Tue, 25 Oct 2022 03:25:36 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:20:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:21:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:21b8f46bc1957ff60412d81678134500cf7a4f0e7f198ba384fedb2e5747d847`  
		Last Modified: Tue, 25 Oct 2022 03:27:21 GMT  
		Size: 30.4 MB (30443225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7a73c0177bc0907d9770e0863fb7f6949a870d385b401421a0817a32cd56be`  
		Last Modified: Tue, 25 Oct 2022 06:52:33 GMT  
		Size: 7.1 MB (7051025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f82d4b01549cae8ea6c3b7e9f210d370b148dd8004af19925715e43994e9ff`  
		Last Modified: Tue, 25 Oct 2022 06:52:32 GMT  
		Size: 3.7 MB (3740646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:171c50890d275551e068fbc231b063d10c68d4f76bb5c113b55893fd0c094898
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34674453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23932295597dc4628240979d04d45ef0bac7ff6e5a0e864ddec4d112b2aa2143`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:02 GMT
ADD file:0843e89b8865a30626cece7a42cf27708a86422aadb28029168b2f159a8768fa in / 
# Tue, 25 Oct 2022 01:23:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:34:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:34:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4cd692a206d359f66e10c4f4f2a37009c4162f022df78a9bb8e8c24def290167`  
		Last Modified: Tue, 25 Oct 2022 01:24:23 GMT  
		Size: 25.4 MB (25371461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1872edbfc35ad376faca8b8da8bfdde0ac95f27652b1188c2036672466ab8233`  
		Last Modified: Tue, 25 Oct 2022 02:51:21 GMT  
		Size: 6.3 MB (6326364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5dda90dab707bb33111b66abdc094ed182c70b7a83b6844b6b316ba93a0f779`  
		Last Modified: Tue, 25 Oct 2022 02:51:21 GMT  
		Size: 3.0 MB (2976628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:18.04-scm`

```console
$ docker pull buildpack-deps@sha256:2cd1279307ba80edb1d4d0d882abbb11aab1d95d217ad147971be1e53f48d7df
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
$ docker pull buildpack-deps@sha256:2185d9b019c2c7ffa24811155449345078f4adb96a6b771140d25fa96128e80d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81864921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e18c1737a8adb0820fe73beb358791cbde70dc5a532a61b2fa74b072d928cca6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:04 GMT
ADD file:ed601c56cf74241eeb1971b24ed969fb855cd2b9330276d3c5779ecdb0b28364 in / 
# Tue, 04 Oct 2022 23:35:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:00:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:00:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:01:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e706e0a9f42365312b366bf4caa22f3cdd8fc7fd8f6f49b4dd3782711f66aca7`  
		Last Modified: Tue, 04 Oct 2022 11:37:26 GMT  
		Size: 26.7 MB (26711852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14bb308d0caa16e5231c4d889948a8b0c06b9e2c461919c74887b27e349d490`  
		Last Modified: Wed, 05 Oct 2022 01:22:33 GMT  
		Size: 6.6 MB (6631019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd853d7120feb9f81650bf7bc95fac3a301e6f7fb667e27ff0c44f05fc3bd84`  
		Last Modified: Wed, 05 Oct 2022 01:22:33 GMT  
		Size: 3.0 MB (3023747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e261a80722021da4732449560d09c9be0f3a45bc7cd83a11ec75216c88d19d8`  
		Last Modified: Wed, 05 Oct 2022 01:22:50 GMT  
		Size: 45.5 MB (45498303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:c135384e7b3dd71613cf28fbeb9805b51ae11140898b2d9034275ce1c7c77988
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71278861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d25e3b88b9f8e85d32a18eda77ceaf66170755d464f812b3b79a2aeb16210730`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:31 GMT
ADD file:20e0d71059d38b1e18636b9db71f534d7297c3f571d73d45a75b4b8d3cac86c7 in / 
# Wed, 05 Oct 2022 00:13:32 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:40:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:40:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:41:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:91bb9a9844d67fd31f07ebd74dc8a4f4f18e2f959d3aa2166aca86ae57f353c6`  
		Last Modified: Wed, 05 Oct 2022 00:15:26 GMT  
		Size: 22.3 MB (22305721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5da5c18a3ec9c91b23737d7223b602b070f7de605771c25aadd8092545e561`  
		Last Modified: Wed, 05 Oct 2022 00:57:59 GMT  
		Size: 5.7 MB (5697196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327d003e6583d861f4c3df07410a51c18c3b7f4a0649fbfde6aab1ec77b4b110`  
		Last Modified: Wed, 05 Oct 2022 00:57:58 GMT  
		Size: 2.6 MB (2585088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdc6a2f528031e62d90580aa8ccad6d2351f1de9a49f1ebeed4945a07ffeed3`  
		Last Modified: Wed, 05 Oct 2022 00:58:23 GMT  
		Size: 40.7 MB (40690856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:831b524d20f9c5814aac27758c344b403757f5ab45060243817b13a2c40102e6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75897815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e470c3c6917737866b9756535cfe361c65e8808582d7c42f618ac621feedca3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:56 GMT
ADD file:585011162da73734395f2ef251ad89b72cfed0101c7da2435fac55061f99b516 in / 
# Tue, 25 Oct 2022 05:54:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:03:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:04:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:04:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a217cb16e35b382d60a7ab454a8c4db0fbe5e0aeec4b4c346e51eb1e77d34f8c`  
		Last Modified: Tue, 25 Oct 2022 05:55:45 GMT  
		Size: 23.7 MB (23735856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296237f400b08de0ee2566d1d70f0c0fa8e7334ec80823903e2aaf4904c5a49d`  
		Last Modified: Tue, 25 Oct 2022 08:33:20 GMT  
		Size: 6.1 MB (6074795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82de00773434d5186afe917dba4d4a8e731ffb220b4b8b348628c4df9f9e773e`  
		Last Modified: Tue, 25 Oct 2022 08:33:20 GMT  
		Size: 2.8 MB (2790789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ead073af2bd060ee0645628a8ca9a37e4f01b5c89e089690cff894da4eb30b`  
		Last Modified: Tue, 25 Oct 2022 08:33:34 GMT  
		Size: 43.3 MB (43296375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:83df231eb79f3c19636d63aa33a16412557b58c3d612af24a8992bf30c0bf2bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.2 MB (84213456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a9bbfb87a10a33a893bf414b33e9b8b13d1a1613ff530d2f7f475add897a53d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:34:56 GMT
ADD file:40406c12653f21504e334fcfb19c00ee9eed94dbaa2eb7c7bfdb293677697aa6 in / 
# Tue, 25 Oct 2022 02:34:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:20:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:21:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 05:21:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1beb66ce54f29e44b5005bf3e2d004424176aa3361ee8e602a9ae10a8ee447cf`  
		Last Modified: Tue, 25 Oct 2022 02:35:33 GMT  
		Size: 27.2 MB (27166059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196f1fa30db3bbf53093b5c7d1d2add129bf1974ce53a6e094f0f0795c7881e7`  
		Last Modified: Tue, 25 Oct 2022 05:31:10 GMT  
		Size: 6.9 MB (6921884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f025677e2376712e8fb9824f1fcfefa2d3005ebe8cebe43324e65b6d2f3a106`  
		Last Modified: Tue, 25 Oct 2022 05:31:09 GMT  
		Size: 3.0 MB (3042023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5439394181cf9e8ac2e0b446f62199582c04aa5f5903de80e9b8474a01ca5c24`  
		Last Modified: Tue, 25 Oct 2022 05:31:28 GMT  
		Size: 47.1 MB (47083490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:9b3b087f55c1efa8493ec4b43697807a5c2d17ed20ae7d7d9be3b0c0059e5780
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.0 MB (94976043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:799cb2cdce8facd27fc40f8e46c9d7af5acfdb40bc0350b08603cb8ef204716f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:34 GMT
ADD file:254e11be9bc865d645aba7c16a39a04f5ce227b7aa4280f7a42baec47b0c6ee0 in / 
# Tue, 25 Oct 2022 03:25:36 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:20:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:21:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:22:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:21b8f46bc1957ff60412d81678134500cf7a4f0e7f198ba384fedb2e5747d847`  
		Last Modified: Tue, 25 Oct 2022 03:27:21 GMT  
		Size: 30.4 MB (30443225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7a73c0177bc0907d9770e0863fb7f6949a870d385b401421a0817a32cd56be`  
		Last Modified: Tue, 25 Oct 2022 06:52:33 GMT  
		Size: 7.1 MB (7051025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f82d4b01549cae8ea6c3b7e9f210d370b148dd8004af19925715e43994e9ff`  
		Last Modified: Tue, 25 Oct 2022 06:52:32 GMT  
		Size: 3.7 MB (3740646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc5edd6bb0a218e937aacff2efa004bac7b35909a1d19740f14acbae1df7b87`  
		Last Modified: Tue, 25 Oct 2022 06:52:59 GMT  
		Size: 53.7 MB (53741147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a1f61989c50474fceff25499a47ac25dcaa6159237d67e49479a11f64bf78697
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79719386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66335b8c0d2152b8e22f15bb354ebf842a232eb17f087314607606c364ab9d5d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:02 GMT
ADD file:0843e89b8865a30626cece7a42cf27708a86422aadb28029168b2f159a8768fa in / 
# Tue, 25 Oct 2022 01:23:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:34:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:34:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 02:35:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4cd692a206d359f66e10c4f4f2a37009c4162f022df78a9bb8e8c24def290167`  
		Last Modified: Tue, 25 Oct 2022 01:24:23 GMT  
		Size: 25.4 MB (25371461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1872edbfc35ad376faca8b8da8bfdde0ac95f27652b1188c2036672466ab8233`  
		Last Modified: Tue, 25 Oct 2022 02:51:21 GMT  
		Size: 6.3 MB (6326364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5dda90dab707bb33111b66abdc094ed182c70b7a83b6844b6b316ba93a0f779`  
		Last Modified: Tue, 25 Oct 2022 02:51:21 GMT  
		Size: 3.0 MB (2976628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feacbe49c2940d688c7c8200c29c610e8a5a65180c8b6d67c78b193f408418a7`  
		Last Modified: Tue, 25 Oct 2022 02:51:34 GMT  
		Size: 45.0 MB (45044933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:20.04`

```console
$ docker pull buildpack-deps@sha256:17448e01180652e618c3052d3fe2360d3a99593b4e504591ec5e9deac35f0712
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
$ docker pull buildpack-deps@sha256:df1cb039c302258fc7aeb3d09633c18b7c2330f4df5febec069e06b01e7a631e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.8 MB (245760922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff0be4edc3bf215849f05ed174892ef853e12761ee649124bde965c0d9fa7789`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:04:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:04:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:05:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:08:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7215646fa628a9c18e31f7ea7321ae4140b44d69995ec4cdf3968cbce9a5c0b4`  
		Last Modified: Wed, 05 Oct 2022 01:23:38 GMT  
		Size: 7.7 MB (7747231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6c7ee6250b02a6cf0a3a3080d082e4ce4f858e2749921bc2623c896c487897`  
		Last Modified: Wed, 05 Oct 2022 01:23:37 GMT  
		Size: 3.6 MB (3624405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927ce100b3517cefcb05b92b71a8c91e9881466e25f273c9ce8b59ade42ef3a3`  
		Last Modified: Wed, 05 Oct 2022 01:23:58 GMT  
		Size: 60.7 MB (60738241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2912631d641854e38546e76428eb259b076e4d737fc5ef8a27d790b7f6b5d85`  
		Last Modified: Wed, 05 Oct 2022 01:24:28 GMT  
		Size: 145.1 MB (145076594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:8e9c5845425de993e8a14f762a07ba75002b29b1a385b14ce0884f9d3055d449
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.8 MB (211802501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56f88acbe9e38aa875d1ccc4954298f23f43d45f8a3d373c5f13c22f1ba9223f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:44 GMT
ADD file:75870468a948359044fa3df6c07c80badfea3dcde4823d41a19285436c40cf76 in / 
# Wed, 05 Oct 2022 00:13:44 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:42:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:42:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:43:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:44:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e679d63f382033c15f8f921851bd71fb8a85a432c0a7a612bbef16e989075145`  
		Last Modified: Wed, 05 Oct 2022 00:15:44 GMT  
		Size: 24.6 MB (24590092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8314cec2c7a441a36532dc89979b531fd7dab365416e8d4f077f16c6322a222`  
		Last Modified: Wed, 05 Oct 2022 00:59:17 GMT  
		Size: 6.7 MB (6740274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b75361ec0073f1728c7bbc9fbf5e55f5ffc978176453aaccd3f3097a710904`  
		Last Modified: Wed, 05 Oct 2022 00:59:16 GMT  
		Size: 3.1 MB (3103607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0cd29b8c09506d2393921adb0cded05dba5f57e529ff475ad92160d2b38c475`  
		Last Modified: Wed, 05 Oct 2022 00:59:45 GMT  
		Size: 55.4 MB (55441138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1062ee353a76044d7056fa8d73eb9cc0e68c08ed4df3ef21e497189a70233c3`  
		Last Modified: Wed, 05 Oct 2022 01:00:24 GMT  
		Size: 121.9 MB (121927390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:445e10a7ae38f20373cd85399fc91f13053769747294e9d0edda602105168041
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.0 MB (235997220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3e5ee77d909660495f56fcdbf233971a6f13e03d21943ea5d5a8ea754e140a3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:09:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:09:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:10:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:13:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f7d42f1359bed862a992a062b3c7cf025e6bf6625dc1ca56ae2c66d7250fba`  
		Last Modified: Tue, 25 Oct 2022 08:34:12 GMT  
		Size: 7.6 MB (7616212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc75acb9c1e02b10ddc3966608ccbac66c6fd9eeb3bff80797f9983f268a9b1a`  
		Last Modified: Tue, 25 Oct 2022 08:34:12 GMT  
		Size: 3.6 MB (3617606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d21db26b13141f20e7cce995a63f8234838277895d2d6d0e2ec4f35e659c78`  
		Last Modified: Tue, 25 Oct 2022 08:34:33 GMT  
		Size: 60.8 MB (60807384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de20e53c6129f32162fa091a310f594b29ebc675880357219b832913b9aa05b`  
		Last Modified: Tue, 25 Oct 2022 08:34:58 GMT  
		Size: 136.8 MB (136760020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:32c07eb6326ad1e49be450e350b8b21f2125e3ff69930bb973b7e82c886d2f12
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.6 MB (269600630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d09b001b9596b00fd30464d8345d01c8e29cc965f6afc931f6f78201fbac9c8c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:47 GMT
ADD file:013ddcea49540903962069a03762fe471452e8cf00bafeb530724940405797e1 in / 
# Tue, 25 Oct 2022 03:25:49 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:27:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:27:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:29:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:32:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:42e5f4d60d38e5070be91d6965be1cff1294e6dc275038002dc2ef1812233b0e`  
		Last Modified: Tue, 25 Oct 2022 03:27:44 GMT  
		Size: 33.3 MB (33300542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa48197ece6cedfce46328b98e2bd3ffa7f116e92dc0cd9aba21390a5edf11f`  
		Last Modified: Tue, 25 Oct 2022 06:54:02 GMT  
		Size: 8.7 MB (8705088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b91159ec91712ffe519d3e9624103d9ec7b58e6b1959cad0b77145851e14fc55`  
		Last Modified: Tue, 25 Oct 2022 06:54:01 GMT  
		Size: 4.5 MB (4486836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c68813dea6733b577ebd8f432367b30fab9f0639692bc2e99d633f9347aff6`  
		Last Modified: Tue, 25 Oct 2022 06:54:33 GMT  
		Size: 69.5 MB (69528310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f928b500f12d32eab804a83c4abf92c24bbba3f2da97a4be3a6502f4a8736507`  
		Last Modified: Tue, 25 Oct 2022 06:55:25 GMT  
		Size: 153.6 MB (153579854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:742a98177295e32b0bc88d6a1e64e2ff9abd71c350bfc3357830f4634a650bae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.4 MB (226379572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3144900fdfaa2b4486324df2ecd5a82c8f3e7987f46e44589b8e88418ffed7c5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:11 GMT
ADD file:c657b467ecb15f1f4a49a5f04a525f38924750c8187c9ef9f0b886d0264e21f1 in / 
# Tue, 25 Oct 2022 01:23:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:37:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:37:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 02:38:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:40:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a63328f08dbd14148b5ffe154c18846ead48e759779d007b78ec3fb19f5f43a5`  
		Last Modified: Tue, 25 Oct 2022 01:24:36 GMT  
		Size: 27.0 MB (27016028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc7f4256f9365e6546f5def4594e750767ee106712ba11997c58b0e9b15ab10a`  
		Last Modified: Tue, 25 Oct 2022 02:52:05 GMT  
		Size: 7.4 MB (7390068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c49cddcfee6d6315b4a734cc802ff8d05a8ecb16654aeca9cbd0076b7dec22f`  
		Last Modified: Tue, 25 Oct 2022 02:52:04 GMT  
		Size: 3.5 MB (3542342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8b09e3088369fc4b7c4afe1c6fa3627b4a08b7f6388e1e455d9bbb75dbe837`  
		Last Modified: Tue, 25 Oct 2022 02:52:20 GMT  
		Size: 60.0 MB (60019048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:182b0410bb16e1bb8d9c66620b8886fe5f6f64897e68159d3247d1ef9d1686a5`  
		Last Modified: Tue, 25 Oct 2022 02:52:43 GMT  
		Size: 128.4 MB (128412086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:20.04-curl`

```console
$ docker pull buildpack-deps@sha256:26c49a9dc3d707e42cd1c397e82457dfe3a7e634512d308f107ac3ce2fbb8e11
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
$ docker pull buildpack-deps@sha256:577ab5375346239a411e7b8a20882febf76564a20092492c60089c9614bd58fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.9 MB (39946087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac3978effc4af1fb7f140324ee1b2ef790c7b87608d8633f6099ac4a442193e0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:04:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:04:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7215646fa628a9c18e31f7ea7321ae4140b44d69995ec4cdf3968cbce9a5c0b4`  
		Last Modified: Wed, 05 Oct 2022 01:23:38 GMT  
		Size: 7.7 MB (7747231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6c7ee6250b02a6cf0a3a3080d082e4ce4f858e2749921bc2623c896c487897`  
		Last Modified: Wed, 05 Oct 2022 01:23:37 GMT  
		Size: 3.6 MB (3624405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:8b15c3f4b12c531ad54a4129ad38bc19cb166573ec4213563fc6bf9ee949f5dd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34433973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3679946ffe22fbdc937f477ccad2f1008636611a792de1cc56c09bc3c310d8e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:44 GMT
ADD file:75870468a948359044fa3df6c07c80badfea3dcde4823d41a19285436c40cf76 in / 
# Wed, 05 Oct 2022 00:13:44 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:42:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:42:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e679d63f382033c15f8f921851bd71fb8a85a432c0a7a612bbef16e989075145`  
		Last Modified: Wed, 05 Oct 2022 00:15:44 GMT  
		Size: 24.6 MB (24590092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8314cec2c7a441a36532dc89979b531fd7dab365416e8d4f077f16c6322a222`  
		Last Modified: Wed, 05 Oct 2022 00:59:17 GMT  
		Size: 6.7 MB (6740274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b75361ec0073f1728c7bbc9fbf5e55f5ffc978176453aaccd3f3097a710904`  
		Last Modified: Wed, 05 Oct 2022 00:59:16 GMT  
		Size: 3.1 MB (3103607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:24ebe2372b2d4d6605c25b48eb53d26516e00fd2f83265e47a8412192928063b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.4 MB (38429816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bb123f8970cfe7554a7c140d5f8ef986976f115ef6e59c08649ff0a4772a7b9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:09:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:09:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f7d42f1359bed862a992a062b3c7cf025e6bf6625dc1ca56ae2c66d7250fba`  
		Last Modified: Tue, 25 Oct 2022 08:34:12 GMT  
		Size: 7.6 MB (7616212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc75acb9c1e02b10ddc3966608ccbac66c6fd9eeb3bff80797f9983f268a9b1a`  
		Last Modified: Tue, 25 Oct 2022 08:34:12 GMT  
		Size: 3.6 MB (3617606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:403b348e50e731cf4a159fec7726249774627b7984d345dd0e4bb9f472515693
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46492466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b086a827e90970916ae80203e8045e5d422fdac19df4dd7e561d8f844aaf5b96`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:47 GMT
ADD file:013ddcea49540903962069a03762fe471452e8cf00bafeb530724940405797e1 in / 
# Tue, 25 Oct 2022 03:25:49 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:27:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:27:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:42e5f4d60d38e5070be91d6965be1cff1294e6dc275038002dc2ef1812233b0e`  
		Last Modified: Tue, 25 Oct 2022 03:27:44 GMT  
		Size: 33.3 MB (33300542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa48197ece6cedfce46328b98e2bd3ffa7f116e92dc0cd9aba21390a5edf11f`  
		Last Modified: Tue, 25 Oct 2022 06:54:02 GMT  
		Size: 8.7 MB (8705088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b91159ec91712ffe519d3e9624103d9ec7b58e6b1959cad0b77145851e14fc55`  
		Last Modified: Tue, 25 Oct 2022 06:54:01 GMT  
		Size: 4.5 MB (4486836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:03f6b7e0468f3a039213527067a008db1cef213244a75d3406a175aa2d68b215
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34113041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:629e46285cd96bbf2061784773e791fccde26297e92c9cf51561f276b3c6fc5c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:12:13 GMT
ADD file:8c408c11e1eeed71fdd784404ddf9ac52b700161e6187e2313c2751d756e3442 in / 
# Wed, 05 Oct 2022 00:12:14 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:43:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:43:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:edcdeceb0859700b9f2e87516c30c0049092e29666696c30e6b862e0df3d4961`  
		Last Modified: Wed, 05 Oct 2022 00:29:16 GMT  
		Size: 24.2 MB (24242839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750231dc28469e93ce7c6e7d14be0b30332503e15a9a7516729ab0815bbeb749`  
		Last Modified: Wed, 05 Oct 2022 03:42:06 GMT  
		Size: 6.7 MB (6725280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3455cf9ca9db352ee4e1bdf9c1bd8bd85713203a5b2ae128f9a7d02af28fea50`  
		Last Modified: Wed, 05 Oct 2022 03:42:00 GMT  
		Size: 3.1 MB (3144922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:1a57b03716bdc4d36ffbc98cfc91f6bcf59d28fd7d79b1b189bfc0d6e8aeeeb2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37948438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45eb95eb88b1bfec442d1a02a64ad20f4424239eb7f44b117ae092061619489d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:11 GMT
ADD file:c657b467ecb15f1f4a49a5f04a525f38924750c8187c9ef9f0b886d0264e21f1 in / 
# Tue, 25 Oct 2022 01:23:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:37:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:37:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a63328f08dbd14148b5ffe154c18846ead48e759779d007b78ec3fb19f5f43a5`  
		Last Modified: Tue, 25 Oct 2022 01:24:36 GMT  
		Size: 27.0 MB (27016028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc7f4256f9365e6546f5def4594e750767ee106712ba11997c58b0e9b15ab10a`  
		Last Modified: Tue, 25 Oct 2022 02:52:05 GMT  
		Size: 7.4 MB (7390068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c49cddcfee6d6315b4a734cc802ff8d05a8ecb16654aeca9cbd0076b7dec22f`  
		Last Modified: Tue, 25 Oct 2022 02:52:04 GMT  
		Size: 3.5 MB (3542342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:20.04-scm`

```console
$ docker pull buildpack-deps@sha256:aa83529c20e9637d81c8bb79ec8042bb08701d8e0aeb6700ce4bceddb07c2155
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
$ docker pull buildpack-deps@sha256:3fbf9b728805f4855a1e1714abd1122f590819c3c940af6add1e74b6edb1a583
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.7 MB (100684328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:556eaf86e2c531f983516419b73441c5850909052e50ab552d75a9d7b29130a5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:04:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:04:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:05:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7215646fa628a9c18e31f7ea7321ae4140b44d69995ec4cdf3968cbce9a5c0b4`  
		Last Modified: Wed, 05 Oct 2022 01:23:38 GMT  
		Size: 7.7 MB (7747231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6c7ee6250b02a6cf0a3a3080d082e4ce4f858e2749921bc2623c896c487897`  
		Last Modified: Wed, 05 Oct 2022 01:23:37 GMT  
		Size: 3.6 MB (3624405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927ce100b3517cefcb05b92b71a8c91e9881466e25f273c9ce8b59ade42ef3a3`  
		Last Modified: Wed, 05 Oct 2022 01:23:58 GMT  
		Size: 60.7 MB (60738241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ea745c791fe0fd9b6b7bf04130cdc270995b03279f2c411722ff840cd212ead9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.9 MB (89875111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddd42e22b4a80d23d5304ea494d56e753af1132c2869050e028ca61cc3f46c61`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:44 GMT
ADD file:75870468a948359044fa3df6c07c80badfea3dcde4823d41a19285436c40cf76 in / 
# Wed, 05 Oct 2022 00:13:44 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:42:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:42:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:43:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e679d63f382033c15f8f921851bd71fb8a85a432c0a7a612bbef16e989075145`  
		Last Modified: Wed, 05 Oct 2022 00:15:44 GMT  
		Size: 24.6 MB (24590092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8314cec2c7a441a36532dc89979b531fd7dab365416e8d4f077f16c6322a222`  
		Last Modified: Wed, 05 Oct 2022 00:59:17 GMT  
		Size: 6.7 MB (6740274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b75361ec0073f1728c7bbc9fbf5e55f5ffc978176453aaccd3f3097a710904`  
		Last Modified: Wed, 05 Oct 2022 00:59:16 GMT  
		Size: 3.1 MB (3103607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0cd29b8c09506d2393921adb0cded05dba5f57e529ff475ad92160d2b38c475`  
		Last Modified: Wed, 05 Oct 2022 00:59:45 GMT  
		Size: 55.4 MB (55441138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:328e8c05b0f0341747f5871823ad81ae7ac6e958a44be976bcca059cc132912e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99237200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:238b304b5e34bc73bb2557c4303d7a9380f67900d30cac408cfa2c46b7c6b625`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:09:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:09:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:10:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f7d42f1359bed862a992a062b3c7cf025e6bf6625dc1ca56ae2c66d7250fba`  
		Last Modified: Tue, 25 Oct 2022 08:34:12 GMT  
		Size: 7.6 MB (7616212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc75acb9c1e02b10ddc3966608ccbac66c6fd9eeb3bff80797f9983f268a9b1a`  
		Last Modified: Tue, 25 Oct 2022 08:34:12 GMT  
		Size: 3.6 MB (3617606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d21db26b13141f20e7cce995a63f8234838277895d2d6d0e2ec4f35e659c78`  
		Last Modified: Tue, 25 Oct 2022 08:34:33 GMT  
		Size: 60.8 MB (60807384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:0b5156fdea407f78ae8f5dd5a40c70d5686fd01e7a1316d3896a123aa5f2d1e8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (116020776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d728b216db5852c775762c0dbeb7021e76038e61147d6565e4df9ebaf321e554`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:47 GMT
ADD file:013ddcea49540903962069a03762fe471452e8cf00bafeb530724940405797e1 in / 
# Tue, 25 Oct 2022 03:25:49 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:27:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:27:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:29:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:42e5f4d60d38e5070be91d6965be1cff1294e6dc275038002dc2ef1812233b0e`  
		Last Modified: Tue, 25 Oct 2022 03:27:44 GMT  
		Size: 33.3 MB (33300542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa48197ece6cedfce46328b98e2bd3ffa7f116e92dc0cd9aba21390a5edf11f`  
		Last Modified: Tue, 25 Oct 2022 06:54:02 GMT  
		Size: 8.7 MB (8705088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b91159ec91712ffe519d3e9624103d9ec7b58e6b1959cad0b77145851e14fc55`  
		Last Modified: Tue, 25 Oct 2022 06:54:01 GMT  
		Size: 4.5 MB (4486836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c68813dea6733b577ebd8f432367b30fab9f0639692bc2e99d633f9347aff6`  
		Last Modified: Tue, 25 Oct 2022 06:54:33 GMT  
		Size: 69.5 MB (69528310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:6e1c097aaa5b10d603b3ca7af97305eb87efa8eb846c6b08fea8968c3a45fe4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.0 MB (97967486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01cb9f67e31afed0eb376d14ac80a2758ecbb81e5ccb14b069d1b33c9da0399f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:11 GMT
ADD file:c657b467ecb15f1f4a49a5f04a525f38924750c8187c9ef9f0b886d0264e21f1 in / 
# Tue, 25 Oct 2022 01:23:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:37:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:37:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 02:38:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a63328f08dbd14148b5ffe154c18846ead48e759779d007b78ec3fb19f5f43a5`  
		Last Modified: Tue, 25 Oct 2022 01:24:36 GMT  
		Size: 27.0 MB (27016028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc7f4256f9365e6546f5def4594e750767ee106712ba11997c58b0e9b15ab10a`  
		Last Modified: Tue, 25 Oct 2022 02:52:05 GMT  
		Size: 7.4 MB (7390068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c49cddcfee6d6315b4a734cc802ff8d05a8ecb16654aeca9cbd0076b7dec22f`  
		Last Modified: Tue, 25 Oct 2022 02:52:04 GMT  
		Size: 3.5 MB (3542342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8b09e3088369fc4b7c4afe1c6fa3627b4a08b7f6388e1e455d9bbb75dbe837`  
		Last Modified: Tue, 25 Oct 2022 02:52:20 GMT  
		Size: 60.0 MB (60019048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.04`

```console
$ docker pull buildpack-deps@sha256:4eb7cafc88b6230a8bed1a8b923d59335967af21faf91b258577a8c692bf4414
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
$ docker pull buildpack-deps@sha256:0a04bf1c7b7015264a105a127d437901cc38216b3e05f80652717d4fbffe1f49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.0 MB (249961758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:799867dd0caf9dc22795fd510b367612d8d37d5e1fc091eebea256c0f1fec1b4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:20 GMT
ADD file:6cd2e13356aa5339c1f2abd3c210a52f6ed74fae05cd61aa09f37b6a4764f65c in / 
# Tue, 04 Oct 2022 23:35:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:09:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:09:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:10:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:13:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cf92e523b49ea3d1fae59f5f082437a5f96c244fda6697995920142ff31d59cf`  
		Last Modified: Tue, 04 Oct 2022 03:04:01 GMT  
		Size: 30.4 MB (30428928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19b9364a5e7fea40b9e9eb4614f0e4533857b602c7fba30362889933ef14298`  
		Last Modified: Wed, 05 Oct 2022 01:24:38 GMT  
		Size: 3.8 MB (3804673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:856d49148d8882ac6866bcbcbaa08bacfe1f0d0d382b73675630ae29d44ae3f2`  
		Last Modified: Wed, 05 Oct 2022 01:24:38 GMT  
		Size: 3.6 MB (3561097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f83374f27f6992ee240fe68ce2e0c2d9db958dc2c9acf1864ef83040cc5387`  
		Last Modified: Wed, 05 Oct 2022 01:24:54 GMT  
		Size: 39.3 MB (39349072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be916118df24025fcea61e45a4784cdf94b7d69e7f9e78290268844a5b3869c`  
		Last Modified: Wed, 05 Oct 2022 01:25:27 GMT  
		Size: 172.8 MB (172817988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:b499e85bc82d56d7053e6deb96cc3a62b6f8b07cea61e9e79aab9378374bfa0f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.6 MB (216595227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99a929445888a8297e1d1e0a72a43df4e15b1986b48a95eab496a572b59cc70d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:57 GMT
ADD file:11e25fc4812528219464289700bb0495bf9298918899103c33d7ef9022690eb0 in / 
# Wed, 05 Oct 2022 00:13:57 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:44:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:45:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:45:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:47:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99b9c73338a7c0dbe41f9fc543fae706650a616453e1e330f870e20916c18a11`  
		Last Modified: Wed, 05 Oct 2022 00:16:02 GMT  
		Size: 27.0 MB (27018632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c337b77409c2e34b5e69df73a11e0ef62cd00b8b23e7d6776235d6491726ac80`  
		Last Modified: Wed, 05 Oct 2022 01:00:37 GMT  
		Size: 3.6 MB (3555370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a1dc485f1a7e2433bb9a4501dac3fb4727fb7708715e743277a50ba4933ca1`  
		Last Modified: Wed, 05 Oct 2022 01:00:37 GMT  
		Size: 3.7 MB (3712768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5595ebdf3f8239b659bdbfc55b5e0a70965f29a4e546cc5efdda43f8e3a4ef76`  
		Last Modified: Wed, 05 Oct 2022 01:01:00 GMT  
		Size: 41.9 MB (41900106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e2ea778678da62e1245bc9a3cc4044027e3903041d44869b3d3d6e1039ce53`  
		Last Modified: Wed, 05 Oct 2022 01:01:41 GMT  
		Size: 140.4 MB (140408351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3062403000f5efd37324066992c8bdb0d10becc4c9f71cda23a5964934215fe1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.3 MB (241329313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b53b6e726046563cf829cd77f37b736f5cac3bc10e64cc69c786796131519ce`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:55:02 GMT
ADD file:515177312f20fb1814b89bfccfe695fa2354bbb6d43fdb6e018bf5b1acc17e9f in / 
# Tue, 25 Oct 2022 05:55:02 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:14:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:14:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:15:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:18:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:56a2caa6b2c66e01954c1a013b37ea359b6e6af8989dbfb958124b6318771af4`  
		Last Modified: Tue, 25 Oct 2022 05:56:14 GMT  
		Size: 28.4 MB (28382489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85c75d65daee139419e66b36968af1443c6839bbfa07f1ff10f41c14059531f8`  
		Last Modified: Tue, 25 Oct 2022 08:35:08 GMT  
		Size: 3.8 MB (3776223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b571e5291fabe657fef93ed4c8e7109c81e0538a58853a65f33d52b4aa5a9f`  
		Last Modified: Tue, 25 Oct 2022 08:35:08 GMT  
		Size: 3.5 MB (3535453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d47a2b6e938e7cf8632d33777355c83ebf1eb36d91c3dc64efc269e15e34ddb`  
		Last Modified: Tue, 25 Oct 2022 08:35:23 GMT  
		Size: 39.2 MB (39236083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8135ee8a3cbc8d92cf867f078f0e7c23411bc10d28f13c3bac60472392514a98`  
		Last Modified: Tue, 25 Oct 2022 08:35:50 GMT  
		Size: 166.4 MB (166399065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:860ed8bcd4c5c4c962c3fdc88871467e7f44c8908c33faea5b7ceea1b6fb14b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.8 MB (271828709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:322a2cb433f862a334e63b1447de75d88df78488ae1653acc45c6d6672584436`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:26:00 GMT
ADD file:766b7743de4ed1a194fc749b7649d245b0cd545b03cc2c81f16a6c15e91c87e7 in / 
# Tue, 25 Oct 2022 03:26:02 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:33:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:33:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:34:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:39:09 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:aa33126e789290559dc146af02cbf168119ed23be1e30fd99fe8572956e50616`  
		Last Modified: Tue, 25 Oct 2022 03:28:08 GMT  
		Size: 35.7 MB (35709401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6373837e7f2a85c7283b43d7d1a07f2541140a0a6287dc704fdf1df6ed09c5e`  
		Last Modified: Tue, 25 Oct 2022 06:55:38 GMT  
		Size: 4.3 MB (4276445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:847050f2ae34b2e1019b09f2bdbac09fd4a3c7efcaf4545aa162094c15b7f016`  
		Last Modified: Tue, 25 Oct 2022 06:55:38 GMT  
		Size: 4.2 MB (4234460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186cf1c98556ab0c2ae47af200ed2f3a8f340ad4cd305379f23619197f2ec188`  
		Last Modified: Tue, 25 Oct 2022 06:56:02 GMT  
		Size: 43.8 MB (43753297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9009bf6240bebccdaeaec57cdd31c0023771a5c2e59499153ff583df56ad8429`  
		Last Modified: Tue, 25 Oct 2022 06:56:57 GMT  
		Size: 183.9 MB (183855106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:883d6acf11862386cb075d26a5eeb067aecd009e926bf289a86848849796adbc
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.9 MB (274910739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ccd65b0e2c99958523b95730fa70b845815fe14d64756c2e1dbf17d4eb51ba0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:14:15 GMT
ADD file:e1fa146cf8e97dd6a2f3ebb2dacba539556ef4a1e87dc53bd745a3cf0ba10aef in / 
# Wed, 05 Oct 2022 00:14:16 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:46:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:47:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 02:51:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:57:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cbeff255552ba792be63b343113968df42de6f599d1372edd4c7346d08dfeace`  
		Last Modified: Wed, 05 Oct 2022 00:31:39 GMT  
		Size: 27.7 MB (27747416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6129e2d138d3d5141f87ef04090f82aeeb874b1d1e3c6f6e94d843cd2447826`  
		Last Modified: Wed, 05 Oct 2022 03:43:29 GMT  
		Size: 3.6 MB (3598134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a1ba2d60715be154c4f520ac4f1ef149f66b921651ab2726a809c14316e55a`  
		Last Modified: Wed, 05 Oct 2022 03:43:27 GMT  
		Size: 3.8 MB (3778196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91414a4a50607595a5e83cc27ee8f8e885ea1d1c43848a3df1487911ae62cc19`  
		Last Modified: Wed, 05 Oct 2022 03:45:48 GMT  
		Size: 42.1 MB (42114477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b2617d47bf73f10f7e72de1aef1781f5db0ee40d20e6f41b05861a722e3d8e`  
		Last Modified: Wed, 05 Oct 2022 03:52:56 GMT  
		Size: 197.7 MB (197672516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a029d0d8ff77597549c4887e0b7c71c4c2dc6c5b837db8eaa6edbcbdf5c56729
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.7 MB (223702443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c21ca30b7fafab565f525a6aeb99324f35dad0e19bfc20af0c4aabe5d9f01f7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:21 GMT
ADD file:d9af7670f58e9478e400dac85a0fcb07a4209846dbd1ea560fdc6de6e2cb5e4e in / 
# Tue, 25 Oct 2022 01:23:22 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:40:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:40:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 02:41:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:43:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9aed974aece14dd3aed00810d58a89e87eb5be9ad1c6fbb1ed077dc3f145dccc`  
		Last Modified: Tue, 25 Oct 2022 01:24:48 GMT  
		Size: 28.6 MB (28641668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0474dffae2d1e16bb420718a81adc05c65e7cf46cfec815544e0ed630334ee45`  
		Last Modified: Tue, 25 Oct 2022 02:52:51 GMT  
		Size: 3.8 MB (3809925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdff4ace6c098f616aa6e4ddee394e5472cdf30f97f3b22e0dc26d42d42e234`  
		Last Modified: Tue, 25 Oct 2022 02:52:50 GMT  
		Size: 3.5 MB (3472443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92140a87366357bdb10310a5cb8497d894c21c28e686a09af051436e071d5075`  
		Last Modified: Tue, 25 Oct 2022 02:53:04 GMT  
		Size: 39.3 MB (39282461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbee90fa764eaad308daac34a4b01988b99caaacb98cb0406b358fbe0189c634`  
		Last Modified: Tue, 25 Oct 2022 02:53:28 GMT  
		Size: 148.5 MB (148495946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.04-curl`

```console
$ docker pull buildpack-deps@sha256:ddf553ac35b8e1c73edae378982907fffdf1efaa9b9feb2252bdf37fc789e1db
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
$ docker pull buildpack-deps@sha256:c7cae1ebcf24a005d9b891b12f383a883c7f895687513539d29e2bd2c232c277
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37794698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35f4a6fc9e8fc4a47f232b1e95bf6c08b6eebe56c156237c14846c8ca8cc33aa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:20 GMT
ADD file:6cd2e13356aa5339c1f2abd3c210a52f6ed74fae05cd61aa09f37b6a4764f65c in / 
# Tue, 04 Oct 2022 23:35:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:09:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:09:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:cf92e523b49ea3d1fae59f5f082437a5f96c244fda6697995920142ff31d59cf`  
		Last Modified: Tue, 04 Oct 2022 03:04:01 GMT  
		Size: 30.4 MB (30428928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19b9364a5e7fea40b9e9eb4614f0e4533857b602c7fba30362889933ef14298`  
		Last Modified: Wed, 05 Oct 2022 01:24:38 GMT  
		Size: 3.8 MB (3804673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:856d49148d8882ac6866bcbcbaa08bacfe1f0d0d382b73675630ae29d44ae3f2`  
		Last Modified: Wed, 05 Oct 2022 01:24:38 GMT  
		Size: 3.6 MB (3561097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:89e3caec70fda990f819f3531875b9b314c843b4dd840be4234868015633048e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34286770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ce49fd48b1ba4f7396facd63ca2177d567b41ea796aae1f686d42df955bc0e9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:57 GMT
ADD file:11e25fc4812528219464289700bb0495bf9298918899103c33d7ef9022690eb0 in / 
# Wed, 05 Oct 2022 00:13:57 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:44:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:45:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:99b9c73338a7c0dbe41f9fc543fae706650a616453e1e330f870e20916c18a11`  
		Last Modified: Wed, 05 Oct 2022 00:16:02 GMT  
		Size: 27.0 MB (27018632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c337b77409c2e34b5e69df73a11e0ef62cd00b8b23e7d6776235d6491726ac80`  
		Last Modified: Wed, 05 Oct 2022 01:00:37 GMT  
		Size: 3.6 MB (3555370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a1dc485f1a7e2433bb9a4501dac3fb4727fb7708715e743277a50ba4933ca1`  
		Last Modified: Wed, 05 Oct 2022 01:00:37 GMT  
		Size: 3.7 MB (3712768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:cde36d71bbe4425cd9a8fb5d75a26f77d01d71b9e6d658f8784a56d78df99760
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35694165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35a2b15ea2ec567cdf8db58cf77a502d8fe85f3a84932dc89b54aafc94a6d716`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:55:02 GMT
ADD file:515177312f20fb1814b89bfccfe695fa2354bbb6d43fdb6e018bf5b1acc17e9f in / 
# Tue, 25 Oct 2022 05:55:02 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:14:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:14:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:56a2caa6b2c66e01954c1a013b37ea359b6e6af8989dbfb958124b6318771af4`  
		Last Modified: Tue, 25 Oct 2022 05:56:14 GMT  
		Size: 28.4 MB (28382489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85c75d65daee139419e66b36968af1443c6839bbfa07f1ff10f41c14059531f8`  
		Last Modified: Tue, 25 Oct 2022 08:35:08 GMT  
		Size: 3.8 MB (3776223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b571e5291fabe657fef93ed4c8e7109c81e0538a58853a65f33d52b4aa5a9f`  
		Last Modified: Tue, 25 Oct 2022 08:35:08 GMT  
		Size: 3.5 MB (3535453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:e149ccd1fd8c23ad674ee2e9cb1640264f96480646dce6134a50c9e1f1e2755a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44220306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f1727c427b596139f4521abd4689b24bbfa286d1a6220a86f3a1705080d7778`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:26:00 GMT
ADD file:766b7743de4ed1a194fc749b7649d245b0cd545b03cc2c81f16a6c15e91c87e7 in / 
# Tue, 25 Oct 2022 03:26:02 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:33:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:33:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:aa33126e789290559dc146af02cbf168119ed23be1e30fd99fe8572956e50616`  
		Last Modified: Tue, 25 Oct 2022 03:28:08 GMT  
		Size: 35.7 MB (35709401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6373837e7f2a85c7283b43d7d1a07f2541140a0a6287dc704fdf1df6ed09c5e`  
		Last Modified: Tue, 25 Oct 2022 06:55:38 GMT  
		Size: 4.3 MB (4276445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:847050f2ae34b2e1019b09f2bdbac09fd4a3c7efcaf4545aa162094c15b7f016`  
		Last Modified: Tue, 25 Oct 2022 06:55:38 GMT  
		Size: 4.2 MB (4234460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:674baad7923a60a55b6a139740aa1dd03ec351bca096cec8eef67d577490dce6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35123746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:165bda599f3c7984f6273e3a5eccf5326245110c5394238add81f83ae779e6e6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:14:15 GMT
ADD file:e1fa146cf8e97dd6a2f3ebb2dacba539556ef4a1e87dc53bd745a3cf0ba10aef in / 
# Wed, 05 Oct 2022 00:14:16 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:46:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:47:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:cbeff255552ba792be63b343113968df42de6f599d1372edd4c7346d08dfeace`  
		Last Modified: Wed, 05 Oct 2022 00:31:39 GMT  
		Size: 27.7 MB (27747416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6129e2d138d3d5141f87ef04090f82aeeb874b1d1e3c6f6e94d843cd2447826`  
		Last Modified: Wed, 05 Oct 2022 03:43:29 GMT  
		Size: 3.6 MB (3598134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a1ba2d60715be154c4f520ac4f1ef149f66b921651ab2726a809c14316e55a`  
		Last Modified: Wed, 05 Oct 2022 03:43:27 GMT  
		Size: 3.8 MB (3778196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:c9f438fe30404f17ac10a8f79981bf6ab4f788d3706b23e99b92133fa1133a58
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35924036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13ac7d74d18b331d205348291551e18d9bd7010f18fc44d6f55875b60652fdf1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:21 GMT
ADD file:d9af7670f58e9478e400dac85a0fcb07a4209846dbd1ea560fdc6de6e2cb5e4e in / 
# Tue, 25 Oct 2022 01:23:22 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:40:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:40:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9aed974aece14dd3aed00810d58a89e87eb5be9ad1c6fbb1ed077dc3f145dccc`  
		Last Modified: Tue, 25 Oct 2022 01:24:48 GMT  
		Size: 28.6 MB (28641668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0474dffae2d1e16bb420718a81adc05c65e7cf46cfec815544e0ed630334ee45`  
		Last Modified: Tue, 25 Oct 2022 02:52:51 GMT  
		Size: 3.8 MB (3809925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdff4ace6c098f616aa6e4ddee394e5472cdf30f97f3b22e0dc26d42d42e234`  
		Last Modified: Tue, 25 Oct 2022 02:52:50 GMT  
		Size: 3.5 MB (3472443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.04-scm`

```console
$ docker pull buildpack-deps@sha256:6625116a3d22e3df460e9151fa87afc625bcee4797882f9fd56f946c8b7d587f
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
$ docker pull buildpack-deps@sha256:dd6a1375f1f144120e73c33263d15fad407cdf3af5700bf06b98c42e712a0d2a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77143770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da5fb79923d815372876a15ca9afa7294969ee8f6142ae8377dd987dd91de455`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:20 GMT
ADD file:6cd2e13356aa5339c1f2abd3c210a52f6ed74fae05cd61aa09f37b6a4764f65c in / 
# Tue, 04 Oct 2022 23:35:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:09:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:09:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:10:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cf92e523b49ea3d1fae59f5f082437a5f96c244fda6697995920142ff31d59cf`  
		Last Modified: Tue, 04 Oct 2022 03:04:01 GMT  
		Size: 30.4 MB (30428928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19b9364a5e7fea40b9e9eb4614f0e4533857b602c7fba30362889933ef14298`  
		Last Modified: Wed, 05 Oct 2022 01:24:38 GMT  
		Size: 3.8 MB (3804673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:856d49148d8882ac6866bcbcbaa08bacfe1f0d0d382b73675630ae29d44ae3f2`  
		Last Modified: Wed, 05 Oct 2022 01:24:38 GMT  
		Size: 3.6 MB (3561097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f83374f27f6992ee240fe68ce2e0c2d9db958dc2c9acf1864ef83040cc5387`  
		Last Modified: Wed, 05 Oct 2022 01:24:54 GMT  
		Size: 39.3 MB (39349072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:8ee2ceb7f89309d35af0ffd83a4e9f99593da3ebc818ef9db16edea6807e5999
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76186876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ac586f0d0ef3e15932beb867ebeae6c400aec079dbb4e9675345a7b3a0cfb07`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:57 GMT
ADD file:11e25fc4812528219464289700bb0495bf9298918899103c33d7ef9022690eb0 in / 
# Wed, 05 Oct 2022 00:13:57 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:44:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:45:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:45:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99b9c73338a7c0dbe41f9fc543fae706650a616453e1e330f870e20916c18a11`  
		Last Modified: Wed, 05 Oct 2022 00:16:02 GMT  
		Size: 27.0 MB (27018632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c337b77409c2e34b5e69df73a11e0ef62cd00b8b23e7d6776235d6491726ac80`  
		Last Modified: Wed, 05 Oct 2022 01:00:37 GMT  
		Size: 3.6 MB (3555370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a1dc485f1a7e2433bb9a4501dac3fb4727fb7708715e743277a50ba4933ca1`  
		Last Modified: Wed, 05 Oct 2022 01:00:37 GMT  
		Size: 3.7 MB (3712768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5595ebdf3f8239b659bdbfc55b5e0a70965f29a4e546cc5efdda43f8e3a4ef76`  
		Last Modified: Wed, 05 Oct 2022 01:01:00 GMT  
		Size: 41.9 MB (41900106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ba599423790494bb456afcac072a93c962e4ec9d980064386cabcee48af29d1c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.9 MB (74930248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:808e03b9a2c409feb946d3d926084d928f7da4f40a01604e98dafd06b7f57b9e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:55:02 GMT
ADD file:515177312f20fb1814b89bfccfe695fa2354bbb6d43fdb6e018bf5b1acc17e9f in / 
# Tue, 25 Oct 2022 05:55:02 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:14:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:14:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:15:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:56a2caa6b2c66e01954c1a013b37ea359b6e6af8989dbfb958124b6318771af4`  
		Last Modified: Tue, 25 Oct 2022 05:56:14 GMT  
		Size: 28.4 MB (28382489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85c75d65daee139419e66b36968af1443c6839bbfa07f1ff10f41c14059531f8`  
		Last Modified: Tue, 25 Oct 2022 08:35:08 GMT  
		Size: 3.8 MB (3776223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b571e5291fabe657fef93ed4c8e7109c81e0538a58853a65f33d52b4aa5a9f`  
		Last Modified: Tue, 25 Oct 2022 08:35:08 GMT  
		Size: 3.5 MB (3535453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d47a2b6e938e7cf8632d33777355c83ebf1eb36d91c3dc64efc269e15e34ddb`  
		Last Modified: Tue, 25 Oct 2022 08:35:23 GMT  
		Size: 39.2 MB (39236083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:9d256e35b3c4819a62e8a49fcf0872c6714d2d5ae957d9812046d42db0aa388b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.0 MB (87973603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b228d7257419ba62688701d08a6f0b18e366ccb8c7796bd83cc3c3b1ae61030b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:26:00 GMT
ADD file:766b7743de4ed1a194fc749b7649d245b0cd545b03cc2c81f16a6c15e91c87e7 in / 
# Tue, 25 Oct 2022 03:26:02 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:33:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:33:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:34:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:aa33126e789290559dc146af02cbf168119ed23be1e30fd99fe8572956e50616`  
		Last Modified: Tue, 25 Oct 2022 03:28:08 GMT  
		Size: 35.7 MB (35709401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6373837e7f2a85c7283b43d7d1a07f2541140a0a6287dc704fdf1df6ed09c5e`  
		Last Modified: Tue, 25 Oct 2022 06:55:38 GMT  
		Size: 4.3 MB (4276445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:847050f2ae34b2e1019b09f2bdbac09fd4a3c7efcaf4545aa162094c15b7f016`  
		Last Modified: Tue, 25 Oct 2022 06:55:38 GMT  
		Size: 4.2 MB (4234460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186cf1c98556ab0c2ae47af200ed2f3a8f340ad4cd305379f23619197f2ec188`  
		Last Modified: Tue, 25 Oct 2022 06:56:02 GMT  
		Size: 43.8 MB (43753297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:0b59c501076932d75abe6baf6b45272617ca658c00bea23c4c642ecf0cef54ad
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77238223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c179e15b046f9a7a277678332c1ba0ff71c2985288dede5b120f176dbd7b378`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:14:15 GMT
ADD file:e1fa146cf8e97dd6a2f3ebb2dacba539556ef4a1e87dc53bd745a3cf0ba10aef in / 
# Wed, 05 Oct 2022 00:14:16 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:46:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:47:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 02:51:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cbeff255552ba792be63b343113968df42de6f599d1372edd4c7346d08dfeace`  
		Last Modified: Wed, 05 Oct 2022 00:31:39 GMT  
		Size: 27.7 MB (27747416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6129e2d138d3d5141f87ef04090f82aeeb874b1d1e3c6f6e94d843cd2447826`  
		Last Modified: Wed, 05 Oct 2022 03:43:29 GMT  
		Size: 3.6 MB (3598134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a1ba2d60715be154c4f520ac4f1ef149f66b921651ab2726a809c14316e55a`  
		Last Modified: Wed, 05 Oct 2022 03:43:27 GMT  
		Size: 3.8 MB (3778196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91414a4a50607595a5e83cc27ee8f8e885ea1d1c43848a3df1487911ae62cc19`  
		Last Modified: Wed, 05 Oct 2022 03:45:48 GMT  
		Size: 42.1 MB (42114477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:1261bcd972c83821318a0ffbee775f7c50792bde771fc73c806e78a7af67b584
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75206497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44680731da527ce74344c9ff0197ff653c79174a875a4711b0b82402a398c303`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:21 GMT
ADD file:d9af7670f58e9478e400dac85a0fcb07a4209846dbd1ea560fdc6de6e2cb5e4e in / 
# Tue, 25 Oct 2022 01:23:22 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:40:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:40:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 02:41:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9aed974aece14dd3aed00810d58a89e87eb5be9ad1c6fbb1ed077dc3f145dccc`  
		Last Modified: Tue, 25 Oct 2022 01:24:48 GMT  
		Size: 28.6 MB (28641668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0474dffae2d1e16bb420718a81adc05c65e7cf46cfec815544e0ed630334ee45`  
		Last Modified: Tue, 25 Oct 2022 02:52:51 GMT  
		Size: 3.8 MB (3809925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdff4ace6c098f616aa6e4ddee394e5472cdf30f97f3b22e0dc26d42d42e234`  
		Last Modified: Tue, 25 Oct 2022 02:52:50 GMT  
		Size: 3.5 MB (3472443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92140a87366357bdb10310a5cb8497d894c21c28e686a09af051436e071d5075`  
		Last Modified: Tue, 25 Oct 2022 02:53:04 GMT  
		Size: 39.3 MB (39282461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.10`

```console
$ docker pull buildpack-deps@sha256:4bb8f04c36a68d87bb5d569f8ef15acf77df7d6d27bb36b3b935211fddc8acd2
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
$ docker pull buildpack-deps@sha256:b33788a433b2f998ebd368f99762872a3c6c6009abe173f62fb4e1e94c9ae7a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.8 MB (265793471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:622366e2d78507bc25ad39ba5e3b6c6a4b43d982571e1a8250ba68d37223db3e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:28 GMT
ADD file:3384549425c94b92a7d7be15958e3ec7494bdf83242deb465d9059d4362d34d6 in / 
# Tue, 04 Oct 2022 23:35:28 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:13:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:13:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:14:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:16:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5887826a0d8b4c403d9bfaf57279fd8b585d272c3f450d374349365dc22cd8ef`  
		Last Modified: Tue, 04 Oct 2022 23:36:56 GMT  
		Size: 27.5 MB (27455077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b7fd9cb5adf6a195c3c2162caa409d926d4342598cad09f7fa4691e9ddd25f`  
		Last Modified: Wed, 05 Oct 2022 01:25:38 GMT  
		Size: 6.8 MB (6780586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9023f9ecbe71ceaba400cb934168d975ecabc157d85fe246f71d3d684947742d`  
		Last Modified: Wed, 05 Oct 2022 01:25:37 GMT  
		Size: 3.6 MB (3633909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d44eedd822ec1ffd1b32f87638bae3694f27cf99e85f8d3d8f6d1f2857fdc1`  
		Last Modified: Wed, 05 Oct 2022 01:25:54 GMT  
		Size: 39.7 MB (39713928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46cfc3a166e18ca21a45cacaeec49e724ff39c9215001117796bd74cb3b40410`  
		Last Modified: Wed, 05 Oct 2022 01:26:30 GMT  
		Size: 188.2 MB (188209971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:d55d7353e6aa732cad00a73a6c198a481ba08a5afd55721ac086a1017b1559ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.1 MB (228118532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10bca3a5fa8bf85ff72ac75e507466eacf465294389c059f87eb1ceaa37efa93`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:14:09 GMT
ADD file:4b538f2c7b46aa601d747159ce9e8c2c7a99b2b6e09e4efe1073ca58e47fbeed in / 
# Wed, 05 Oct 2022 00:14:09 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:47:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:47:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:48:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:49:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:788f7bb1e1d719f6a9a9b3b1530cc5bbe5b808a2ad77a65f23e2c6d15b8ae546`  
		Last Modified: Wed, 05 Oct 2022 00:16:28 GMT  
		Size: 25.9 MB (25873193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31aeed2022326b456329596b112851c2e027ba5773dab33fcd717efb1a016274`  
		Last Modified: Wed, 05 Oct 2022 01:01:56 GMT  
		Size: 6.0 MB (5955685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b8a4829745394c3402e5970b4558ef9fe23515f895e7f8a99fe24ae33a7c4f3`  
		Last Modified: Wed, 05 Oct 2022 01:01:55 GMT  
		Size: 3.8 MB (3801708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199fb45c30ad58843e78384afd22f7dec65ac55a285086da2083dea2426fd37e`  
		Last Modified: Wed, 05 Oct 2022 01:02:19 GMT  
		Size: 42.6 MB (42596389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd5d37220a8883d442a1686f49907c73299d8c1df3d5f6cc9a9d1b8c9012583`  
		Last Modified: Wed, 05 Oct 2022 01:03:07 GMT  
		Size: 149.9 MB (149891557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7f591bb67e4190e35105756af84f44d4bdd7c020d451632335a530a83e8e299a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.6 MB (246644046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:418c243a099dd8aadaf491de0633949554b9e17b02bb3dbecaeba22314be0c60`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:55:06 GMT
ADD file:30361063c284df6e20a85ff95b9c7b93648fe9e04ac935c9ff888e5c5f3af7ea in / 
# Tue, 25 Oct 2022 05:55:06 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:19:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:19:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:20:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:23:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a2e58a4bc1e52e3ab8904706a68a79146364ec32d8caf1bd106c3c9966a38fc`  
		Last Modified: Tue, 25 Oct 2022 05:56:30 GMT  
		Size: 26.7 MB (26676995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208c8913a9c66f64a1f5ca1349c8a8b9923f9eb9c8aed25bf3ec160a33e5a796`  
		Last Modified: Tue, 25 Oct 2022 08:36:03 GMT  
		Size: 6.6 MB (6607031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8491d7cc7a42af61771e26652e91532db813e380fa19339f7279420206df0290`  
		Last Modified: Tue, 25 Oct 2022 08:36:03 GMT  
		Size: 3.6 MB (3602476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2cf60ff33717c4a17f0ca2f77473b69d8d357e4dc81ef8bb8a5e24382aa106`  
		Last Modified: Tue, 25 Oct 2022 08:36:17 GMT  
		Size: 39.5 MB (39486568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2297c22e5e80de066ab641f5f47a060831dda9dbda728c9ffc0333ffd65aec38`  
		Last Modified: Tue, 25 Oct 2022 08:36:45 GMT  
		Size: 170.3 MB (170270976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:b85564067cd24e7645a51fcc5b5ee66f50498a7a4cad4db8f8e748271b4cbfe0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.3 MB (281263738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:402a9d4fffb8624f6fa449162bbd5c6ef48031ba4a3813d392416260f6ab5055`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:26:14 GMT
ADD file:60dd11bbfa9f1e2bc613c7f05cbbb83bca9e4b81550b6a0540a5d1d39f870cdd in / 
# Tue, 25 Oct 2022 03:26:16 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:40:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:40:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:41:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:44:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6d37bc653a986baef621c195bf8def80ca65133b8a3917bbd3a148b31bc1704f`  
		Last Modified: Tue, 25 Oct 2022 03:28:34 GMT  
		Size: 32.1 MB (32099941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc18decfda3085820c97e73c59dba18c534c4455c2eafc5812d29975ad7a9292`  
		Last Modified: Tue, 25 Oct 2022 06:57:12 GMT  
		Size: 7.8 MB (7752006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a931134d9aa21913f6400e3083b4c6955008f9fab7eae04019249a1d912c279`  
		Last Modified: Tue, 25 Oct 2022 06:57:10 GMT  
		Size: 4.4 MB (4361351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33eb213c2d45440f6da62e4c97dcc2936c1a9881896421d53a86927e2618b29`  
		Last Modified: Tue, 25 Oct 2022 06:57:35 GMT  
		Size: 44.1 MB (44120965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77829c624efe1a2e9a13f40cb1d0c0f4d7fe497125dbf87d40699e87a907c260`  
		Last Modified: Tue, 25 Oct 2022 06:58:34 GMT  
		Size: 192.9 MB (192929475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:5670cbeec0868228f4cbe82cc9abb1f3c09d621ebbf85c7bf0369b24642df074
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.6 MB (285585964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f98764f075d571c93930c9fbb0965fe3cfd34f36ad2840deac11698e7d1b51d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:16:49 GMT
ADD file:2d01ff45e6105658cf6791d4ade5cc3168c7d455422fc973a54a795907023c4e in / 
# Wed, 05 Oct 2022 00:16:51 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:00:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:01:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 03:04:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:11:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:69c33ccbf3d1b09c78fae3f88deb756ae33a9e4610a01fc9ab8b457ee6107d7f`  
		Last Modified: Wed, 05 Oct 2022 00:35:11 GMT  
		Size: 25.6 MB (25618700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6742bf73589f8dd7c6c3ba8c0c07b6783a8c31c40b8e815941b550d904b49030`  
		Last Modified: Wed, 05 Oct 2022 03:54:22 GMT  
		Size: 5.9 MB (5938180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039b60e6247434b31a05dcae8802e410a92a3e9e6f9f6472455a58d4c1d5e1b6`  
		Last Modified: Wed, 05 Oct 2022 03:54:18 GMT  
		Size: 3.9 MB (3881311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde1ee2ce8c7376ef3e85ac490d31dcdf52bf954c3186472c53f3404c2421078`  
		Last Modified: Wed, 05 Oct 2022 03:56:41 GMT  
		Size: 42.8 MB (42832698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5e3cc23193e77d3695c7e56f6e60082abbcf0e11af954a30dda857279c355b`  
		Last Modified: Wed, 05 Oct 2022 04:03:57 GMT  
		Size: 207.3 MB (207315075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:10403bdb366987e6b3d1e90233130b79cd5e6931553eebe344edb75b787b74d6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.6 MB (228553552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e5108db95c124c6268c561f7f0b5c01f26b48f3801c253310534a9736f474fd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:31 GMT
ADD file:9c0c4172b14f0d37b0b074729a4738aeb165efe5c83e2d9bfefc5b39e4a4fe0b in / 
# Tue, 25 Oct 2022 01:23:32 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:44:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:44:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 02:44:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:46:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cf61a33f110308ce64c1dd7a5dddf2a5587ee1c8ab2351219b925428957cbc10`  
		Last Modified: Tue, 25 Oct 2022 01:25:01 GMT  
		Size: 26.0 MB (26022178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df11273ce2e4ff8fbfe44b4708e1c3b2323d38c23cc29bfb9935c1788807165`  
		Last Modified: Tue, 25 Oct 2022 02:53:37 GMT  
		Size: 6.5 MB (6473357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36f51f919c9bd6bce882afd5ce69c1de2f32276ae54369c26ae41702ff241ce`  
		Last Modified: Tue, 25 Oct 2022 02:53:35 GMT  
		Size: 3.6 MB (3625569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69ad44ec319ab50167d51a4bd01dd344bd736541842217bc94d0c6da1960b16c`  
		Last Modified: Tue, 25 Oct 2022 02:53:49 GMT  
		Size: 39.5 MB (39548002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed2d65b37ea7643db5c4a31a4261ef32fbaa397af4762b1b8e36a5f997c79998`  
		Last Modified: Tue, 25 Oct 2022 02:54:14 GMT  
		Size: 152.9 MB (152884446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.10-curl`

```console
$ docker pull buildpack-deps@sha256:d2ccc8013b79e84b3e20ef12b0baabd38c34272a9dbc9699d528528df2739163
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
$ docker pull buildpack-deps@sha256:2346451d88d35553f8bab367cb3a5e8de051d8da464fdcbf91e6030f07149fa2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37869572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb4b09635cfc10ef52385f01ae24c23a01d1531710e0aadd890ac70cde9de7c7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:28 GMT
ADD file:3384549425c94b92a7d7be15958e3ec7494bdf83242deb465d9059d4362d34d6 in / 
# Tue, 04 Oct 2022 23:35:28 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:13:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:13:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5887826a0d8b4c403d9bfaf57279fd8b585d272c3f450d374349365dc22cd8ef`  
		Last Modified: Tue, 04 Oct 2022 23:36:56 GMT  
		Size: 27.5 MB (27455077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b7fd9cb5adf6a195c3c2162caa409d926d4342598cad09f7fa4691e9ddd25f`  
		Last Modified: Wed, 05 Oct 2022 01:25:38 GMT  
		Size: 6.8 MB (6780586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9023f9ecbe71ceaba400cb934168d975ecabc157d85fe246f71d3d684947742d`  
		Last Modified: Wed, 05 Oct 2022 01:25:37 GMT  
		Size: 3.6 MB (3633909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:fff25ce4b7d7eb809d772ea4f8ad0b01880c3d7746627218ba716aacb733fd61
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.6 MB (35630586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1de0ca1a233d815d4617f6e298996b96f5857277214408cdde8ef90d1a4a38e0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:14:09 GMT
ADD file:4b538f2c7b46aa601d747159ce9e8c2c7a99b2b6e09e4efe1073ca58e47fbeed in / 
# Wed, 05 Oct 2022 00:14:09 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:47:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:47:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:788f7bb1e1d719f6a9a9b3b1530cc5bbe5b808a2ad77a65f23e2c6d15b8ae546`  
		Last Modified: Wed, 05 Oct 2022 00:16:28 GMT  
		Size: 25.9 MB (25873193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31aeed2022326b456329596b112851c2e027ba5773dab33fcd717efb1a016274`  
		Last Modified: Wed, 05 Oct 2022 01:01:56 GMT  
		Size: 6.0 MB (5955685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b8a4829745394c3402e5970b4558ef9fe23515f895e7f8a99fe24ae33a7c4f3`  
		Last Modified: Wed, 05 Oct 2022 01:01:55 GMT  
		Size: 3.8 MB (3801708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:373a282293140d34f364cb32917ccbfbb1b5657135e1d5b77becf7ec26d57437
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.9 MB (36886502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d0532ca7c686b7c5989d673e4c097b51d9fa7759a3b351e18ab993f11252e5d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:55:06 GMT
ADD file:30361063c284df6e20a85ff95b9c7b93648fe9e04ac935c9ff888e5c5f3af7ea in / 
# Tue, 25 Oct 2022 05:55:06 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:19:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:19:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:7a2e58a4bc1e52e3ab8904706a68a79146364ec32d8caf1bd106c3c9966a38fc`  
		Last Modified: Tue, 25 Oct 2022 05:56:30 GMT  
		Size: 26.7 MB (26676995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208c8913a9c66f64a1f5ca1349c8a8b9923f9eb9c8aed25bf3ec160a33e5a796`  
		Last Modified: Tue, 25 Oct 2022 08:36:03 GMT  
		Size: 6.6 MB (6607031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8491d7cc7a42af61771e26652e91532db813e380fa19339f7279420206df0290`  
		Last Modified: Tue, 25 Oct 2022 08:36:03 GMT  
		Size: 3.6 MB (3602476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:9144ea52e36fbf4e170dfe335aab6d5de9469737d3055aa70abfbed5e80d33fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44213298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9c8b0212d45ff3894e9e1dbc78bade496aa82a9c927fd6b5fd083714d2fa734`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:26:14 GMT
ADD file:60dd11bbfa9f1e2bc613c7f05cbbb83bca9e4b81550b6a0540a5d1d39f870cdd in / 
# Tue, 25 Oct 2022 03:26:16 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:40:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:40:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6d37bc653a986baef621c195bf8def80ca65133b8a3917bbd3a148b31bc1704f`  
		Last Modified: Tue, 25 Oct 2022 03:28:34 GMT  
		Size: 32.1 MB (32099941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc18decfda3085820c97e73c59dba18c534c4455c2eafc5812d29975ad7a9292`  
		Last Modified: Tue, 25 Oct 2022 06:57:12 GMT  
		Size: 7.8 MB (7752006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a931134d9aa21913f6400e3083b4c6955008f9fab7eae04019249a1d912c279`  
		Last Modified: Tue, 25 Oct 2022 06:57:10 GMT  
		Size: 4.4 MB (4361351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:4a2ac75c4ca1565140be2a5b2034effcf76de970fa53df98e47b6f6e7d58d3b5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.4 MB (35438191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b1442e7c0a8c0abe0dfc567219f3d6aa55e9adf597d425bff2605c64c8115bb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:16:49 GMT
ADD file:2d01ff45e6105658cf6791d4ade5cc3168c7d455422fc973a54a795907023c4e in / 
# Wed, 05 Oct 2022 00:16:51 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:00:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:01:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:69c33ccbf3d1b09c78fae3f88deb756ae33a9e4610a01fc9ab8b457ee6107d7f`  
		Last Modified: Wed, 05 Oct 2022 00:35:11 GMT  
		Size: 25.6 MB (25618700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6742bf73589f8dd7c6c3ba8c0c07b6783a8c31c40b8e815941b550d904b49030`  
		Last Modified: Wed, 05 Oct 2022 03:54:22 GMT  
		Size: 5.9 MB (5938180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039b60e6247434b31a05dcae8802e410a92a3e9e6f9f6472455a58d4c1d5e1b6`  
		Last Modified: Wed, 05 Oct 2022 03:54:18 GMT  
		Size: 3.9 MB (3881311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:75ab25d6d67c72f804bc2ecca53130abb5963b93b91371b24be4f8ab90b4b54a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.1 MB (36121104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:644ada4f863420e616b970ac64e228a95ba0993dfbee2c4fb59ad86e50b0566e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:31 GMT
ADD file:9c0c4172b14f0d37b0b074729a4738aeb165efe5c83e2d9bfefc5b39e4a4fe0b in / 
# Tue, 25 Oct 2022 01:23:32 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:44:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:44:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:cf61a33f110308ce64c1dd7a5dddf2a5587ee1c8ab2351219b925428957cbc10`  
		Last Modified: Tue, 25 Oct 2022 01:25:01 GMT  
		Size: 26.0 MB (26022178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df11273ce2e4ff8fbfe44b4708e1c3b2323d38c23cc29bfb9935c1788807165`  
		Last Modified: Tue, 25 Oct 2022 02:53:37 GMT  
		Size: 6.5 MB (6473357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36f51f919c9bd6bce882afd5ce69c1de2f32276ae54369c26ae41702ff241ce`  
		Last Modified: Tue, 25 Oct 2022 02:53:35 GMT  
		Size: 3.6 MB (3625569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.10-scm`

```console
$ docker pull buildpack-deps@sha256:044006a56118d10d105fef337fa49803641ab52652693b35a7a4b6a22555ef48
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
$ docker pull buildpack-deps@sha256:d04920e171fddca160ba2431b2421bf49b424767a2a15f5be91bb9d94f21bb2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.6 MB (77583500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64ef1de29f63807a6093e6af698173335a81692ab641a3e02e63bc9df42ea5f9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:28 GMT
ADD file:3384549425c94b92a7d7be15958e3ec7494bdf83242deb465d9059d4362d34d6 in / 
# Tue, 04 Oct 2022 23:35:28 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:13:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:13:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:14:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5887826a0d8b4c403d9bfaf57279fd8b585d272c3f450d374349365dc22cd8ef`  
		Last Modified: Tue, 04 Oct 2022 23:36:56 GMT  
		Size: 27.5 MB (27455077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b7fd9cb5adf6a195c3c2162caa409d926d4342598cad09f7fa4691e9ddd25f`  
		Last Modified: Wed, 05 Oct 2022 01:25:38 GMT  
		Size: 6.8 MB (6780586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9023f9ecbe71ceaba400cb934168d975ecabc157d85fe246f71d3d684947742d`  
		Last Modified: Wed, 05 Oct 2022 01:25:37 GMT  
		Size: 3.6 MB (3633909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d44eedd822ec1ffd1b32f87638bae3694f27cf99e85f8d3d8f6d1f2857fdc1`  
		Last Modified: Wed, 05 Oct 2022 01:25:54 GMT  
		Size: 39.7 MB (39713928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:2965cc2f6b4e99430ed3e5dc6e19cff61861fd39ce9247198d0446c4ea18da12
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.2 MB (78226975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf87da53eb6a1926ffac398aa2b41ffc1c7ba4e19fa01b0c1e132a9fcfa6d7ad`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:14:09 GMT
ADD file:4b538f2c7b46aa601d747159ce9e8c2c7a99b2b6e09e4efe1073ca58e47fbeed in / 
# Wed, 05 Oct 2022 00:14:09 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:47:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:47:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:48:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:788f7bb1e1d719f6a9a9b3b1530cc5bbe5b808a2ad77a65f23e2c6d15b8ae546`  
		Last Modified: Wed, 05 Oct 2022 00:16:28 GMT  
		Size: 25.9 MB (25873193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31aeed2022326b456329596b112851c2e027ba5773dab33fcd717efb1a016274`  
		Last Modified: Wed, 05 Oct 2022 01:01:56 GMT  
		Size: 6.0 MB (5955685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b8a4829745394c3402e5970b4558ef9fe23515f895e7f8a99fe24ae33a7c4f3`  
		Last Modified: Wed, 05 Oct 2022 01:01:55 GMT  
		Size: 3.8 MB (3801708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199fb45c30ad58843e78384afd22f7dec65ac55a285086da2083dea2426fd37e`  
		Last Modified: Wed, 05 Oct 2022 01:02:19 GMT  
		Size: 42.6 MB (42596389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f9e6c255feb050995c15d584bed8b4ef31d7171ecc8f79741ce561d7ab013ce5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.4 MB (76373070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2e46d98faf0c177cab0e52968d9d062a3a4f181d3c42f5759c5eb9615ccd5b8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:55:06 GMT
ADD file:30361063c284df6e20a85ff95b9c7b93648fe9e04ac935c9ff888e5c5f3af7ea in / 
# Tue, 25 Oct 2022 05:55:06 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:19:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:19:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:20:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a2e58a4bc1e52e3ab8904706a68a79146364ec32d8caf1bd106c3c9966a38fc`  
		Last Modified: Tue, 25 Oct 2022 05:56:30 GMT  
		Size: 26.7 MB (26676995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208c8913a9c66f64a1f5ca1349c8a8b9923f9eb9c8aed25bf3ec160a33e5a796`  
		Last Modified: Tue, 25 Oct 2022 08:36:03 GMT  
		Size: 6.6 MB (6607031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8491d7cc7a42af61771e26652e91532db813e380fa19339f7279420206df0290`  
		Last Modified: Tue, 25 Oct 2022 08:36:03 GMT  
		Size: 3.6 MB (3602476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2cf60ff33717c4a17f0ca2f77473b69d8d357e4dc81ef8bb8a5e24382aa106`  
		Last Modified: Tue, 25 Oct 2022 08:36:17 GMT  
		Size: 39.5 MB (39486568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:ce93a24cd078d6b8c4f5f7301e8e03082dc0b280b7699a23b4a638e67ae2efdb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.3 MB (88334263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b98ffc392030e610f3af3f6119e1fda61df1f4b3d9ae0d893603fbbc1949cfc0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:26:14 GMT
ADD file:60dd11bbfa9f1e2bc613c7f05cbbb83bca9e4b81550b6a0540a5d1d39f870cdd in / 
# Tue, 25 Oct 2022 03:26:16 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:40:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:40:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:41:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6d37bc653a986baef621c195bf8def80ca65133b8a3917bbd3a148b31bc1704f`  
		Last Modified: Tue, 25 Oct 2022 03:28:34 GMT  
		Size: 32.1 MB (32099941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc18decfda3085820c97e73c59dba18c534c4455c2eafc5812d29975ad7a9292`  
		Last Modified: Tue, 25 Oct 2022 06:57:12 GMT  
		Size: 7.8 MB (7752006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a931134d9aa21913f6400e3083b4c6955008f9fab7eae04019249a1d912c279`  
		Last Modified: Tue, 25 Oct 2022 06:57:10 GMT  
		Size: 4.4 MB (4361351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33eb213c2d45440f6da62e4c97dcc2936c1a9881896421d53a86927e2618b29`  
		Last Modified: Tue, 25 Oct 2022 06:57:35 GMT  
		Size: 44.1 MB (44120965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:ab238169f3b08dc7c08c8e3ed46e6ad74014ba89c7d7d398a9038687df3104a5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78270889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bec2b637df9811eabf5c8c05afc79681031c55e2b577567a231be07852233f7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:16:49 GMT
ADD file:2d01ff45e6105658cf6791d4ade5cc3168c7d455422fc973a54a795907023c4e in / 
# Wed, 05 Oct 2022 00:16:51 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:00:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:01:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 03:04:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:69c33ccbf3d1b09c78fae3f88deb756ae33a9e4610a01fc9ab8b457ee6107d7f`  
		Last Modified: Wed, 05 Oct 2022 00:35:11 GMT  
		Size: 25.6 MB (25618700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6742bf73589f8dd7c6c3ba8c0c07b6783a8c31c40b8e815941b550d904b49030`  
		Last Modified: Wed, 05 Oct 2022 03:54:22 GMT  
		Size: 5.9 MB (5938180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039b60e6247434b31a05dcae8802e410a92a3e9e6f9f6472455a58d4c1d5e1b6`  
		Last Modified: Wed, 05 Oct 2022 03:54:18 GMT  
		Size: 3.9 MB (3881311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde1ee2ce8c7376ef3e85ac490d31dcdf52bf954c3186472c53f3404c2421078`  
		Last Modified: Wed, 05 Oct 2022 03:56:41 GMT  
		Size: 42.8 MB (42832698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:ca6937235c92176f4e66e5e83e654d8ac06099c69d6cdd2917dca4640643463c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75669106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15939ebf9f49b3608111d36fac9b9adb1584829b3dcfba4701e71c081de209c0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:31 GMT
ADD file:9c0c4172b14f0d37b0b074729a4738aeb165efe5c83e2d9bfefc5b39e4a4fe0b in / 
# Tue, 25 Oct 2022 01:23:32 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:44:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:44:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 02:44:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cf61a33f110308ce64c1dd7a5dddf2a5587ee1c8ab2351219b925428957cbc10`  
		Last Modified: Tue, 25 Oct 2022 01:25:01 GMT  
		Size: 26.0 MB (26022178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df11273ce2e4ff8fbfe44b4708e1c3b2323d38c23cc29bfb9935c1788807165`  
		Last Modified: Tue, 25 Oct 2022 02:53:37 GMT  
		Size: 6.5 MB (6473357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36f51f919c9bd6bce882afd5ce69c1de2f32276ae54369c26ae41702ff241ce`  
		Last Modified: Tue, 25 Oct 2022 02:53:35 GMT  
		Size: 3.6 MB (3625569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69ad44ec319ab50167d51a4bd01dd344bd736541842217bc94d0c6da1960b16c`  
		Last Modified: Tue, 25 Oct 2022 02:53:49 GMT  
		Size: 39.5 MB (39548002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bionic`

```console
$ docker pull buildpack-deps@sha256:9fd1bd60ef4fb6123e4e4c8874cac211e0d563dad6b188f64574e33eed1094bc
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
$ docker pull buildpack-deps@sha256:8e193981b35a706985cdc98b60c03e5542e213ee488587b2d9958940c84561d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.4 MB (221393894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2608fa2156d0a642f6ac431b67743a605276f1e936f72ecc653a3da10b792ea4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:04 GMT
ADD file:ed601c56cf74241eeb1971b24ed969fb855cd2b9330276d3c5779ecdb0b28364 in / 
# Tue, 04 Oct 2022 23:35:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:00:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:00:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:01:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:04:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e706e0a9f42365312b366bf4caa22f3cdd8fc7fd8f6f49b4dd3782711f66aca7`  
		Last Modified: Tue, 04 Oct 2022 11:37:26 GMT  
		Size: 26.7 MB (26711852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14bb308d0caa16e5231c4d889948a8b0c06b9e2c461919c74887b27e349d490`  
		Last Modified: Wed, 05 Oct 2022 01:22:33 GMT  
		Size: 6.6 MB (6631019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd853d7120feb9f81650bf7bc95fac3a301e6f7fb667e27ff0c44f05fc3bd84`  
		Last Modified: Wed, 05 Oct 2022 01:22:33 GMT  
		Size: 3.0 MB (3023747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e261a80722021da4732449560d09c9be0f3a45bc7cd83a11ec75216c88d19d8`  
		Last Modified: Wed, 05 Oct 2022 01:22:50 GMT  
		Size: 45.5 MB (45498303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f4264228ed8e7647983ec917c22f259b84a520ddaee10cd3d968f9c68bff1ac`  
		Last Modified: Wed, 05 Oct 2022 01:23:19 GMT  
		Size: 139.5 MB (139528973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:8c42ce93b617d12c423261ac5d8a9b5949385d3ee604c85ab12add1f2354b260
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.6 MB (189554619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fd4e33dc0507b376b73e9f97cafb185f57745359d69c95771a51290fe3c978a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:31 GMT
ADD file:20e0d71059d38b1e18636b9db71f534d7297c3f571d73d45a75b4b8d3cac86c7 in / 
# Wed, 05 Oct 2022 00:13:32 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:40:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:40:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:41:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:42:24 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:91bb9a9844d67fd31f07ebd74dc8a4f4f18e2f959d3aa2166aca86ae57f353c6`  
		Last Modified: Wed, 05 Oct 2022 00:15:26 GMT  
		Size: 22.3 MB (22305721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5da5c18a3ec9c91b23737d7223b602b070f7de605771c25aadd8092545e561`  
		Last Modified: Wed, 05 Oct 2022 00:57:59 GMT  
		Size: 5.7 MB (5697196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327d003e6583d861f4c3df07410a51c18c3b7f4a0649fbfde6aab1ec77b4b110`  
		Last Modified: Wed, 05 Oct 2022 00:57:58 GMT  
		Size: 2.6 MB (2585088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdc6a2f528031e62d90580aa8ccad6d2351f1de9a49f1ebeed4945a07ffeed3`  
		Last Modified: Wed, 05 Oct 2022 00:58:23 GMT  
		Size: 40.7 MB (40690856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dbc06c808278c578a9ebcf12b02c2e632f8eb0c39fa50538a9faf7483bd4953`  
		Last Modified: Wed, 05 Oct 2022 00:59:02 GMT  
		Size: 118.3 MB (118275758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3e79fc3dd3b14b9bb575350832102635634b50d09fc0e17787f8ab9461363820
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.0 MB (205988599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:307ed33f4f8918cc97443f064b1a80b4169652a8a5830856adc59899d807e672`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:56 GMT
ADD file:585011162da73734395f2ef251ad89b72cfed0101c7da2435fac55061f99b516 in / 
# Tue, 25 Oct 2022 05:54:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:03:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:04:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:04:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:08:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a217cb16e35b382d60a7ab454a8c4db0fbe5e0aeec4b4c346e51eb1e77d34f8c`  
		Last Modified: Tue, 25 Oct 2022 05:55:45 GMT  
		Size: 23.7 MB (23735856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296237f400b08de0ee2566d1d70f0c0fa8e7334ec80823903e2aaf4904c5a49d`  
		Last Modified: Tue, 25 Oct 2022 08:33:20 GMT  
		Size: 6.1 MB (6074795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82de00773434d5186afe917dba4d4a8e731ffb220b4b8b348628c4df9f9e773e`  
		Last Modified: Tue, 25 Oct 2022 08:33:20 GMT  
		Size: 2.8 MB (2790789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ead073af2bd060ee0645628a8ca9a37e4f01b5c89e089690cff894da4eb30b`  
		Last Modified: Tue, 25 Oct 2022 08:33:34 GMT  
		Size: 43.3 MB (43296375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ac6f110046b149cfabf2ddff78dd4a130eeac7523196ddbe458ecf807d0656`  
		Last Modified: Tue, 25 Oct 2022 08:34:01 GMT  
		Size: 130.1 MB (130090784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; 386

```console
$ docker pull buildpack-deps@sha256:88842772446e48882fcdf20872ab09cd43f8fcb75681fa5f61b926dc8644445f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.2 MB (218240056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0daef8c85d992fa89d4cc85af6ebe982b049919dd5c9fd4465b81a65a9cd2bd9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:34:56 GMT
ADD file:40406c12653f21504e334fcfb19c00ee9eed94dbaa2eb7c7bfdb293677697aa6 in / 
# Tue, 25 Oct 2022 02:34:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:20:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:21:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 05:21:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:24:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1beb66ce54f29e44b5005bf3e2d004424176aa3361ee8e602a9ae10a8ee447cf`  
		Last Modified: Tue, 25 Oct 2022 02:35:33 GMT  
		Size: 27.2 MB (27166059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196f1fa30db3bbf53093b5c7d1d2add129bf1974ce53a6e094f0f0795c7881e7`  
		Last Modified: Tue, 25 Oct 2022 05:31:10 GMT  
		Size: 6.9 MB (6921884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f025677e2376712e8fb9824f1fcfefa2d3005ebe8cebe43324e65b6d2f3a106`  
		Last Modified: Tue, 25 Oct 2022 05:31:09 GMT  
		Size: 3.0 MB (3042023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5439394181cf9e8ac2e0b446f62199582c04aa5f5903de80e9b8474a01ca5c24`  
		Last Modified: Tue, 25 Oct 2022 05:31:28 GMT  
		Size: 47.1 MB (47083490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb1497899c9f48cc0c773769e863fb5f587546a5831104b7ee048453a776aebe`  
		Last Modified: Tue, 25 Oct 2022 05:31:56 GMT  
		Size: 134.0 MB (134026600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:443a00cd3f35125ff2856e16c19720e7963f64acd7ca5955fed24d8763ebaffa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.4 MB (246426888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70f27d2f9478275b6a5a2a4b9587a5ceea77a4af2af4a05be63e9ee1adb3ce8d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:34 GMT
ADD file:254e11be9bc865d645aba7c16a39a04f5ce227b7aa4280f7a42baec47b0c6ee0 in / 
# Tue, 25 Oct 2022 03:25:36 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:20:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:21:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:22:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:27:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:21b8f46bc1957ff60412d81678134500cf7a4f0e7f198ba384fedb2e5747d847`  
		Last Modified: Tue, 25 Oct 2022 03:27:21 GMT  
		Size: 30.4 MB (30443225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7a73c0177bc0907d9770e0863fb7f6949a870d385b401421a0817a32cd56be`  
		Last Modified: Tue, 25 Oct 2022 06:52:33 GMT  
		Size: 7.1 MB (7051025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f82d4b01549cae8ea6c3b7e9f210d370b148dd8004af19925715e43994e9ff`  
		Last Modified: Tue, 25 Oct 2022 06:52:32 GMT  
		Size: 3.7 MB (3740646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc5edd6bb0a218e937aacff2efa004bac7b35909a1d19740f14acbae1df7b87`  
		Last Modified: Tue, 25 Oct 2022 06:52:59 GMT  
		Size: 53.7 MB (53741147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600501f491d899f441f91702b04e48dda009fb613806254ab578645e5cc0307f`  
		Last Modified: Tue, 25 Oct 2022 06:53:48 GMT  
		Size: 151.5 MB (151450845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:16eceed169fc7d8e7dd3f213936244ab45f5e6ec0e5090ecd3f9a8f04e0f9e4c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.8 MB (205759274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ab91687893f8d5e47036caf530ff156ea86a4d93a7b61bf9ad5037e833453cf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:02 GMT
ADD file:0843e89b8865a30626cece7a42cf27708a86422aadb28029168b2f159a8768fa in / 
# Tue, 25 Oct 2022 01:23:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:34:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:34:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 02:35:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:37:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4cd692a206d359f66e10c4f4f2a37009c4162f022df78a9bb8e8c24def290167`  
		Last Modified: Tue, 25 Oct 2022 01:24:23 GMT  
		Size: 25.4 MB (25371461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1872edbfc35ad376faca8b8da8bfdde0ac95f27652b1188c2036672466ab8233`  
		Last Modified: Tue, 25 Oct 2022 02:51:21 GMT  
		Size: 6.3 MB (6326364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5dda90dab707bb33111b66abdc094ed182c70b7a83b6844b6b316ba93a0f779`  
		Last Modified: Tue, 25 Oct 2022 02:51:21 GMT  
		Size: 3.0 MB (2976628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feacbe49c2940d688c7c8200c29c610e8a5a65180c8b6d67c78b193f408418a7`  
		Last Modified: Tue, 25 Oct 2022 02:51:34 GMT  
		Size: 45.0 MB (45044933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74da665a3988b61dbc1e55c52dc97c4d3fcf3b2c58feb3f9664d6b471d420d91`  
		Last Modified: Tue, 25 Oct 2022 02:51:56 GMT  
		Size: 126.0 MB (126039888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bionic-curl`

```console
$ docker pull buildpack-deps@sha256:437c0a65f1a0597bc2aea93d7ed8c38b6209d7768299cb9af858a074be32277e
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
$ docker pull buildpack-deps@sha256:c4539563e222d7175a071977335bfbb5a52887b403295e6bede505e11a183e63
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36366618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b86072004a7e51f50a4f9308592351b5df03fbcf3569269d2aded7b6d06f5141`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:04 GMT
ADD file:ed601c56cf74241eeb1971b24ed969fb855cd2b9330276d3c5779ecdb0b28364 in / 
# Tue, 04 Oct 2022 23:35:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:00:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:00:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e706e0a9f42365312b366bf4caa22f3cdd8fc7fd8f6f49b4dd3782711f66aca7`  
		Last Modified: Tue, 04 Oct 2022 11:37:26 GMT  
		Size: 26.7 MB (26711852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14bb308d0caa16e5231c4d889948a8b0c06b9e2c461919c74887b27e349d490`  
		Last Modified: Wed, 05 Oct 2022 01:22:33 GMT  
		Size: 6.6 MB (6631019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd853d7120feb9f81650bf7bc95fac3a301e6f7fb667e27ff0c44f05fc3bd84`  
		Last Modified: Wed, 05 Oct 2022 01:22:33 GMT  
		Size: 3.0 MB (3023747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:64eb7b3da5d316eb2ccb73ac59d267a9e931c6a22c3ccfb92ca219eac156b3e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30588005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faa01cb702a2d7c8668373897fe036b5e3a9734a7731883f831ee6232ef49e5d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:31 GMT
ADD file:20e0d71059d38b1e18636b9db71f534d7297c3f571d73d45a75b4b8d3cac86c7 in / 
# Wed, 05 Oct 2022 00:13:32 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:40:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:40:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:91bb9a9844d67fd31f07ebd74dc8a4f4f18e2f959d3aa2166aca86ae57f353c6`  
		Last Modified: Wed, 05 Oct 2022 00:15:26 GMT  
		Size: 22.3 MB (22305721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5da5c18a3ec9c91b23737d7223b602b070f7de605771c25aadd8092545e561`  
		Last Modified: Wed, 05 Oct 2022 00:57:59 GMT  
		Size: 5.7 MB (5697196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327d003e6583d861f4c3df07410a51c18c3b7f4a0649fbfde6aab1ec77b4b110`  
		Last Modified: Wed, 05 Oct 2022 00:57:58 GMT  
		Size: 2.6 MB (2585088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:4a7fb4ce2c117e99998cdeef7a19e67cc71055fe3a3e73e8aa9c33ffb9c67d3b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.6 MB (32601440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ed643d0aed22b28551913f89b4c72639e5b8faaae70ba0f4501439d38584433`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:56 GMT
ADD file:585011162da73734395f2ef251ad89b72cfed0101c7da2435fac55061f99b516 in / 
# Tue, 25 Oct 2022 05:54:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:03:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:04:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a217cb16e35b382d60a7ab454a8c4db0fbe5e0aeec4b4c346e51eb1e77d34f8c`  
		Last Modified: Tue, 25 Oct 2022 05:55:45 GMT  
		Size: 23.7 MB (23735856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296237f400b08de0ee2566d1d70f0c0fa8e7334ec80823903e2aaf4904c5a49d`  
		Last Modified: Tue, 25 Oct 2022 08:33:20 GMT  
		Size: 6.1 MB (6074795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82de00773434d5186afe917dba4d4a8e731ffb220b4b8b348628c4df9f9e773e`  
		Last Modified: Tue, 25 Oct 2022 08:33:20 GMT  
		Size: 2.8 MB (2790789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:f9d7810c1b79a2b1c2979e85b4ec6d5fcc001703c2e12449627f1aad25218640
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37129966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dda5cb77527fbe9d18b28b41ea7c3b6c7ae3fd43336a9b9cbf26b6f9e7194841`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:34:56 GMT
ADD file:40406c12653f21504e334fcfb19c00ee9eed94dbaa2eb7c7bfdb293677697aa6 in / 
# Tue, 25 Oct 2022 02:34:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:20:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:21:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1beb66ce54f29e44b5005bf3e2d004424176aa3361ee8e602a9ae10a8ee447cf`  
		Last Modified: Tue, 25 Oct 2022 02:35:33 GMT  
		Size: 27.2 MB (27166059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196f1fa30db3bbf53093b5c7d1d2add129bf1974ce53a6e094f0f0795c7881e7`  
		Last Modified: Tue, 25 Oct 2022 05:31:10 GMT  
		Size: 6.9 MB (6921884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f025677e2376712e8fb9824f1fcfefa2d3005ebe8cebe43324e65b6d2f3a106`  
		Last Modified: Tue, 25 Oct 2022 05:31:09 GMT  
		Size: 3.0 MB (3042023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:45c832bf6c3088da7c40d8e5205cdf1f8357326d9ad8840ddc61343237447345
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41234896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a774524b743b63f11381672077399dd0cdf35bb59695140dc3f5f7e3b3f523b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:34 GMT
ADD file:254e11be9bc865d645aba7c16a39a04f5ce227b7aa4280f7a42baec47b0c6ee0 in / 
# Tue, 25 Oct 2022 03:25:36 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:20:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:21:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:21b8f46bc1957ff60412d81678134500cf7a4f0e7f198ba384fedb2e5747d847`  
		Last Modified: Tue, 25 Oct 2022 03:27:21 GMT  
		Size: 30.4 MB (30443225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7a73c0177bc0907d9770e0863fb7f6949a870d385b401421a0817a32cd56be`  
		Last Modified: Tue, 25 Oct 2022 06:52:33 GMT  
		Size: 7.1 MB (7051025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f82d4b01549cae8ea6c3b7e9f210d370b148dd8004af19925715e43994e9ff`  
		Last Modified: Tue, 25 Oct 2022 06:52:32 GMT  
		Size: 3.7 MB (3740646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:171c50890d275551e068fbc231b063d10c68d4f76bb5c113b55893fd0c094898
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34674453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23932295597dc4628240979d04d45ef0bac7ff6e5a0e864ddec4d112b2aa2143`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:02 GMT
ADD file:0843e89b8865a30626cece7a42cf27708a86422aadb28029168b2f159a8768fa in / 
# Tue, 25 Oct 2022 01:23:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:34:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:34:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4cd692a206d359f66e10c4f4f2a37009c4162f022df78a9bb8e8c24def290167`  
		Last Modified: Tue, 25 Oct 2022 01:24:23 GMT  
		Size: 25.4 MB (25371461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1872edbfc35ad376faca8b8da8bfdde0ac95f27652b1188c2036672466ab8233`  
		Last Modified: Tue, 25 Oct 2022 02:51:21 GMT  
		Size: 6.3 MB (6326364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5dda90dab707bb33111b66abdc094ed182c70b7a83b6844b6b316ba93a0f779`  
		Last Modified: Tue, 25 Oct 2022 02:51:21 GMT  
		Size: 3.0 MB (2976628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bionic-scm`

```console
$ docker pull buildpack-deps@sha256:2cd1279307ba80edb1d4d0d882abbb11aab1d95d217ad147971be1e53f48d7df
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
$ docker pull buildpack-deps@sha256:2185d9b019c2c7ffa24811155449345078f4adb96a6b771140d25fa96128e80d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81864921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e18c1737a8adb0820fe73beb358791cbde70dc5a532a61b2fa74b072d928cca6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:04 GMT
ADD file:ed601c56cf74241eeb1971b24ed969fb855cd2b9330276d3c5779ecdb0b28364 in / 
# Tue, 04 Oct 2022 23:35:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:00:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:00:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:01:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e706e0a9f42365312b366bf4caa22f3cdd8fc7fd8f6f49b4dd3782711f66aca7`  
		Last Modified: Tue, 04 Oct 2022 11:37:26 GMT  
		Size: 26.7 MB (26711852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14bb308d0caa16e5231c4d889948a8b0c06b9e2c461919c74887b27e349d490`  
		Last Modified: Wed, 05 Oct 2022 01:22:33 GMT  
		Size: 6.6 MB (6631019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd853d7120feb9f81650bf7bc95fac3a301e6f7fb667e27ff0c44f05fc3bd84`  
		Last Modified: Wed, 05 Oct 2022 01:22:33 GMT  
		Size: 3.0 MB (3023747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e261a80722021da4732449560d09c9be0f3a45bc7cd83a11ec75216c88d19d8`  
		Last Modified: Wed, 05 Oct 2022 01:22:50 GMT  
		Size: 45.5 MB (45498303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:c135384e7b3dd71613cf28fbeb9805b51ae11140898b2d9034275ce1c7c77988
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71278861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d25e3b88b9f8e85d32a18eda77ceaf66170755d464f812b3b79a2aeb16210730`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:31 GMT
ADD file:20e0d71059d38b1e18636b9db71f534d7297c3f571d73d45a75b4b8d3cac86c7 in / 
# Wed, 05 Oct 2022 00:13:32 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:40:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:40:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:41:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:91bb9a9844d67fd31f07ebd74dc8a4f4f18e2f959d3aa2166aca86ae57f353c6`  
		Last Modified: Wed, 05 Oct 2022 00:15:26 GMT  
		Size: 22.3 MB (22305721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5da5c18a3ec9c91b23737d7223b602b070f7de605771c25aadd8092545e561`  
		Last Modified: Wed, 05 Oct 2022 00:57:59 GMT  
		Size: 5.7 MB (5697196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327d003e6583d861f4c3df07410a51c18c3b7f4a0649fbfde6aab1ec77b4b110`  
		Last Modified: Wed, 05 Oct 2022 00:57:58 GMT  
		Size: 2.6 MB (2585088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdc6a2f528031e62d90580aa8ccad6d2351f1de9a49f1ebeed4945a07ffeed3`  
		Last Modified: Wed, 05 Oct 2022 00:58:23 GMT  
		Size: 40.7 MB (40690856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:831b524d20f9c5814aac27758c344b403757f5ab45060243817b13a2c40102e6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75897815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e470c3c6917737866b9756535cfe361c65e8808582d7c42f618ac621feedca3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:56 GMT
ADD file:585011162da73734395f2ef251ad89b72cfed0101c7da2435fac55061f99b516 in / 
# Tue, 25 Oct 2022 05:54:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:03:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:04:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:04:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a217cb16e35b382d60a7ab454a8c4db0fbe5e0aeec4b4c346e51eb1e77d34f8c`  
		Last Modified: Tue, 25 Oct 2022 05:55:45 GMT  
		Size: 23.7 MB (23735856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296237f400b08de0ee2566d1d70f0c0fa8e7334ec80823903e2aaf4904c5a49d`  
		Last Modified: Tue, 25 Oct 2022 08:33:20 GMT  
		Size: 6.1 MB (6074795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82de00773434d5186afe917dba4d4a8e731ffb220b4b8b348628c4df9f9e773e`  
		Last Modified: Tue, 25 Oct 2022 08:33:20 GMT  
		Size: 2.8 MB (2790789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ead073af2bd060ee0645628a8ca9a37e4f01b5c89e089690cff894da4eb30b`  
		Last Modified: Tue, 25 Oct 2022 08:33:34 GMT  
		Size: 43.3 MB (43296375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:83df231eb79f3c19636d63aa33a16412557b58c3d612af24a8992bf30c0bf2bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.2 MB (84213456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a9bbfb87a10a33a893bf414b33e9b8b13d1a1613ff530d2f7f475add897a53d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:34:56 GMT
ADD file:40406c12653f21504e334fcfb19c00ee9eed94dbaa2eb7c7bfdb293677697aa6 in / 
# Tue, 25 Oct 2022 02:34:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:20:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:21:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 05:21:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1beb66ce54f29e44b5005bf3e2d004424176aa3361ee8e602a9ae10a8ee447cf`  
		Last Modified: Tue, 25 Oct 2022 02:35:33 GMT  
		Size: 27.2 MB (27166059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196f1fa30db3bbf53093b5c7d1d2add129bf1974ce53a6e094f0f0795c7881e7`  
		Last Modified: Tue, 25 Oct 2022 05:31:10 GMT  
		Size: 6.9 MB (6921884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f025677e2376712e8fb9824f1fcfefa2d3005ebe8cebe43324e65b6d2f3a106`  
		Last Modified: Tue, 25 Oct 2022 05:31:09 GMT  
		Size: 3.0 MB (3042023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5439394181cf9e8ac2e0b446f62199582c04aa5f5903de80e9b8474a01ca5c24`  
		Last Modified: Tue, 25 Oct 2022 05:31:28 GMT  
		Size: 47.1 MB (47083490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:9b3b087f55c1efa8493ec4b43697807a5c2d17ed20ae7d7d9be3b0c0059e5780
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.0 MB (94976043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:799cb2cdce8facd27fc40f8e46c9d7af5acfdb40bc0350b08603cb8ef204716f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:34 GMT
ADD file:254e11be9bc865d645aba7c16a39a04f5ce227b7aa4280f7a42baec47b0c6ee0 in / 
# Tue, 25 Oct 2022 03:25:36 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:20:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:21:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:22:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:21b8f46bc1957ff60412d81678134500cf7a4f0e7f198ba384fedb2e5747d847`  
		Last Modified: Tue, 25 Oct 2022 03:27:21 GMT  
		Size: 30.4 MB (30443225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7a73c0177bc0907d9770e0863fb7f6949a870d385b401421a0817a32cd56be`  
		Last Modified: Tue, 25 Oct 2022 06:52:33 GMT  
		Size: 7.1 MB (7051025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f82d4b01549cae8ea6c3b7e9f210d370b148dd8004af19925715e43994e9ff`  
		Last Modified: Tue, 25 Oct 2022 06:52:32 GMT  
		Size: 3.7 MB (3740646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc5edd6bb0a218e937aacff2efa004bac7b35909a1d19740f14acbae1df7b87`  
		Last Modified: Tue, 25 Oct 2022 06:52:59 GMT  
		Size: 53.7 MB (53741147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a1f61989c50474fceff25499a47ac25dcaa6159237d67e49479a11f64bf78697
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79719386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66335b8c0d2152b8e22f15bb354ebf842a232eb17f087314607606c364ab9d5d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:02 GMT
ADD file:0843e89b8865a30626cece7a42cf27708a86422aadb28029168b2f159a8768fa in / 
# Tue, 25 Oct 2022 01:23:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:34:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:34:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 02:35:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4cd692a206d359f66e10c4f4f2a37009c4162f022df78a9bb8e8c24def290167`  
		Last Modified: Tue, 25 Oct 2022 01:24:23 GMT  
		Size: 25.4 MB (25371461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1872edbfc35ad376faca8b8da8bfdde0ac95f27652b1188c2036672466ab8233`  
		Last Modified: Tue, 25 Oct 2022 02:51:21 GMT  
		Size: 6.3 MB (6326364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5dda90dab707bb33111b66abdc094ed182c70b7a83b6844b6b316ba93a0f779`  
		Last Modified: Tue, 25 Oct 2022 02:51:21 GMT  
		Size: 3.0 MB (2976628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feacbe49c2940d688c7c8200c29c610e8a5a65180c8b6d67c78b193f408418a7`  
		Last Modified: Tue, 25 Oct 2022 02:51:34 GMT  
		Size: 45.0 MB (45044933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bookworm`

```console
$ docker pull buildpack-deps@sha256:2b1077fc56cdca828f6c4f2fa98e5d65c4b046f877a626cca060199cb08b551e
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
$ docker pull buildpack-deps@sha256:d02593a621ee4f4e7e1fcf39298988b2d0ed222e1d591c59c1d473821d34b6f0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.9 MB (344906770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f0c0cbc5ed6d6e7cc27ef5c4f8b20fdb7085d85320252f8db1c8f63fc75f111`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:03 GMT
ADD file:ca5a5911d0951e5c75f1790eb644a6fd41dcb9712fa2af0fb6d3a537a72e6ad8 in / 
# Tue, 04 Oct 2022 23:26:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:52:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:52:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:52:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:54:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6674a3ae4f8f54c2f747bad2069e50ce00e352d650887729310d984cebecea22`  
		Last Modified: Tue, 04 Oct 2022 23:29:50 GMT  
		Size: 53.0 MB (52962415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e064222ce493e48ae4ceac8f18316e08d2afb963ad57bd63b8630a0ae009f8`  
		Last Modified: Wed, 05 Oct 2022 01:18:07 GMT  
		Size: 9.3 MB (9298646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab229472e3a483409ce2bbc4d461fc6512c03c687daf6546b52705bc7f18961`  
		Last Modified: Wed, 05 Oct 2022 01:18:08 GMT  
		Size: 11.4 MB (11381655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93a5a87ebbd4472db252972521c82b5789bcc45b6bf1ff4d5e59ab129a4847a`  
		Last Modified: Wed, 05 Oct 2022 01:18:25 GMT  
		Size: 57.2 MB (57201277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:685ee8ce50d5fd303a9b0b6cb4cdf889b35afe78677a8c5006983f396b8fca18`  
		Last Modified: Wed, 05 Oct 2022 01:19:02 GMT  
		Size: 214.1 MB (214062777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:d7f420e4177af2c9b91b120ebe9e979d0dcad3966763acb1ed21525041e635fe
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.9 MB (309899153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9046c47430ebdd5f5d55eed0c00fd443d2e16476c60f2500fb777b7b45a350e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:05:47 GMT
ADD file:226ff5e5e8066a03822e2865c6f72c554de94710c5664ee8bebd127d8aa32388 in / 
# Tue, 25 Oct 2022 03:05:48 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:08:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:08:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:09:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:11:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cff7bd795d206b13b585de0da179a0c9616a5278eb7d74a97c97746085567403`  
		Last Modified: Tue, 25 Oct 2022 03:10:30 GMT  
		Size: 50.2 MB (50178371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40202823259eac4be0260092f1fb5f25fa9d866c32ec384dcadb0c7bb6bf8363`  
		Last Modified: Tue, 25 Oct 2022 06:17:42 GMT  
		Size: 8.6 MB (8599297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72794c6cd90917676f9d44ebd1f1f244c5564c41ea99e25ce09ad37df455551`  
		Last Modified: Tue, 25 Oct 2022 06:17:42 GMT  
		Size: 11.5 MB (11507226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0eb73f65f06d3ba6bd41e6c61146c374cf595cc07b9da8e8d08207cdff5b13c`  
		Last Modified: Tue, 25 Oct 2022 06:18:06 GMT  
		Size: 54.8 MB (54848363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7ed4a8a2ecd9b8eaf5a1622f101fd89785ada6f5b963abb9d8a661f9a06bc76`  
		Last Modified: Tue, 25 Oct 2022 06:18:49 GMT  
		Size: 184.8 MB (184765896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f8a1f3a13a8adaaea5da7e387c0c6867d981753b39f1e85cc607bb0e97fa47a7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.6 MB (298606196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:922e36dda65d9735b5f1feb9124dfafb756dd2899076bce2617b826416afae3c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:57:54 GMT
ADD file:9f3a74b8856c0affe36dd4e0700a8a2686a9d2275934fd9af95135f13731d10e in / 
# Tue, 04 Oct 2022 23:57:54 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:29:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:29:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:29:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:32:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b2ee1685df1bf13149eece9e0085c6befe355f21deeea69484a3ab1fab51e40c`  
		Last Modified: Wed, 05 Oct 2022 00:03:53 GMT  
		Size: 49.7 MB (49692608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237b865ef48770b9d41964e18461ec2d393677f4fc653a0953e9f0b9773d47ac`  
		Last Modified: Wed, 05 Oct 2022 00:52:01 GMT  
		Size: 8.4 MB (8396889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902b8eea02f53006b302a3dbae787275ce520ccf78df670e0dcafbfd1c4e17cd`  
		Last Modified: Wed, 05 Oct 2022 00:52:01 GMT  
		Size: 10.7 MB (10661490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540119c620ce1fcebd013dc72077ca8f4751440b9eb633b56bd350f29e749420`  
		Last Modified: Wed, 05 Oct 2022 00:52:26 GMT  
		Size: 53.0 MB (53011353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a5488439a4130d35884d12b04702afc44c003d55109f1c35f807bec217827a`  
		Last Modified: Wed, 05 Oct 2022 00:53:14 GMT  
		Size: 176.8 MB (176843856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ee5b64f7e30f64d230a9ff27700194f9626fb19c2c73fe165d174212296040a2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.6 MB (331564773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84aff2caea9cce7230accd474a102aed797b4fe65257864e59b236a314318e71`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:45:44 GMT
ADD file:83253dd857c3f1ea456b2b77494a2d865a467a36c188ecaeaf493faa5afb4c1c in / 
# Tue, 25 Oct 2022 05:45:44 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:56:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:56:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 07:57:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:58:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bec7a4c1eec818efa32bedb19eba072edfb65db7384f73efc2a6ee7b13a3ca49`  
		Last Modified: Tue, 25 Oct 2022 05:48:08 GMT  
		Size: 51.3 MB (51263048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4dc154ad7b510114eae26976432c9de05c3e285368849cc3bf60481e326fa2`  
		Last Modified: Tue, 25 Oct 2022 08:29:25 GMT  
		Size: 9.0 MB (8982532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4415de5e6c24b057c96d4d8d3d21d5834d4e30729a87dda8eb4f92335d108f53`  
		Last Modified: Tue, 25 Oct 2022 08:29:25 GMT  
		Size: 11.8 MB (11833453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2f80dfabd19f4d09eacf6b535eddbd31119db80916887d34ccb44789d2c48d`  
		Last Modified: Tue, 25 Oct 2022 08:29:42 GMT  
		Size: 57.0 MB (57038097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d56771029d9a89dd111cdb7504b5beb3d00b15609edb9efb094397bcd1b35b`  
		Last Modified: Tue, 25 Oct 2022 08:30:12 GMT  
		Size: 202.4 MB (202447643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:cd231c46916a59c2c2bc5835368b83385c4b55bf48767e2a85292860022b37aa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.5 MB (344545856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a75efaa56b01dda2b7cfee3829312128b18b88f8201eb147e8e83c442bfb2e2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:21:54 GMT
ADD file:f47fc1d53965bb08e38b482e78bd79e3cbeecc53e586ffd88bff0e6fed0a1f3c in / 
# Tue, 25 Oct 2022 02:21:55 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:12:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:12:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 05:13:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:14:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11f88873ba86e184f57ba78457d36c4f22e16eaffb9c293964adc7905e18bfe5`  
		Last Modified: Tue, 25 Oct 2022 02:27:09 GMT  
		Size: 52.2 MB (52224672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:683bf09527f61248ec1a0fa70be7388069c28d961ae31bd3a05c43ae41192a7a`  
		Last Modified: Tue, 25 Oct 2022 05:26:29 GMT  
		Size: 9.3 MB (9330348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823ddfa7a0daf2e9e0c4b6ce038b2e2cce83bde4ba9aef56fb6911d8241ca03d`  
		Last Modified: Tue, 25 Oct 2022 05:26:29 GMT  
		Size: 12.1 MB (12094186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f47813fb488b28b2af09c6f4d188832f52b886546c7885a3bb2d1b67b0d69be`  
		Last Modified: Tue, 25 Oct 2022 05:26:48 GMT  
		Size: 58.6 MB (58616294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7ff00f1ad533c8fdcd88e287626a678680009104d15d1e1eadf92ce8d913b96`  
		Last Modified: Tue, 25 Oct 2022 05:27:25 GMT  
		Size: 212.3 MB (212280356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:e96c56d3802f1d03989d4afc1c9e54f75b256e0ab531932a5452aefc857c2b97
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **319.9 MB (319903659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d117325794165da4de7ce6de9904f16f3847ebfa03ff1dbda099d1546e9c8aba`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:08:36 GMT
ADD file:f17f2d6b2018174ed9b628a69ee630ae6e011a3022bb5a0f3196ef9009d39270 in / 
# Wed, 05 Oct 2022 00:08:41 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:01:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:02:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:04:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:11:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:17006ab86ecbcadb62dabb0d565c7783b28660c51cccb5d7b46f01518a3753a3`  
		Last Modified: Wed, 05 Oct 2022 00:16:34 GMT  
		Size: 53.0 MB (52966979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cc6e8e3ab563929336c7963595d1f292897822342a96c95dcb7cff4bc403b4`  
		Last Modified: Wed, 05 Oct 2022 01:28:47 GMT  
		Size: 8.7 MB (8663556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018c7dae3a16e88ec9bace52486f5c77ed5891921868e64784dd35f09d55ab46`  
		Last Modified: Wed, 05 Oct 2022 01:28:47 GMT  
		Size: 11.1 MB (11128331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e031ef7803b56989f08a0276998fb1edfcabb65ab13ea4a75513a55ad575bc42`  
		Last Modified: Wed, 05 Oct 2022 01:29:37 GMT  
		Size: 56.0 MB (56034915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc6482afe3cbf6106cb4fac04ae9d8ed471a7830e0984fba53bec6d8616c441`  
		Last Modified: Wed, 05 Oct 2022 01:31:49 GMT  
		Size: 191.1 MB (191109878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:10b2439d4c94fc7a0ba39b4e84eaed23c271b8710fe08cfbd1ae8d6f6670d842
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.8 MB (353751941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c23610f60883dea822eec2be63953e6e838d90afc6601ab133f664b2867939f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:12:50 GMT
ADD file:1f55ca9aa64d69398e6bff99fdfd63dbf022ecefc46450a6fd32ae46e9718557 in / 
# Tue, 25 Oct 2022 03:12:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:09:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:09:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:10:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:13:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:264fa02db63011b604885c7feecaeb78fbee4ce4d8191fa5050f4fef88c74001`  
		Last Modified: Tue, 25 Oct 2022 03:18:00 GMT  
		Size: 55.3 MB (55338800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1baf225de572024a1c39187c5ece555fd8056d94bb80d56f889f4e825aa70b`  
		Last Modified: Tue, 25 Oct 2022 06:47:11 GMT  
		Size: 9.7 MB (9732694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55c6a98be02e0940d4fe69cf5b8ef19e3e86304cda7170f1dd085e4a01338a2`  
		Last Modified: Tue, 25 Oct 2022 06:47:11 GMT  
		Size: 12.7 MB (12677561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e65982f752eb81f7771ff52e7dc61db3a43a5e7b89882ff7934a391492daaae`  
		Last Modified: Tue, 25 Oct 2022 06:47:45 GMT  
		Size: 61.9 MB (61899359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3848d68d34827501ccc99d058522edfc766c2b8e572d9746ee9fe584768e46a6`  
		Last Modified: Tue, 25 Oct 2022 06:48:47 GMT  
		Size: 214.1 MB (214103527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3187110300a65451f0ac705920a497de95773130cd67d6e0c464fcd99b688388
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.8 MB (309800763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fa4a44fa173102a4106d3d5e3dafaaa3a72e2769418c8076d5f4f047a14ef7c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:13:56 GMT
ADD file:92a462945d4b32c30f41478992b9ab30d452ac37b0ecef64e2325e4e99296ea8 in / 
# Tue, 25 Oct 2022 01:13:58 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:29:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:29:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 02:30:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:30:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e544dc28605cf962b36f5ba4703f824c022460d64f8973e49764cd76163df5ff`  
		Last Modified: Tue, 25 Oct 2022 01:18:08 GMT  
		Size: 49.6 MB (49578501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50715b09b75ed5a3b59f5532be8529ac130746e899c823894a3ee91fc976a5ed`  
		Last Modified: Tue, 25 Oct 2022 02:48:44 GMT  
		Size: 8.8 MB (8785586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09bb8ed5a6b2d134cb7b866721196b0adaa54ab94d27c13c65773f16fffc143d`  
		Last Modified: Tue, 25 Oct 2022 02:48:44 GMT  
		Size: 11.7 MB (11727044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094b78b28a264fd0d8e36e29b1b3e4c349049eedd6af26957228a4bb291b7f90`  
		Last Modified: Tue, 25 Oct 2022 02:48:58 GMT  
		Size: 56.4 MB (56393185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7928bcdca7e0273482c1c8420378652a6c34aba7f44c83eef04a283ed7cb46da`  
		Last Modified: Tue, 25 Oct 2022 02:49:25 GMT  
		Size: 183.3 MB (183316447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bookworm-curl`

```console
$ docker pull buildpack-deps@sha256:e5a6600893bb6c0ca5d5ca3f2563e5500212cced47a82394304054187061a5de
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
$ docker pull buildpack-deps@sha256:65f4152e56d007d77c7d77e60f052056273d3a9ecd93ec0ee27f03e9d06c15a2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73642716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4264bd0b8285ea524f31b2355c6cd723c750a6c269a38987e6a7776185b1666`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:03 GMT
ADD file:ca5a5911d0951e5c75f1790eb644a6fd41dcb9712fa2af0fb6d3a537a72e6ad8 in / 
# Tue, 04 Oct 2022 23:26:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:52:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:52:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6674a3ae4f8f54c2f747bad2069e50ce00e352d650887729310d984cebecea22`  
		Last Modified: Tue, 04 Oct 2022 23:29:50 GMT  
		Size: 53.0 MB (52962415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e064222ce493e48ae4ceac8f18316e08d2afb963ad57bd63b8630a0ae009f8`  
		Last Modified: Wed, 05 Oct 2022 01:18:07 GMT  
		Size: 9.3 MB (9298646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab229472e3a483409ce2bbc4d461fc6512c03c687daf6546b52705bc7f18961`  
		Last Modified: Wed, 05 Oct 2022 01:18:08 GMT  
		Size: 11.4 MB (11381655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:20a4a8343b1da71a409f34e1f00df05ec1afb92deef31bf069ccfcba95ef865a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.3 MB (70284894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50b5509fe779851e321daf80c976e594a6bc3082ea32eb4bd672f0808170781a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:05:47 GMT
ADD file:226ff5e5e8066a03822e2865c6f72c554de94710c5664ee8bebd127d8aa32388 in / 
# Tue, 25 Oct 2022 03:05:48 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:08:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:08:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:cff7bd795d206b13b585de0da179a0c9616a5278eb7d74a97c97746085567403`  
		Last Modified: Tue, 25 Oct 2022 03:10:30 GMT  
		Size: 50.2 MB (50178371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40202823259eac4be0260092f1fb5f25fa9d866c32ec384dcadb0c7bb6bf8363`  
		Last Modified: Tue, 25 Oct 2022 06:17:42 GMT  
		Size: 8.6 MB (8599297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72794c6cd90917676f9d44ebd1f1f244c5564c41ea99e25ce09ad37df455551`  
		Last Modified: Tue, 25 Oct 2022 06:17:42 GMT  
		Size: 11.5 MB (11507226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:5b0dee0e2cc0e1938cf13bff64e7e8012209764899a65e170b1d0ebc91e645e3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68750987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d654a5ab6c7cd35f5bd3a5856e37d1f2b004dd7fd02791250fb62401d704090`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:57:54 GMT
ADD file:9f3a74b8856c0affe36dd4e0700a8a2686a9d2275934fd9af95135f13731d10e in / 
# Tue, 04 Oct 2022 23:57:54 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:29:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:29:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b2ee1685df1bf13149eece9e0085c6befe355f21deeea69484a3ab1fab51e40c`  
		Last Modified: Wed, 05 Oct 2022 00:03:53 GMT  
		Size: 49.7 MB (49692608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237b865ef48770b9d41964e18461ec2d393677f4fc653a0953e9f0b9773d47ac`  
		Last Modified: Wed, 05 Oct 2022 00:52:01 GMT  
		Size: 8.4 MB (8396889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902b8eea02f53006b302a3dbae787275ce520ccf78df670e0dcafbfd1c4e17cd`  
		Last Modified: Wed, 05 Oct 2022 00:52:01 GMT  
		Size: 10.7 MB (10661490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:2ccd628358c05a1df1a611b3f2ddb74940265bbf961c494a44ad3dcdd8faf922
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.1 MB (72079033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bf40f5b1eb3957c789e1c4d10270c32dd0616f31b280461f8d4e00e823a5552`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:45:44 GMT
ADD file:83253dd857c3f1ea456b2b77494a2d865a467a36c188ecaeaf493faa5afb4c1c in / 
# Tue, 25 Oct 2022 05:45:44 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:56:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:56:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:bec7a4c1eec818efa32bedb19eba072edfb65db7384f73efc2a6ee7b13a3ca49`  
		Last Modified: Tue, 25 Oct 2022 05:48:08 GMT  
		Size: 51.3 MB (51263048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4dc154ad7b510114eae26976432c9de05c3e285368849cc3bf60481e326fa2`  
		Last Modified: Tue, 25 Oct 2022 08:29:25 GMT  
		Size: 9.0 MB (8982532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4415de5e6c24b057c96d4d8d3d21d5834d4e30729a87dda8eb4f92335d108f53`  
		Last Modified: Tue, 25 Oct 2022 08:29:25 GMT  
		Size: 11.8 MB (11833453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:167dce0d41220877a7d69d1e1e4402a1f7db01d68c2ede73609723628b0d8d40
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73649206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e11ce92eb7a28e68b38ee4db9094ad80ebf756d2c10f5310aacf4d6fe927bfc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:21:54 GMT
ADD file:f47fc1d53965bb08e38b482e78bd79e3cbeecc53e586ffd88bff0e6fed0a1f3c in / 
# Tue, 25 Oct 2022 02:21:55 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:12:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:12:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:11f88873ba86e184f57ba78457d36c4f22e16eaffb9c293964adc7905e18bfe5`  
		Last Modified: Tue, 25 Oct 2022 02:27:09 GMT  
		Size: 52.2 MB (52224672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:683bf09527f61248ec1a0fa70be7388069c28d961ae31bd3a05c43ae41192a7a`  
		Last Modified: Tue, 25 Oct 2022 05:26:29 GMT  
		Size: 9.3 MB (9330348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823ddfa7a0daf2e9e0c4b6ce038b2e2cce83bde4ba9aef56fb6911d8241ca03d`  
		Last Modified: Tue, 25 Oct 2022 05:26:29 GMT  
		Size: 12.1 MB (12094186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:493af583c74bf77e0b891e256e7da2871572e0ac49991ed4bd9ffed3bc97e620
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.8 MB (72758866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:478aeba09b867d6194866aa4f12b4d9bfb445ad80db4cd1a7f24338c467bc945`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:08:36 GMT
ADD file:f17f2d6b2018174ed9b628a69ee630ae6e011a3022bb5a0f3196ef9009d39270 in / 
# Wed, 05 Oct 2022 00:08:41 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:01:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:02:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:17006ab86ecbcadb62dabb0d565c7783b28660c51cccb5d7b46f01518a3753a3`  
		Last Modified: Wed, 05 Oct 2022 00:16:34 GMT  
		Size: 53.0 MB (52966979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cc6e8e3ab563929336c7963595d1f292897822342a96c95dcb7cff4bc403b4`  
		Last Modified: Wed, 05 Oct 2022 01:28:47 GMT  
		Size: 8.7 MB (8663556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018c7dae3a16e88ec9bace52486f5c77ed5891921868e64784dd35f09d55ab46`  
		Last Modified: Wed, 05 Oct 2022 01:28:47 GMT  
		Size: 11.1 MB (11128331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:8e9cde9494655880ad5e98d1f19c1e7753f180d5e1350dc775dd60d8d1f98846
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.7 MB (77749055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3320b26d31e084b5b012dcb3b58bcd0cddfcb8d3c6ed8349cebe37bed468b61`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:12:50 GMT
ADD file:1f55ca9aa64d69398e6bff99fdfd63dbf022ecefc46450a6fd32ae46e9718557 in / 
# Tue, 25 Oct 2022 03:12:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:09:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:09:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:264fa02db63011b604885c7feecaeb78fbee4ce4d8191fa5050f4fef88c74001`  
		Last Modified: Tue, 25 Oct 2022 03:18:00 GMT  
		Size: 55.3 MB (55338800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1baf225de572024a1c39187c5ece555fd8056d94bb80d56f889f4e825aa70b`  
		Last Modified: Tue, 25 Oct 2022 06:47:11 GMT  
		Size: 9.7 MB (9732694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55c6a98be02e0940d4fe69cf5b8ef19e3e86304cda7170f1dd085e4a01338a2`  
		Last Modified: Tue, 25 Oct 2022 06:47:11 GMT  
		Size: 12.7 MB (12677561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:894b1261a23e6de74babe1ee3f40ba9e50b5c66394124baddfddd8c053c67ccf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.1 MB (70091131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0d41791c8becaef1121c6430e271e2135e1dc7887ebe7a1da86fdacbd5a8eaa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:13:56 GMT
ADD file:92a462945d4b32c30f41478992b9ab30d452ac37b0ecef64e2325e4e99296ea8 in / 
# Tue, 25 Oct 2022 01:13:58 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:29:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:29:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e544dc28605cf962b36f5ba4703f824c022460d64f8973e49764cd76163df5ff`  
		Last Modified: Tue, 25 Oct 2022 01:18:08 GMT  
		Size: 49.6 MB (49578501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50715b09b75ed5a3b59f5532be8529ac130746e899c823894a3ee91fc976a5ed`  
		Last Modified: Tue, 25 Oct 2022 02:48:44 GMT  
		Size: 8.8 MB (8785586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09bb8ed5a6b2d134cb7b866721196b0adaa54ab94d27c13c65773f16fffc143d`  
		Last Modified: Tue, 25 Oct 2022 02:48:44 GMT  
		Size: 11.7 MB (11727044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bookworm-scm`

```console
$ docker pull buildpack-deps@sha256:b9e0da7d52fc1e1ef0815334215b86b36631a7e6608bced2cd595865dfa67fea
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
$ docker pull buildpack-deps@sha256:000ac73bce79972e52d53c962a31162be24fdc559f0538904ee6a0150d222c68
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.8 MB (130843993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7945f5e0e10aedb5f27374316d0f3c7b5531582fae4f0662e75f879cc562a3f4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:03 GMT
ADD file:ca5a5911d0951e5c75f1790eb644a6fd41dcb9712fa2af0fb6d3a537a72e6ad8 in / 
# Tue, 04 Oct 2022 23:26:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:52:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:52:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:52:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6674a3ae4f8f54c2f747bad2069e50ce00e352d650887729310d984cebecea22`  
		Last Modified: Tue, 04 Oct 2022 23:29:50 GMT  
		Size: 53.0 MB (52962415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e064222ce493e48ae4ceac8f18316e08d2afb963ad57bd63b8630a0ae009f8`  
		Last Modified: Wed, 05 Oct 2022 01:18:07 GMT  
		Size: 9.3 MB (9298646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab229472e3a483409ce2bbc4d461fc6512c03c687daf6546b52705bc7f18961`  
		Last Modified: Wed, 05 Oct 2022 01:18:08 GMT  
		Size: 11.4 MB (11381655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93a5a87ebbd4472db252972521c82b5789bcc45b6bf1ff4d5e59ab129a4847a`  
		Last Modified: Wed, 05 Oct 2022 01:18:25 GMT  
		Size: 57.2 MB (57201277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:bd890e3ac7fa16b49f774875a45a77bb1e7ae1299879970541ab68e599add920
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.1 MB (125133257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a3ab1b7aecdfddcde09b5a928e85f6963370f7286f701da119d78dd0fe10c85`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:05:47 GMT
ADD file:226ff5e5e8066a03822e2865c6f72c554de94710c5664ee8bebd127d8aa32388 in / 
# Tue, 25 Oct 2022 03:05:48 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:08:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:08:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:09:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cff7bd795d206b13b585de0da179a0c9616a5278eb7d74a97c97746085567403`  
		Last Modified: Tue, 25 Oct 2022 03:10:30 GMT  
		Size: 50.2 MB (50178371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40202823259eac4be0260092f1fb5f25fa9d866c32ec384dcadb0c7bb6bf8363`  
		Last Modified: Tue, 25 Oct 2022 06:17:42 GMT  
		Size: 8.6 MB (8599297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72794c6cd90917676f9d44ebd1f1f244c5564c41ea99e25ce09ad37df455551`  
		Last Modified: Tue, 25 Oct 2022 06:17:42 GMT  
		Size: 11.5 MB (11507226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0eb73f65f06d3ba6bd41e6c61146c374cf595cc07b9da8e8d08207cdff5b13c`  
		Last Modified: Tue, 25 Oct 2022 06:18:06 GMT  
		Size: 54.8 MB (54848363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:2daee8056defbefb7c44552cd1459e5679697f2c0b0d6dcea2ec5040b4ea1137
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121762340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65bd8e30ab8ce2052ff48b213f632b23717eb24125bc8a555a52332d56a64ce4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:57:54 GMT
ADD file:9f3a74b8856c0affe36dd4e0700a8a2686a9d2275934fd9af95135f13731d10e in / 
# Tue, 04 Oct 2022 23:57:54 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:29:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:29:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:29:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b2ee1685df1bf13149eece9e0085c6befe355f21deeea69484a3ab1fab51e40c`  
		Last Modified: Wed, 05 Oct 2022 00:03:53 GMT  
		Size: 49.7 MB (49692608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237b865ef48770b9d41964e18461ec2d393677f4fc653a0953e9f0b9773d47ac`  
		Last Modified: Wed, 05 Oct 2022 00:52:01 GMT  
		Size: 8.4 MB (8396889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902b8eea02f53006b302a3dbae787275ce520ccf78df670e0dcafbfd1c4e17cd`  
		Last Modified: Wed, 05 Oct 2022 00:52:01 GMT  
		Size: 10.7 MB (10661490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540119c620ce1fcebd013dc72077ca8f4751440b9eb633b56bd350f29e749420`  
		Last Modified: Wed, 05 Oct 2022 00:52:26 GMT  
		Size: 53.0 MB (53011353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:04516cc98d3556b69d602a778fcc926cd176190c038ce4d315c5cf14d37b282a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.1 MB (129117130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41da76e26040b5bf1fc2bcaf32382c780d6103a841e405cfa8abb0442b2e3c87`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:45:44 GMT
ADD file:83253dd857c3f1ea456b2b77494a2d865a467a36c188ecaeaf493faa5afb4c1c in / 
# Tue, 25 Oct 2022 05:45:44 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:56:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:56:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 07:57:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bec7a4c1eec818efa32bedb19eba072edfb65db7384f73efc2a6ee7b13a3ca49`  
		Last Modified: Tue, 25 Oct 2022 05:48:08 GMT  
		Size: 51.3 MB (51263048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4dc154ad7b510114eae26976432c9de05c3e285368849cc3bf60481e326fa2`  
		Last Modified: Tue, 25 Oct 2022 08:29:25 GMT  
		Size: 9.0 MB (8982532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4415de5e6c24b057c96d4d8d3d21d5834d4e30729a87dda8eb4f92335d108f53`  
		Last Modified: Tue, 25 Oct 2022 08:29:25 GMT  
		Size: 11.8 MB (11833453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2f80dfabd19f4d09eacf6b535eddbd31119db80916887d34ccb44789d2c48d`  
		Last Modified: Tue, 25 Oct 2022 08:29:42 GMT  
		Size: 57.0 MB (57038097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:bb8f335fbccf0d2040d44a9901f5d5892fddf6faf56f84c2699db34d21e91570
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.3 MB (132265500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:533c3f4baead23baa420e1ab640834843dc1a50aec17fc4a2c085177b12d89ce`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:21:54 GMT
ADD file:f47fc1d53965bb08e38b482e78bd79e3cbeecc53e586ffd88bff0e6fed0a1f3c in / 
# Tue, 25 Oct 2022 02:21:55 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:12:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:12:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 05:13:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11f88873ba86e184f57ba78457d36c4f22e16eaffb9c293964adc7905e18bfe5`  
		Last Modified: Tue, 25 Oct 2022 02:27:09 GMT  
		Size: 52.2 MB (52224672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:683bf09527f61248ec1a0fa70be7388069c28d961ae31bd3a05c43ae41192a7a`  
		Last Modified: Tue, 25 Oct 2022 05:26:29 GMT  
		Size: 9.3 MB (9330348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823ddfa7a0daf2e9e0c4b6ce038b2e2cce83bde4ba9aef56fb6911d8241ca03d`  
		Last Modified: Tue, 25 Oct 2022 05:26:29 GMT  
		Size: 12.1 MB (12094186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f47813fb488b28b2af09c6f4d188832f52b886546c7885a3bb2d1b67b0d69be`  
		Last Modified: Tue, 25 Oct 2022 05:26:48 GMT  
		Size: 58.6 MB (58616294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:c942e931db31d5c2e72264278254cf3270324e3f44fb7f1395d1bb1521d12600
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.8 MB (128793781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40553f8f691301cee00d5f713fbac8c57b59252c2dd9245ae7f5714fe6e1495d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:08:36 GMT
ADD file:f17f2d6b2018174ed9b628a69ee630ae6e011a3022bb5a0f3196ef9009d39270 in / 
# Wed, 05 Oct 2022 00:08:41 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:01:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:02:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:04:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:17006ab86ecbcadb62dabb0d565c7783b28660c51cccb5d7b46f01518a3753a3`  
		Last Modified: Wed, 05 Oct 2022 00:16:34 GMT  
		Size: 53.0 MB (52966979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cc6e8e3ab563929336c7963595d1f292897822342a96c95dcb7cff4bc403b4`  
		Last Modified: Wed, 05 Oct 2022 01:28:47 GMT  
		Size: 8.7 MB (8663556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018c7dae3a16e88ec9bace52486f5c77ed5891921868e64784dd35f09d55ab46`  
		Last Modified: Wed, 05 Oct 2022 01:28:47 GMT  
		Size: 11.1 MB (11128331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e031ef7803b56989f08a0276998fb1edfcabb65ab13ea4a75513a55ad575bc42`  
		Last Modified: Wed, 05 Oct 2022 01:29:37 GMT  
		Size: 56.0 MB (56034915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:8aedd3f69ab37457552ec526445326e02d180a5e2d4fcd5e9921b0acccee7f55
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.6 MB (139648414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06e4d95381966110ef09af6732f8433a26f7b8e7f0895481c387ea2612e84de8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:12:50 GMT
ADD file:1f55ca9aa64d69398e6bff99fdfd63dbf022ecefc46450a6fd32ae46e9718557 in / 
# Tue, 25 Oct 2022 03:12:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:09:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:09:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:10:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:264fa02db63011b604885c7feecaeb78fbee4ce4d8191fa5050f4fef88c74001`  
		Last Modified: Tue, 25 Oct 2022 03:18:00 GMT  
		Size: 55.3 MB (55338800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1baf225de572024a1c39187c5ece555fd8056d94bb80d56f889f4e825aa70b`  
		Last Modified: Tue, 25 Oct 2022 06:47:11 GMT  
		Size: 9.7 MB (9732694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55c6a98be02e0940d4fe69cf5b8ef19e3e86304cda7170f1dd085e4a01338a2`  
		Last Modified: Tue, 25 Oct 2022 06:47:11 GMT  
		Size: 12.7 MB (12677561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e65982f752eb81f7771ff52e7dc61db3a43a5e7b89882ff7934a391492daaae`  
		Last Modified: Tue, 25 Oct 2022 06:47:45 GMT  
		Size: 61.9 MB (61899359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:221812309a8315f40e7a00439dfae7b687e3828c543190683390eec5bc6263dd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126484316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c27b9f13f925e68613971e6806d863cbc335c648a119e6ce33664f7874816557`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:13:56 GMT
ADD file:92a462945d4b32c30f41478992b9ab30d452ac37b0ecef64e2325e4e99296ea8 in / 
# Tue, 25 Oct 2022 01:13:58 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:29:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:29:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 02:30:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e544dc28605cf962b36f5ba4703f824c022460d64f8973e49764cd76163df5ff`  
		Last Modified: Tue, 25 Oct 2022 01:18:08 GMT  
		Size: 49.6 MB (49578501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50715b09b75ed5a3b59f5532be8529ac130746e899c823894a3ee91fc976a5ed`  
		Last Modified: Tue, 25 Oct 2022 02:48:44 GMT  
		Size: 8.8 MB (8785586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09bb8ed5a6b2d134cb7b866721196b0adaa54ab94d27c13c65773f16fffc143d`  
		Last Modified: Tue, 25 Oct 2022 02:48:44 GMT  
		Size: 11.7 MB (11727044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094b78b28a264fd0d8e36e29b1b3e4c349049eedd6af26957228a4bb291b7f90`  
		Last Modified: Tue, 25 Oct 2022 02:48:58 GMT  
		Size: 56.4 MB (56393185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bullseye`

```console
$ docker pull buildpack-deps@sha256:4c611d88a39769ef8b4a77505f9377f74df78ae41bf9f81be47522d13549ba1b
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
$ docker pull buildpack-deps@sha256:da6442775441c5a43c9cdcbc18c633c9a94196521736ea0c04d3bc4ab6d24007
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.5 MB (322518570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c35b468f323a45e3ac977f6960f5657ec31473c3a183f96f5ff908fdfa3f9b8d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:27 GMT
ADD file:d1268789456d2cdace6e50149e60404ad5a849b7c61e8fc8bc7b6e0eb6eeb7ca in / 
# Tue, 04 Oct 2022 23:26:27 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:54:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:55:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:55:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:56:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f606d8928ed378229f2460b94b504cca239fb906efc57acbdf9340bd298d5ddf`  
		Last Modified: Tue, 04 Oct 2022 23:30:27 GMT  
		Size: 55.0 MB (55046248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47db815c6a4547dc224b75222193cb1851cf529d2cbdf26f854b9bbf97099b98`  
		Last Modified: Wed, 05 Oct 2022 01:19:13 GMT  
		Size: 5.2 MB (5163279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf48494000001a037b72870d2a6a2536f9da8bc5d1ceddd72d79f4a51fe7a60e`  
		Last Modified: Wed, 05 Oct 2022 01:19:13 GMT  
		Size: 10.9 MB (10876505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a572f7a256d36a93ab0777949771b120c5d7dce75ea2a2d3d9444793b26b2ef1`  
		Last Modified: Wed, 05 Oct 2022 01:19:34 GMT  
		Size: 54.6 MB (54584293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f7d0525895528fdb73153451e112bbd8e1854549bd1e0e6f4ac0b4a2ee98172`  
		Last Modified: Wed, 05 Oct 2022 01:20:11 GMT  
		Size: 196.8 MB (196848245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:e95f5a44cff65278e6f2df29eef9d7957e19ab74e610841ca613250500cfb07c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.6 MB (295556261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5fc1f9478434ff5825094db6336cb96abec3dff210ea3918afc05508b3b8389`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:06:19 GMT
ADD file:b314b98654e8532fd10a08a172ea5c3edb7d7a36c7faf85d06d14be12f7b83ef in / 
# Tue, 25 Oct 2022 03:06:19 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:12:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:12:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:12:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:14:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1f0ecb08923b99bef3f82c2e88603bb53e3ed084c13252275c05039cc279c158`  
		Last Modified: Tue, 25 Oct 2022 03:11:15 GMT  
		Size: 52.5 MB (52547473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b399c5eb53b4c35fa33682a82d73bdc4b096cd78ae95fe36c4ed81d18f6849`  
		Last Modified: Tue, 25 Oct 2022 06:19:02 GMT  
		Size: 5.1 MB (5072235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ccdd06393cd3873a3cc8b9cbe170a2032fd61d1d545b7045b649faf2f4e732`  
		Last Modified: Tue, 25 Oct 2022 06:19:02 GMT  
		Size: 10.6 MB (10574279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aafe0e287af4e488dcda51195e4eb1ae1386e3265989c457172f32f6357bf26`  
		Last Modified: Tue, 25 Oct 2022 06:19:28 GMT  
		Size: 52.3 MB (52322157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22771ccea19352dbb0e5ba44c17b8ef14425ff0a22c744bca41cdbde02bdfd9f`  
		Last Modified: Tue, 25 Oct 2022 06:20:12 GMT  
		Size: 175.0 MB (175040117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:4ef648e774c537efc33738cca9dfbc87771bbbaab19e36fffdc55e0f440c699a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.0 MB (283005348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe5e78b4d0fb86176858f424786c09b823ee34558e44538321f40a14100f6a57`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:28 GMT
ADD file:47a3f2948af18c39686ca59a88a439c25edaf286064d3a2ccc5dab47fee2fc52 in / 
# Tue, 04 Oct 2022 23:58:29 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:32:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:32:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:32:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:34:32 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e19342fb46cabf6147aec1d1c6af1f3a82736530cf3b067835fc8a09da092ce3`  
		Last Modified: Wed, 05 Oct 2022 00:04:36 GMT  
		Size: 50.2 MB (50209087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a49f93f990f17337480b5bdf526a6bb48d1ae63bd17f54be17cd2f6ebba4de7d`  
		Last Modified: Wed, 05 Oct 2022 00:53:28 GMT  
		Size: 4.9 MB (4931366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3989be0d7ed2f72fae0310039043f6ba76c24a45f9ec9689697ebd932845cc8`  
		Last Modified: Wed, 05 Oct 2022 00:53:28 GMT  
		Size: 10.2 MB (10217872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6487a2e4236617393a6184f0f89a360d295ab118da2ea4ad48fa8645ae211755`  
		Last Modified: Wed, 05 Oct 2022 00:53:57 GMT  
		Size: 50.3 MB (50343324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cb778b20f33d18ee7b4046bfd5685ddf5bb8750a2f3826f14408897c4d9db5`  
		Last Modified: Wed, 05 Oct 2022 00:54:45 GMT  
		Size: 167.3 MB (167303699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:bba56093d706c0b145e14ee726d81f59b1d09e069d3b84c30e9bee0af5a24687
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.2 MB (314172338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c2f1635631cecb5159531c9282693f4a86c19d02ec9f92e0f40baa073e51f5b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:45:55 GMT
ADD file:b16745ece8ef84c028d7e9ac4bf026ac64f885d4170bfcc9d435f237144a1b99 in / 
# Tue, 25 Oct 2022 05:45:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:58:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:58:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 07:59:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:00:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8e1d92e7d04d2a9a9880cb45dc3c32c2805912cd86abed96d0ada3ff28748205`  
		Last Modified: Tue, 25 Oct 2022 05:48:40 GMT  
		Size: 53.7 MB (53701966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66eadbf427bb41b3e329a95935c65b09c6d3b7a9c2fa8e08417e497df02ed996`  
		Last Modified: Tue, 25 Oct 2022 08:30:22 GMT  
		Size: 5.2 MB (5151506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9731f4e3bc3680179c10cece663cf0cfe0488918d6795406f4b76f07b787de`  
		Last Modified: Tue, 25 Oct 2022 08:30:22 GMT  
		Size: 10.9 MB (10874174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d337cb12fd7c6fe341850cd38e880f1806d49a65832c9804b06d00f9032382e0`  
		Last Modified: Tue, 25 Oct 2022 08:30:42 GMT  
		Size: 54.7 MB (54683990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a719597fe1ca78e1dc4c43fffc424754228514a791abcb0e0c06302ad022b8ca`  
		Last Modified: Tue, 25 Oct 2022 08:31:12 GMT  
		Size: 189.8 MB (189760702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; 386

```console
$ docker pull buildpack-deps@sha256:730efefe6d075835e0fede96affe8d8631d8212509b4c7003c32b47bf3c550b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.8 MB (327836520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d42762c45517dca640707932c4cfb4d4903431b010d2feb9a29f09b820a3ed5b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:22:19 GMT
ADD file:aa26f69b37c3e144d08e17bb9be7302ec89ae0579121c874a35f336d7077fd3b in / 
# Tue, 25 Oct 2022 02:22:19 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:15:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:15:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 05:15:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:16:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8caf426a2703f99fb0be4b03411ecaa580d102f7c47ef43b422b6d7c13c380e2`  
		Last Modified: Tue, 25 Oct 2022 02:27:54 GMT  
		Size: 56.0 MB (56023960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b92a2ff5c72653a0679aa7f5e2bc695011c0a71faa424229e560957d204dab`  
		Last Modified: Tue, 25 Oct 2022 05:27:37 GMT  
		Size: 5.1 MB (5086887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6856a3002e686ceb6d48d078731366f576ed3adcb73bd49dcb300057732904`  
		Last Modified: Tue, 25 Oct 2022 05:27:38 GMT  
		Size: 11.0 MB (11032526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e88080d3b5ba1edc8623a97d068bd040dfb89f2bc7bdfc0984d11fc35ff5885`  
		Last Modified: Tue, 25 Oct 2022 05:28:00 GMT  
		Size: 55.9 MB (55924404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b19879261038142328725a860507e23c40804ec5e04f1b7cf8f0dc88ded89d`  
		Last Modified: Tue, 25 Oct 2022 05:28:37 GMT  
		Size: 199.8 MB (199768743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:6088b9f6bed37906eecc152f8a3f642c5688b69f3c6c1ec283bd420ea0168585
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.1 MB (301112687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2991accb9ec37e952acae5a8759ce6006e7e1e39739799c51bab7c987e0d7867`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:09:48 GMT
ADD file:ca40db2df3dbc600910b8cd139c564cf5b8bd6c1a06cc517cae2c1c05cff6dde in / 
# Wed, 05 Oct 2022 00:09:51 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:11:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:12:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:14:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:19:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:25bcd35faf05f859c3077f0e2e7010d24e56cdcfb77efbdeda236e47dc08e14a`  
		Last Modified: Wed, 05 Oct 2022 00:17:52 GMT  
		Size: 53.3 MB (53265834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c44f381e4f9f5eb923a09cbd49bc86d3d36121137c1e063d30d73af518bf0f86`  
		Last Modified: Wed, 05 Oct 2022 01:32:02 GMT  
		Size: 4.9 MB (4918634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59260097f47eb21e87461a2a98c76f46372dd316b878bbd3d4d9c51cc28a62b7`  
		Last Modified: Wed, 05 Oct 2022 01:32:04 GMT  
		Size: 10.7 MB (10661237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f8a68e1316af16785650ca91231ed6373810fcdaff8fb5bec9f58e1ccc2a32`  
		Last Modified: Wed, 05 Oct 2022 01:32:53 GMT  
		Size: 53.3 MB (53304716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbf1a80df4f8f31f1ab3653fe8e3b40cb5a88a81ea4bc64c95e1b388fe7e2cc`  
		Last Modified: Wed, 05 Oct 2022 01:34:59 GMT  
		Size: 179.0 MB (178962266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:39252f001a267e36e8cc4cbd5a51b22eb6f6b8c862a0eebae0f84c115268f828
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.0 MB (331028350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fe0aa4188607937a62728cb0c6bb7d668f569b3384fecff44935b02408e9068`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:13:28 GMT
ADD file:c01a6cc4222fbeeda5c2d679c5b355539880a02c792c64861eb17b81a3678f45 in / 
# Tue, 25 Oct 2022 03:13:31 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:13:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:14:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:14:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:16:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ee5a342763ed1d31bef8cebe9f4cc5dd6d427f630da679a87da0427be7b22e3d`  
		Last Modified: Tue, 25 Oct 2022 03:18:52 GMT  
		Size: 58.9 MB (58916374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a4727f39cbcb19b39abdbd847eeceed842ef65f8514372024c48b913bc951a`  
		Last Modified: Tue, 25 Oct 2022 06:49:00 GMT  
		Size: 5.4 MB (5414507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe601e6c8a1ec9c69c49c65a53339202a65cea9d4f01d161fb34905c06a4a99`  
		Last Modified: Tue, 25 Oct 2022 06:49:01 GMT  
		Size: 11.6 MB (11630153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5055e27b58426c2b637b1c8c179e6abe306e3dfb55a9c170c73fb0d581c6cf3e`  
		Last Modified: Tue, 25 Oct 2022 06:49:31 GMT  
		Size: 58.9 MB (58867355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a503b0a90ce32a745c9586bc6c28360d8de222565d7105d079b530524e1e38`  
		Last Modified: Tue, 25 Oct 2022 06:50:32 GMT  
		Size: 196.2 MB (196199961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:56a7b6a421aea89e44c16d6526e1f2688c8b129fae975687ccdef4707e507432
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.1 MB (296088034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:172dabba1a37b7c132ad4884aca1fd3c1b63d62e29533b09589ac174b5c3f0f7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:14:24 GMT
ADD file:06f15d8a3c04752d271a052e820fb13fcdb76f0d18f6c9afb6e70391d10348ec in / 
# Tue, 25 Oct 2022 01:14:27 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:31:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:31:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 02:31:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:32:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a556186e8bea4ba9925d0c17bea2c12bfbb931653cfab1b980036800482cf0ad`  
		Last Modified: Tue, 25 Oct 2022 01:18:39 GMT  
		Size: 53.3 MB (53279106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1e8478a953d3a464d73e36e4032c979725bc79ce0eeb83aca30212de549b90`  
		Last Modified: Tue, 25 Oct 2022 02:49:32 GMT  
		Size: 5.1 MB (5148477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cdbee45ed722bfaf7e9ba90503afa7a0cf17b87fc1bfa1e87cbf49ca6bd7d9`  
		Last Modified: Tue, 25 Oct 2022 02:49:33 GMT  
		Size: 10.8 MB (10766704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76aacd12f54fec6c8f627f09641ea144eb6fefeebc8f9fc35de80c3e3ab11af7`  
		Last Modified: Tue, 25 Oct 2022 02:49:48 GMT  
		Size: 54.1 MB (54055853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f33c726ca8131121c45361c5d4789cbb8c58f1cf53f551af6b41f3857cb9847`  
		Last Modified: Tue, 25 Oct 2022 02:50:20 GMT  
		Size: 172.8 MB (172837894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bullseye-curl`

```console
$ docker pull buildpack-deps@sha256:f0bc68399bc76e1d562de8399f0fb2990e3bd6cc04aab46bb2eb6d789905caef
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
$ docker pull buildpack-deps@sha256:cb9a3f7bd43628db1b3695a6e7b28d561bf4df306ab1f63a0c232397690bf2dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.1 MB (71086032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1e2c1abde86fb7ff272adfa86162471d1bfa52060a0dec82087fecebdcb31e5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:27 GMT
ADD file:d1268789456d2cdace6e50149e60404ad5a849b7c61e8fc8bc7b6e0eb6eeb7ca in / 
# Tue, 04 Oct 2022 23:26:27 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:54:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:55:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f606d8928ed378229f2460b94b504cca239fb906efc57acbdf9340bd298d5ddf`  
		Last Modified: Tue, 04 Oct 2022 23:30:27 GMT  
		Size: 55.0 MB (55046248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47db815c6a4547dc224b75222193cb1851cf529d2cbdf26f854b9bbf97099b98`  
		Last Modified: Wed, 05 Oct 2022 01:19:13 GMT  
		Size: 5.2 MB (5163279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf48494000001a037b72870d2a6a2536f9da8bc5d1ceddd72d79f4a51fe7a60e`  
		Last Modified: Wed, 05 Oct 2022 01:19:13 GMT  
		Size: 10.9 MB (10876505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:c4307444787732144220d75296f55023fa4114b856df149c28e78559c50359d4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.2 MB (68193987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e39186554e8bc668aa17c37b50cd6803d4a408a41ad404ba37b3e10e2ed96267`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:06:19 GMT
ADD file:b314b98654e8532fd10a08a172ea5c3edb7d7a36c7faf85d06d14be12f7b83ef in / 
# Tue, 25 Oct 2022 03:06:19 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:12:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:12:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1f0ecb08923b99bef3f82c2e88603bb53e3ed084c13252275c05039cc279c158`  
		Last Modified: Tue, 25 Oct 2022 03:11:15 GMT  
		Size: 52.5 MB (52547473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b399c5eb53b4c35fa33682a82d73bdc4b096cd78ae95fe36c4ed81d18f6849`  
		Last Modified: Tue, 25 Oct 2022 06:19:02 GMT  
		Size: 5.1 MB (5072235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ccdd06393cd3873a3cc8b9cbe170a2032fd61d1d545b7045b649faf2f4e732`  
		Last Modified: Tue, 25 Oct 2022 06:19:02 GMT  
		Size: 10.6 MB (10574279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:fa161c8e7935e0810bcd3ca45a9746cf6e3fdc6025c5362e8bc2648f7fae6239
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65358325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b86ef37d02c678f38add592f5f88e1f266a851783e8f323eb1837a5ee7352ac7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:28 GMT
ADD file:47a3f2948af18c39686ca59a88a439c25edaf286064d3a2ccc5dab47fee2fc52 in / 
# Tue, 04 Oct 2022 23:58:29 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:32:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:32:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e19342fb46cabf6147aec1d1c6af1f3a82736530cf3b067835fc8a09da092ce3`  
		Last Modified: Wed, 05 Oct 2022 00:04:36 GMT  
		Size: 50.2 MB (50209087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a49f93f990f17337480b5bdf526a6bb48d1ae63bd17f54be17cd2f6ebba4de7d`  
		Last Modified: Wed, 05 Oct 2022 00:53:28 GMT  
		Size: 4.9 MB (4931366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3989be0d7ed2f72fae0310039043f6ba76c24a45f9ec9689697ebd932845cc8`  
		Last Modified: Wed, 05 Oct 2022 00:53:28 GMT  
		Size: 10.2 MB (10217872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:bc7e9978ee6d44bb721af5cba9e40ee69de8d269140ec556a0c40cbeee8979bb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.7 MB (69727646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c88b9fd10ad56e7d5bac1e3cb67021a7765c589e6e7d144f46d1c76d2811413d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:45:55 GMT
ADD file:b16745ece8ef84c028d7e9ac4bf026ac64f885d4170bfcc9d435f237144a1b99 in / 
# Tue, 25 Oct 2022 05:45:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:58:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:58:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8e1d92e7d04d2a9a9880cb45dc3c32c2805912cd86abed96d0ada3ff28748205`  
		Last Modified: Tue, 25 Oct 2022 05:48:40 GMT  
		Size: 53.7 MB (53701966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66eadbf427bb41b3e329a95935c65b09c6d3b7a9c2fa8e08417e497df02ed996`  
		Last Modified: Tue, 25 Oct 2022 08:30:22 GMT  
		Size: 5.2 MB (5151506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9731f4e3bc3680179c10cece663cf0cfe0488918d6795406f4b76f07b787de`  
		Last Modified: Tue, 25 Oct 2022 08:30:22 GMT  
		Size: 10.9 MB (10874174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:bf477637cd09b9031cd034fff22d013e90a3101df053d80729d928601fb7c14a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.1 MB (72143373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b4b083b9d9929246daf9a5fe0622f9a1e88bfb618b352807b23b97d75ff5a38`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:22:19 GMT
ADD file:aa26f69b37c3e144d08e17bb9be7302ec89ae0579121c874a35f336d7077fd3b in / 
# Tue, 25 Oct 2022 02:22:19 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:15:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:15:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8caf426a2703f99fb0be4b03411ecaa580d102f7c47ef43b422b6d7c13c380e2`  
		Last Modified: Tue, 25 Oct 2022 02:27:54 GMT  
		Size: 56.0 MB (56023960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b92a2ff5c72653a0679aa7f5e2bc695011c0a71faa424229e560957d204dab`  
		Last Modified: Tue, 25 Oct 2022 05:27:37 GMT  
		Size: 5.1 MB (5086887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6856a3002e686ceb6d48d078731366f576ed3adcb73bd49dcb300057732904`  
		Last Modified: Tue, 25 Oct 2022 05:27:38 GMT  
		Size: 11.0 MB (11032526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:668f750c6d59a65e45714ebe9fd3c02e2b07e166cf39df660a4b93a59449e9ad
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68845705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e70040762c35b1ea015572f262495cddda025b3d915f9fbfa15e0a0f6b02130`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:09:48 GMT
ADD file:ca40db2df3dbc600910b8cd139c564cf5b8bd6c1a06cc517cae2c1c05cff6dde in / 
# Wed, 05 Oct 2022 00:09:51 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:11:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:12:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:25bcd35faf05f859c3077f0e2e7010d24e56cdcfb77efbdeda236e47dc08e14a`  
		Last Modified: Wed, 05 Oct 2022 00:17:52 GMT  
		Size: 53.3 MB (53265834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c44f381e4f9f5eb923a09cbd49bc86d3d36121137c1e063d30d73af518bf0f86`  
		Last Modified: Wed, 05 Oct 2022 01:32:02 GMT  
		Size: 4.9 MB (4918634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59260097f47eb21e87461a2a98c76f46372dd316b878bbd3d4d9c51cc28a62b7`  
		Last Modified: Wed, 05 Oct 2022 01:32:04 GMT  
		Size: 10.7 MB (10661237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:469e7517e99c19831cea091b8ba496389124880b75d31d2718cc6c1999060b8e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.0 MB (75961034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5cb6ede5f74b2e5a7f231d8ef2d1f5728c8b419020b8d7640b6aaef3bdfe00e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:13:28 GMT
ADD file:c01a6cc4222fbeeda5c2d679c5b355539880a02c792c64861eb17b81a3678f45 in / 
# Tue, 25 Oct 2022 03:13:31 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:13:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:14:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ee5a342763ed1d31bef8cebe9f4cc5dd6d427f630da679a87da0427be7b22e3d`  
		Last Modified: Tue, 25 Oct 2022 03:18:52 GMT  
		Size: 58.9 MB (58916374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a4727f39cbcb19b39abdbd847eeceed842ef65f8514372024c48b913bc951a`  
		Last Modified: Tue, 25 Oct 2022 06:49:00 GMT  
		Size: 5.4 MB (5414507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe601e6c8a1ec9c69c49c65a53339202a65cea9d4f01d161fb34905c06a4a99`  
		Last Modified: Tue, 25 Oct 2022 06:49:01 GMT  
		Size: 11.6 MB (11630153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:809d9d381f46cf97b2154255bf1ab72c6c7126ca14bef3939630abde9638783d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69194287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14cce275c18bfdc19a1e7f27773751920f1a720c0ccd64c54a8ace1b33e0cf31`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:14:24 GMT
ADD file:06f15d8a3c04752d271a052e820fb13fcdb76f0d18f6c9afb6e70391d10348ec in / 
# Tue, 25 Oct 2022 01:14:27 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:31:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:31:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a556186e8bea4ba9925d0c17bea2c12bfbb931653cfab1b980036800482cf0ad`  
		Last Modified: Tue, 25 Oct 2022 01:18:39 GMT  
		Size: 53.3 MB (53279106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1e8478a953d3a464d73e36e4032c979725bc79ce0eeb83aca30212de549b90`  
		Last Modified: Tue, 25 Oct 2022 02:49:32 GMT  
		Size: 5.1 MB (5148477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cdbee45ed722bfaf7e9ba90503afa7a0cf17b87fc1bfa1e87cbf49ca6bd7d9`  
		Last Modified: Tue, 25 Oct 2022 02:49:33 GMT  
		Size: 10.8 MB (10766704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bullseye-scm`

```console
$ docker pull buildpack-deps@sha256:a7f1c200cd1fd667d3fec5bd3b69dd3672603ce21b7b67891fb7d3a5218874e2
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
$ docker pull buildpack-deps@sha256:fd04e21a45663223207243344f0ac8b1d9c0fe01b1b8601b25d5686a0fdbaa2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125670325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82ff4917fce4dadc637924ff195fcebb04273691c7152bcc869fb766c88d8e15`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:27 GMT
ADD file:d1268789456d2cdace6e50149e60404ad5a849b7c61e8fc8bc7b6e0eb6eeb7ca in / 
# Tue, 04 Oct 2022 23:26:27 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:54:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:55:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:55:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f606d8928ed378229f2460b94b504cca239fb906efc57acbdf9340bd298d5ddf`  
		Last Modified: Tue, 04 Oct 2022 23:30:27 GMT  
		Size: 55.0 MB (55046248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47db815c6a4547dc224b75222193cb1851cf529d2cbdf26f854b9bbf97099b98`  
		Last Modified: Wed, 05 Oct 2022 01:19:13 GMT  
		Size: 5.2 MB (5163279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf48494000001a037b72870d2a6a2536f9da8bc5d1ceddd72d79f4a51fe7a60e`  
		Last Modified: Wed, 05 Oct 2022 01:19:13 GMT  
		Size: 10.9 MB (10876505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a572f7a256d36a93ab0777949771b120c5d7dce75ea2a2d3d9444793b26b2ef1`  
		Last Modified: Wed, 05 Oct 2022 01:19:34 GMT  
		Size: 54.6 MB (54584293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:b510585c7c0379882b7436c2ba9f2bcdf9fa4cadd1aa9e71b177f1bb9bcc57e5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.5 MB (120516144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b46050aede040f8a40b0df16c1d9ec4720cde12aeb7b220cd6ac40588a3ddeb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:06:19 GMT
ADD file:b314b98654e8532fd10a08a172ea5c3edb7d7a36c7faf85d06d14be12f7b83ef in / 
# Tue, 25 Oct 2022 03:06:19 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:12:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:12:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:12:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1f0ecb08923b99bef3f82c2e88603bb53e3ed084c13252275c05039cc279c158`  
		Last Modified: Tue, 25 Oct 2022 03:11:15 GMT  
		Size: 52.5 MB (52547473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b399c5eb53b4c35fa33682a82d73bdc4b096cd78ae95fe36c4ed81d18f6849`  
		Last Modified: Tue, 25 Oct 2022 06:19:02 GMT  
		Size: 5.1 MB (5072235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ccdd06393cd3873a3cc8b9cbe170a2032fd61d1d545b7045b649faf2f4e732`  
		Last Modified: Tue, 25 Oct 2022 06:19:02 GMT  
		Size: 10.6 MB (10574279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aafe0e287af4e488dcda51195e4eb1ae1386e3265989c457172f32f6357bf26`  
		Last Modified: Tue, 25 Oct 2022 06:19:28 GMT  
		Size: 52.3 MB (52322157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:50a85a985b089ddf5972b836da6a0053b066b489827aa55bac5f7bec2bf93ffa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.7 MB (115701649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30f987ffe03e99e4f18811a3ed9c6b544fa00393058f4ef2abb83df5bc1d7673`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:28 GMT
ADD file:47a3f2948af18c39686ca59a88a439c25edaf286064d3a2ccc5dab47fee2fc52 in / 
# Tue, 04 Oct 2022 23:58:29 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:32:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:32:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:32:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e19342fb46cabf6147aec1d1c6af1f3a82736530cf3b067835fc8a09da092ce3`  
		Last Modified: Wed, 05 Oct 2022 00:04:36 GMT  
		Size: 50.2 MB (50209087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a49f93f990f17337480b5bdf526a6bb48d1ae63bd17f54be17cd2f6ebba4de7d`  
		Last Modified: Wed, 05 Oct 2022 00:53:28 GMT  
		Size: 4.9 MB (4931366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3989be0d7ed2f72fae0310039043f6ba76c24a45f9ec9689697ebd932845cc8`  
		Last Modified: Wed, 05 Oct 2022 00:53:28 GMT  
		Size: 10.2 MB (10217872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6487a2e4236617393a6184f0f89a360d295ab118da2ea4ad48fa8645ae211755`  
		Last Modified: Wed, 05 Oct 2022 00:53:57 GMT  
		Size: 50.3 MB (50343324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:8b048c050c2a3ff92ba38fbbe2ceb6d4523c5c2d90dc3ef032dbe78ce741b7c5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124411636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c203e5804baca6a5e5ee110aa8b5c855e1af7aa5b84d282751a6ee78a938f3e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:45:55 GMT
ADD file:b16745ece8ef84c028d7e9ac4bf026ac64f885d4170bfcc9d435f237144a1b99 in / 
# Tue, 25 Oct 2022 05:45:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:58:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:58:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 07:59:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8e1d92e7d04d2a9a9880cb45dc3c32c2805912cd86abed96d0ada3ff28748205`  
		Last Modified: Tue, 25 Oct 2022 05:48:40 GMT  
		Size: 53.7 MB (53701966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66eadbf427bb41b3e329a95935c65b09c6d3b7a9c2fa8e08417e497df02ed996`  
		Last Modified: Tue, 25 Oct 2022 08:30:22 GMT  
		Size: 5.2 MB (5151506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9731f4e3bc3680179c10cece663cf0cfe0488918d6795406f4b76f07b787de`  
		Last Modified: Tue, 25 Oct 2022 08:30:22 GMT  
		Size: 10.9 MB (10874174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d337cb12fd7c6fe341850cd38e880f1806d49a65832c9804b06d00f9032382e0`  
		Last Modified: Tue, 25 Oct 2022 08:30:42 GMT  
		Size: 54.7 MB (54683990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:af3f07f28271542b5cad16677fb8b3eca0cf0897adac022669fd5d2aabbf004d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.1 MB (128067777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41c2e7cc3bce85c55d7b854c187796f854d5d152784c6759eaa5aa5c6dbdc665`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:22:19 GMT
ADD file:aa26f69b37c3e144d08e17bb9be7302ec89ae0579121c874a35f336d7077fd3b in / 
# Tue, 25 Oct 2022 02:22:19 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:15:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:15:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 05:15:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8caf426a2703f99fb0be4b03411ecaa580d102f7c47ef43b422b6d7c13c380e2`  
		Last Modified: Tue, 25 Oct 2022 02:27:54 GMT  
		Size: 56.0 MB (56023960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b92a2ff5c72653a0679aa7f5e2bc695011c0a71faa424229e560957d204dab`  
		Last Modified: Tue, 25 Oct 2022 05:27:37 GMT  
		Size: 5.1 MB (5086887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6856a3002e686ceb6d48d078731366f576ed3adcb73bd49dcb300057732904`  
		Last Modified: Tue, 25 Oct 2022 05:27:38 GMT  
		Size: 11.0 MB (11032526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e88080d3b5ba1edc8623a97d068bd040dfb89f2bc7bdfc0984d11fc35ff5885`  
		Last Modified: Tue, 25 Oct 2022 05:28:00 GMT  
		Size: 55.9 MB (55924404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:a1acaa6746ce03d5ac1c9c184b9983adf517c0cc252294f448e9e9c51580b9c7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122150421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfa73d3a5551fa701da480cd6d0b3d216e9aace1ea0d1de8201cd9fe13f05ce5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:09:48 GMT
ADD file:ca40db2df3dbc600910b8cd139c564cf5b8bd6c1a06cc517cae2c1c05cff6dde in / 
# Wed, 05 Oct 2022 00:09:51 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:11:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:12:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:14:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:25bcd35faf05f859c3077f0e2e7010d24e56cdcfb77efbdeda236e47dc08e14a`  
		Last Modified: Wed, 05 Oct 2022 00:17:52 GMT  
		Size: 53.3 MB (53265834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c44f381e4f9f5eb923a09cbd49bc86d3d36121137c1e063d30d73af518bf0f86`  
		Last Modified: Wed, 05 Oct 2022 01:32:02 GMT  
		Size: 4.9 MB (4918634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59260097f47eb21e87461a2a98c76f46372dd316b878bbd3d4d9c51cc28a62b7`  
		Last Modified: Wed, 05 Oct 2022 01:32:04 GMT  
		Size: 10.7 MB (10661237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f8a68e1316af16785650ca91231ed6373810fcdaff8fb5bec9f58e1ccc2a32`  
		Last Modified: Wed, 05 Oct 2022 01:32:53 GMT  
		Size: 53.3 MB (53304716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:aa6dce1df8020e1e65a5969cd4d256313e3e6bf82526d3774527163c0d3d6b6f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134828389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd50ae9ad837d99d2a9f89b2818813787249d3ea2cd98a78affb4ac0a45caa6d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:13:28 GMT
ADD file:c01a6cc4222fbeeda5c2d679c5b355539880a02c792c64861eb17b81a3678f45 in / 
# Tue, 25 Oct 2022 03:13:31 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:13:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:14:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:14:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ee5a342763ed1d31bef8cebe9f4cc5dd6d427f630da679a87da0427be7b22e3d`  
		Last Modified: Tue, 25 Oct 2022 03:18:52 GMT  
		Size: 58.9 MB (58916374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a4727f39cbcb19b39abdbd847eeceed842ef65f8514372024c48b913bc951a`  
		Last Modified: Tue, 25 Oct 2022 06:49:00 GMT  
		Size: 5.4 MB (5414507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe601e6c8a1ec9c69c49c65a53339202a65cea9d4f01d161fb34905c06a4a99`  
		Last Modified: Tue, 25 Oct 2022 06:49:01 GMT  
		Size: 11.6 MB (11630153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5055e27b58426c2b637b1c8c179e6abe306e3dfb55a9c170c73fb0d581c6cf3e`  
		Last Modified: Tue, 25 Oct 2022 06:49:31 GMT  
		Size: 58.9 MB (58867355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:eba01f860d7d3264a146b7ec7242b3002fd04f91a81d12f89260377ac201f374
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.3 MB (123250140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d21933a18810ed510258d911e9f0408303556697f423746d2ecbcdb6d9df700`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:14:24 GMT
ADD file:06f15d8a3c04752d271a052e820fb13fcdb76f0d18f6c9afb6e70391d10348ec in / 
# Tue, 25 Oct 2022 01:14:27 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:31:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:31:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 02:31:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a556186e8bea4ba9925d0c17bea2c12bfbb931653cfab1b980036800482cf0ad`  
		Last Modified: Tue, 25 Oct 2022 01:18:39 GMT  
		Size: 53.3 MB (53279106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1e8478a953d3a464d73e36e4032c979725bc79ce0eeb83aca30212de549b90`  
		Last Modified: Tue, 25 Oct 2022 02:49:32 GMT  
		Size: 5.1 MB (5148477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cdbee45ed722bfaf7e9ba90503afa7a0cf17b87fc1bfa1e87cbf49ca6bd7d9`  
		Last Modified: Tue, 25 Oct 2022 02:49:33 GMT  
		Size: 10.8 MB (10766704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76aacd12f54fec6c8f627f09641ea144eb6fefeebc8f9fc35de80c3e3ab11af7`  
		Last Modified: Tue, 25 Oct 2022 02:49:48 GMT  
		Size: 54.1 MB (54055853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:buster`

```console
$ docker pull buildpack-deps@sha256:23c324efadf9febfe2d46da3a96f2076678e8ad195ca7e84d328efd29ada237e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:buster` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:9bc85b7b437bfb4388f7160a92e96c24ff5591134dfcc45b5ce939c25923b81a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.6 MB (312646449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f94fc706b3e93d2101993d24cf5d6da5fb762d5475a4b62407e77f8a58088e35`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:56:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:57:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:58:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6315e893372434bf09990677f857fdd026ba0abdd98d435decc2ec5742cee4`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 7.9 MB (7857339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad12dd0da3ea9c59f4c4fc53d6a204e11e2930b9dc4143376024ed8fa5c71bb`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 10.0 MB (9998384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a0ceb4387f59959418bd2da17176107c9ce0ea542cf017ce14835999fa8437`  
		Last Modified: Wed, 05 Oct 2022 01:20:41 GMT  
		Size: 51.8 MB (51844142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0ae5ed3318e8db87d129f9c2652dddc78c89f223625a345ec1b7b84149a882`  
		Last Modified: Wed, 05 Oct 2022 01:21:16 GMT  
		Size: 192.5 MB (192505482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:2e18f1ba0b34255fb800df33fe54f2839e518f98e93129aa8fd87bd702595a12
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.5 MB (278453016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:332432940790fb96e3fd3a0b74f46e3a7df64c05ef7f1204784d6612c1896616`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:59:00 GMT
ADD file:b16f07fda9b8beecd7c275565d0ed135fb298c712482766c8f0e40fac932130c in / 
# Tue, 04 Oct 2022 23:59:01 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:34:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:35:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:35:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:37:59 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bba3a5db4dfa403d6e1db947629616e80fb4514e2190e6aa1fb6a2c828c32491`  
		Last Modified: Wed, 05 Oct 2022 00:05:35 GMT  
		Size: 45.9 MB (45914973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0469c30b40a2c26072c228ab2795c38de425870b9ee85d29a32a2f50db3c4f`  
		Last Modified: Wed, 05 Oct 2022 00:55:03 GMT  
		Size: 7.1 MB (7145345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5315d494a34df967f8f4db548d0b40754c70678b9357188c65dc0b9cfee4f7e`  
		Last Modified: Wed, 05 Oct 2022 00:55:03 GMT  
		Size: 9.3 MB (9344666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317e83f2e93982c08cca0dc1dc3456b7bdfa7cdc43011e894195ad828de7550c`  
		Last Modified: Wed, 05 Oct 2022 00:55:25 GMT  
		Size: 47.4 MB (47363676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2771890b0a61f6c6c34e9aa3b58a50e0cf5b1ac46cf3ddcfe77c70fc410d9d16`  
		Last Modified: Wed, 05 Oct 2022 00:56:10 GMT  
		Size: 168.7 MB (168684356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:4a600eea362e0bb4e0778ac365824e178ff6971f0eb2793d531a21927238697d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.2 MB (303229234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e913c5bd9a75ab5fa70ca778c3b9e620e92e01cd05ea666ccd918794ed90efd5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:07 GMT
ADD file:21afa32c0395cc5046d09741d6821d21cfd9b77bce46ebcfc8fd9aca57c73648 in / 
# Tue, 25 Oct 2022 05:46:08 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:00:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:00:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:01:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3ba81f4c3c21f92780061ee116827d64ac4edbcd02b056845c2aaa3097b730ed`  
		Last Modified: Tue, 25 Oct 2022 05:49:24 GMT  
		Size: 49.2 MB (49233280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5909a8b8cad57ca90fe69eaa8b350c722b820753f9caaa1f528f2337a71f38`  
		Last Modified: Tue, 25 Oct 2022 08:31:26 GMT  
		Size: 7.7 MB (7726424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a633475baeae1eb12baa14cc54f130d1e37ea520470ee16bb2dd23d779d08b4b`  
		Last Modified: Tue, 25 Oct 2022 08:31:25 GMT  
		Size: 10.0 MB (10003562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f22a2b8ddcb8bb5d37d3cd14e13998148d107dc8eb1d7c57c3220c1915fd9d1`  
		Last Modified: Tue, 25 Oct 2022 08:31:41 GMT  
		Size: 52.2 MB (52172864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985dd0945ed8d7e2674a61279668f6edeac4dc80a4a6a517fd01736884e37951`  
		Last Modified: Tue, 25 Oct 2022 08:32:08 GMT  
		Size: 184.1 MB (184093104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; 386

```console
$ docker pull buildpack-deps@sha256:986002256185ea6e031552f9961c582f79bc59cfd0480c91dc617e385c631089
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.8 MB (321844428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbf287ecacbd32c06e7567a97fa798639352e1b8ebee00ba2d94c64cebeee1c6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:22:47 GMT
ADD file:7e14d4afa5499129c959c5ae5dc270e2fa04659c2c9b0527094cda3494c02d0f in / 
# Tue, 25 Oct 2022 02:22:47 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:16:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:16:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 05:17:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:18:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76a731c42f665e7334a622f65117ef9389e97a878b7c74bb4a10dfe9cdb296c6`  
		Last Modified: Tue, 25 Oct 2022 02:28:50 GMT  
		Size: 51.2 MB (51207943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee1fc3722feabf994120ab8f7d4abab754206d1ca425b7274ce1db428f7a651`  
		Last Modified: Tue, 25 Oct 2022 05:28:54 GMT  
		Size: 8.0 MB (8025806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2019db6202a77d9f3c2e49a64c766b8b67d4290e0e66e1480fd8c576078914b2`  
		Last Modified: Tue, 25 Oct 2022 05:28:54 GMT  
		Size: 10.1 MB (10128021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79afff7d2fb8bbf10afd83b8f08278ed493a12e50a8262a18a1b3fc227667ec4`  
		Last Modified: Tue, 25 Oct 2022 05:29:13 GMT  
		Size: 53.4 MB (53442950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9206c74214dfb44ab3f4b75a12fcb6bf38c7e04c253e88ff3af265d2e33152f4`  
		Last Modified: Tue, 25 Oct 2022 05:29:47 GMT  
		Size: 199.0 MB (199039708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:buster-curl`

```console
$ docker pull buildpack-deps@sha256:97a9679f1baca57d6622f9e8757d4539e82686724aec4f5b48ba04bf854a9e00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:buster-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:7f3fca26e9b1bb3ec6998a1a523cf586a2367e52c1231cdbe8bb4aaf8e8db8f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68296825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86d0d53a4b39e141ed1bb691a10b424c3dec11acdd8a74caad8dd92781d9be08`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:56:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6315e893372434bf09990677f857fdd026ba0abdd98d435decc2ec5742cee4`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 7.9 MB (7857339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad12dd0da3ea9c59f4c4fc53d6a204e11e2930b9dc4143376024ed8fa5c71bb`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 10.0 MB (9998384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:5cd59ddd6b9c9a97edda3c72bdcad4b5066c14becf62e1671a3d0941e6d67a9b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62404984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d022800d5a11e049d7a055e547960321c510573aabb0a90de07cb297f8f7d306`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:59:00 GMT
ADD file:b16f07fda9b8beecd7c275565d0ed135fb298c712482766c8f0e40fac932130c in / 
# Tue, 04 Oct 2022 23:59:01 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:34:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:35:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:bba3a5db4dfa403d6e1db947629616e80fb4514e2190e6aa1fb6a2c828c32491`  
		Last Modified: Wed, 05 Oct 2022 00:05:35 GMT  
		Size: 45.9 MB (45914973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0469c30b40a2c26072c228ab2795c38de425870b9ee85d29a32a2f50db3c4f`  
		Last Modified: Wed, 05 Oct 2022 00:55:03 GMT  
		Size: 7.1 MB (7145345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5315d494a34df967f8f4db548d0b40754c70678b9357188c65dc0b9cfee4f7e`  
		Last Modified: Wed, 05 Oct 2022 00:55:03 GMT  
		Size: 9.3 MB (9344666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:62e0978b8f23b168926fbaa2c7e965afe1b8c2f9425020b970f07a341589c10d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (66963266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ef5471fe2492bddb3a059378a30108a47836397b595e088e8385b2232a05668`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:07 GMT
ADD file:21afa32c0395cc5046d09741d6821d21cfd9b77bce46ebcfc8fd9aca57c73648 in / 
# Tue, 25 Oct 2022 05:46:08 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:00:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3ba81f4c3c21f92780061ee116827d64ac4edbcd02b056845c2aaa3097b730ed`  
		Last Modified: Tue, 25 Oct 2022 05:49:24 GMT  
		Size: 49.2 MB (49233280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5909a8b8cad57ca90fe69eaa8b350c722b820753f9caaa1f528f2337a71f38`  
		Last Modified: Tue, 25 Oct 2022 08:31:26 GMT  
		Size: 7.7 MB (7726424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a633475baeae1eb12baa14cc54f130d1e37ea520470ee16bb2dd23d779d08b4b`  
		Last Modified: Tue, 25 Oct 2022 08:31:25 GMT  
		Size: 10.0 MB (10003562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:141fff8c2ffcc8259e3a47678ed76429a31d347a408e2f2f0888e736c49898dd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69361770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff4a03bb5b5ce0fe0aa8976c8784fc059747d3be27552c0f8e0fe675b0862c4d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:22:47 GMT
ADD file:7e14d4afa5499129c959c5ae5dc270e2fa04659c2c9b0527094cda3494c02d0f in / 
# Tue, 25 Oct 2022 02:22:47 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:16:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:16:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:76a731c42f665e7334a622f65117ef9389e97a878b7c74bb4a10dfe9cdb296c6`  
		Last Modified: Tue, 25 Oct 2022 02:28:50 GMT  
		Size: 51.2 MB (51207943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee1fc3722feabf994120ab8f7d4abab754206d1ca425b7274ce1db428f7a651`  
		Last Modified: Tue, 25 Oct 2022 05:28:54 GMT  
		Size: 8.0 MB (8025806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2019db6202a77d9f3c2e49a64c766b8b67d4290e0e66e1480fd8c576078914b2`  
		Last Modified: Tue, 25 Oct 2022 05:28:54 GMT  
		Size: 10.1 MB (10128021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:buster-scm`

```console
$ docker pull buildpack-deps@sha256:a590ddff46a58a462abeb4c8d37ca4fcb4d0d2925cdbef377d1b09601e9fa644
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:buster-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:0fc5aaca490caf0a79503055fbc391b8853d761d5a03215be8be60f41e47e8aa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120140967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59e413a2b1e4e2663e043d48670e90c2884b194881af04864d37af34f210e6ce`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:56:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:57:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6315e893372434bf09990677f857fdd026ba0abdd98d435decc2ec5742cee4`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 7.9 MB (7857339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad12dd0da3ea9c59f4c4fc53d6a204e11e2930b9dc4143376024ed8fa5c71bb`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 10.0 MB (9998384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a0ceb4387f59959418bd2da17176107c9ce0ea542cf017ce14835999fa8437`  
		Last Modified: Wed, 05 Oct 2022 01:20:41 GMT  
		Size: 51.8 MB (51844142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1c44d4c649674b9e3e229b526b0a8c64d775b37ca77c49712dab1a29b053322c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109768660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a258170ac7140810e8320dd1407b51e91999966c0044a20c68c66fe1ea0b5f1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:59:00 GMT
ADD file:b16f07fda9b8beecd7c275565d0ed135fb298c712482766c8f0e40fac932130c in / 
# Tue, 04 Oct 2022 23:59:01 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:34:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:35:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:35:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bba3a5db4dfa403d6e1db947629616e80fb4514e2190e6aa1fb6a2c828c32491`  
		Last Modified: Wed, 05 Oct 2022 00:05:35 GMT  
		Size: 45.9 MB (45914973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0469c30b40a2c26072c228ab2795c38de425870b9ee85d29a32a2f50db3c4f`  
		Last Modified: Wed, 05 Oct 2022 00:55:03 GMT  
		Size: 7.1 MB (7145345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5315d494a34df967f8f4db548d0b40754c70678b9357188c65dc0b9cfee4f7e`  
		Last Modified: Wed, 05 Oct 2022 00:55:03 GMT  
		Size: 9.3 MB (9344666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317e83f2e93982c08cca0dc1dc3456b7bdfa7cdc43011e894195ad828de7550c`  
		Last Modified: Wed, 05 Oct 2022 00:55:25 GMT  
		Size: 47.4 MB (47363676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:9f6e569fb46b186c92f83439bc018e32747d464f7d9b2d8807c7416ef1b64a75
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.1 MB (119136130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:609ea79261cd59e82ef55f8c7c01da32dcad5b2ba53f83090793c43285265b76`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:07 GMT
ADD file:21afa32c0395cc5046d09741d6821d21cfd9b77bce46ebcfc8fd9aca57c73648 in / 
# Tue, 25 Oct 2022 05:46:08 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:00:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:00:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3ba81f4c3c21f92780061ee116827d64ac4edbcd02b056845c2aaa3097b730ed`  
		Last Modified: Tue, 25 Oct 2022 05:49:24 GMT  
		Size: 49.2 MB (49233280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5909a8b8cad57ca90fe69eaa8b350c722b820753f9caaa1f528f2337a71f38`  
		Last Modified: Tue, 25 Oct 2022 08:31:26 GMT  
		Size: 7.7 MB (7726424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a633475baeae1eb12baa14cc54f130d1e37ea520470ee16bb2dd23d779d08b4b`  
		Last Modified: Tue, 25 Oct 2022 08:31:25 GMT  
		Size: 10.0 MB (10003562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f22a2b8ddcb8bb5d37d3cd14e13998148d107dc8eb1d7c57c3220c1915fd9d1`  
		Last Modified: Tue, 25 Oct 2022 08:31:41 GMT  
		Size: 52.2 MB (52172864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:72528f8ffef6e01ca828a63747681ae454b493b4005d786376fa35f432a95d55
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.8 MB (122804720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81b4069d89bb74ef0eca45c2e785bf7ba4d17172c93d68cd25f65cbd17f76d46`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:22:47 GMT
ADD file:7e14d4afa5499129c959c5ae5dc270e2fa04659c2c9b0527094cda3494c02d0f in / 
# Tue, 25 Oct 2022 02:22:47 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:16:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:16:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 05:17:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76a731c42f665e7334a622f65117ef9389e97a878b7c74bb4a10dfe9cdb296c6`  
		Last Modified: Tue, 25 Oct 2022 02:28:50 GMT  
		Size: 51.2 MB (51207943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee1fc3722feabf994120ab8f7d4abab754206d1ca425b7274ce1db428f7a651`  
		Last Modified: Tue, 25 Oct 2022 05:28:54 GMT  
		Size: 8.0 MB (8025806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2019db6202a77d9f3c2e49a64c766b8b67d4290e0e66e1480fd8c576078914b2`  
		Last Modified: Tue, 25 Oct 2022 05:28:54 GMT  
		Size: 10.1 MB (10128021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79afff7d2fb8bbf10afd83b8f08278ed493a12e50a8262a18a1b3fc227667ec4`  
		Last Modified: Tue, 25 Oct 2022 05:29:13 GMT  
		Size: 53.4 MB (53442950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:curl`

```console
$ docker pull buildpack-deps@sha256:f0bc68399bc76e1d562de8399f0fb2990e3bd6cc04aab46bb2eb6d789905caef
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
$ docker pull buildpack-deps@sha256:cb9a3f7bd43628db1b3695a6e7b28d561bf4df306ab1f63a0c232397690bf2dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.1 MB (71086032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1e2c1abde86fb7ff272adfa86162471d1bfa52060a0dec82087fecebdcb31e5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:27 GMT
ADD file:d1268789456d2cdace6e50149e60404ad5a849b7c61e8fc8bc7b6e0eb6eeb7ca in / 
# Tue, 04 Oct 2022 23:26:27 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:54:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:55:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f606d8928ed378229f2460b94b504cca239fb906efc57acbdf9340bd298d5ddf`  
		Last Modified: Tue, 04 Oct 2022 23:30:27 GMT  
		Size: 55.0 MB (55046248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47db815c6a4547dc224b75222193cb1851cf529d2cbdf26f854b9bbf97099b98`  
		Last Modified: Wed, 05 Oct 2022 01:19:13 GMT  
		Size: 5.2 MB (5163279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf48494000001a037b72870d2a6a2536f9da8bc5d1ceddd72d79f4a51fe7a60e`  
		Last Modified: Wed, 05 Oct 2022 01:19:13 GMT  
		Size: 10.9 MB (10876505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:c4307444787732144220d75296f55023fa4114b856df149c28e78559c50359d4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.2 MB (68193987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e39186554e8bc668aa17c37b50cd6803d4a408a41ad404ba37b3e10e2ed96267`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:06:19 GMT
ADD file:b314b98654e8532fd10a08a172ea5c3edb7d7a36c7faf85d06d14be12f7b83ef in / 
# Tue, 25 Oct 2022 03:06:19 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:12:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:12:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1f0ecb08923b99bef3f82c2e88603bb53e3ed084c13252275c05039cc279c158`  
		Last Modified: Tue, 25 Oct 2022 03:11:15 GMT  
		Size: 52.5 MB (52547473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b399c5eb53b4c35fa33682a82d73bdc4b096cd78ae95fe36c4ed81d18f6849`  
		Last Modified: Tue, 25 Oct 2022 06:19:02 GMT  
		Size: 5.1 MB (5072235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ccdd06393cd3873a3cc8b9cbe170a2032fd61d1d545b7045b649faf2f4e732`  
		Last Modified: Tue, 25 Oct 2022 06:19:02 GMT  
		Size: 10.6 MB (10574279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:fa161c8e7935e0810bcd3ca45a9746cf6e3fdc6025c5362e8bc2648f7fae6239
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65358325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b86ef37d02c678f38add592f5f88e1f266a851783e8f323eb1837a5ee7352ac7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:28 GMT
ADD file:47a3f2948af18c39686ca59a88a439c25edaf286064d3a2ccc5dab47fee2fc52 in / 
# Tue, 04 Oct 2022 23:58:29 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:32:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:32:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e19342fb46cabf6147aec1d1c6af1f3a82736530cf3b067835fc8a09da092ce3`  
		Last Modified: Wed, 05 Oct 2022 00:04:36 GMT  
		Size: 50.2 MB (50209087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a49f93f990f17337480b5bdf526a6bb48d1ae63bd17f54be17cd2f6ebba4de7d`  
		Last Modified: Wed, 05 Oct 2022 00:53:28 GMT  
		Size: 4.9 MB (4931366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3989be0d7ed2f72fae0310039043f6ba76c24a45f9ec9689697ebd932845cc8`  
		Last Modified: Wed, 05 Oct 2022 00:53:28 GMT  
		Size: 10.2 MB (10217872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:bc7e9978ee6d44bb721af5cba9e40ee69de8d269140ec556a0c40cbeee8979bb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.7 MB (69727646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c88b9fd10ad56e7d5bac1e3cb67021a7765c589e6e7d144f46d1c76d2811413d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:45:55 GMT
ADD file:b16745ece8ef84c028d7e9ac4bf026ac64f885d4170bfcc9d435f237144a1b99 in / 
# Tue, 25 Oct 2022 05:45:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:58:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:58:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8e1d92e7d04d2a9a9880cb45dc3c32c2805912cd86abed96d0ada3ff28748205`  
		Last Modified: Tue, 25 Oct 2022 05:48:40 GMT  
		Size: 53.7 MB (53701966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66eadbf427bb41b3e329a95935c65b09c6d3b7a9c2fa8e08417e497df02ed996`  
		Last Modified: Tue, 25 Oct 2022 08:30:22 GMT  
		Size: 5.2 MB (5151506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9731f4e3bc3680179c10cece663cf0cfe0488918d6795406f4b76f07b787de`  
		Last Modified: Tue, 25 Oct 2022 08:30:22 GMT  
		Size: 10.9 MB (10874174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:bf477637cd09b9031cd034fff22d013e90a3101df053d80729d928601fb7c14a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.1 MB (72143373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b4b083b9d9929246daf9a5fe0622f9a1e88bfb618b352807b23b97d75ff5a38`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:22:19 GMT
ADD file:aa26f69b37c3e144d08e17bb9be7302ec89ae0579121c874a35f336d7077fd3b in / 
# Tue, 25 Oct 2022 02:22:19 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:15:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:15:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8caf426a2703f99fb0be4b03411ecaa580d102f7c47ef43b422b6d7c13c380e2`  
		Last Modified: Tue, 25 Oct 2022 02:27:54 GMT  
		Size: 56.0 MB (56023960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b92a2ff5c72653a0679aa7f5e2bc695011c0a71faa424229e560957d204dab`  
		Last Modified: Tue, 25 Oct 2022 05:27:37 GMT  
		Size: 5.1 MB (5086887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6856a3002e686ceb6d48d078731366f576ed3adcb73bd49dcb300057732904`  
		Last Modified: Tue, 25 Oct 2022 05:27:38 GMT  
		Size: 11.0 MB (11032526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:668f750c6d59a65e45714ebe9fd3c02e2b07e166cf39df660a4b93a59449e9ad
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68845705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e70040762c35b1ea015572f262495cddda025b3d915f9fbfa15e0a0f6b02130`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:09:48 GMT
ADD file:ca40db2df3dbc600910b8cd139c564cf5b8bd6c1a06cc517cae2c1c05cff6dde in / 
# Wed, 05 Oct 2022 00:09:51 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:11:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:12:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:25bcd35faf05f859c3077f0e2e7010d24e56cdcfb77efbdeda236e47dc08e14a`  
		Last Modified: Wed, 05 Oct 2022 00:17:52 GMT  
		Size: 53.3 MB (53265834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c44f381e4f9f5eb923a09cbd49bc86d3d36121137c1e063d30d73af518bf0f86`  
		Last Modified: Wed, 05 Oct 2022 01:32:02 GMT  
		Size: 4.9 MB (4918634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59260097f47eb21e87461a2a98c76f46372dd316b878bbd3d4d9c51cc28a62b7`  
		Last Modified: Wed, 05 Oct 2022 01:32:04 GMT  
		Size: 10.7 MB (10661237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:469e7517e99c19831cea091b8ba496389124880b75d31d2718cc6c1999060b8e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.0 MB (75961034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5cb6ede5f74b2e5a7f231d8ef2d1f5728c8b419020b8d7640b6aaef3bdfe00e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:13:28 GMT
ADD file:c01a6cc4222fbeeda5c2d679c5b355539880a02c792c64861eb17b81a3678f45 in / 
# Tue, 25 Oct 2022 03:13:31 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:13:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:14:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ee5a342763ed1d31bef8cebe9f4cc5dd6d427f630da679a87da0427be7b22e3d`  
		Last Modified: Tue, 25 Oct 2022 03:18:52 GMT  
		Size: 58.9 MB (58916374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a4727f39cbcb19b39abdbd847eeceed842ef65f8514372024c48b913bc951a`  
		Last Modified: Tue, 25 Oct 2022 06:49:00 GMT  
		Size: 5.4 MB (5414507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe601e6c8a1ec9c69c49c65a53339202a65cea9d4f01d161fb34905c06a4a99`  
		Last Modified: Tue, 25 Oct 2022 06:49:01 GMT  
		Size: 11.6 MB (11630153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:809d9d381f46cf97b2154255bf1ab72c6c7126ca14bef3939630abde9638783d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69194287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14cce275c18bfdc19a1e7f27773751920f1a720c0ccd64c54a8ace1b33e0cf31`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:14:24 GMT
ADD file:06f15d8a3c04752d271a052e820fb13fcdb76f0d18f6c9afb6e70391d10348ec in / 
# Tue, 25 Oct 2022 01:14:27 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:31:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:31:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a556186e8bea4ba9925d0c17bea2c12bfbb931653cfab1b980036800482cf0ad`  
		Last Modified: Tue, 25 Oct 2022 01:18:39 GMT  
		Size: 53.3 MB (53279106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1e8478a953d3a464d73e36e4032c979725bc79ce0eeb83aca30212de549b90`  
		Last Modified: Tue, 25 Oct 2022 02:49:32 GMT  
		Size: 5.1 MB (5148477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cdbee45ed722bfaf7e9ba90503afa7a0cf17b87fc1bfa1e87cbf49ca6bd7d9`  
		Last Modified: Tue, 25 Oct 2022 02:49:33 GMT  
		Size: 10.8 MB (10766704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:focal`

```console
$ docker pull buildpack-deps@sha256:17448e01180652e618c3052d3fe2360d3a99593b4e504591ec5e9deac35f0712
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
$ docker pull buildpack-deps@sha256:df1cb039c302258fc7aeb3d09633c18b7c2330f4df5febec069e06b01e7a631e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.8 MB (245760922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff0be4edc3bf215849f05ed174892ef853e12761ee649124bde965c0d9fa7789`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:04:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:04:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:05:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:08:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7215646fa628a9c18e31f7ea7321ae4140b44d69995ec4cdf3968cbce9a5c0b4`  
		Last Modified: Wed, 05 Oct 2022 01:23:38 GMT  
		Size: 7.7 MB (7747231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6c7ee6250b02a6cf0a3a3080d082e4ce4f858e2749921bc2623c896c487897`  
		Last Modified: Wed, 05 Oct 2022 01:23:37 GMT  
		Size: 3.6 MB (3624405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927ce100b3517cefcb05b92b71a8c91e9881466e25f273c9ce8b59ade42ef3a3`  
		Last Modified: Wed, 05 Oct 2022 01:23:58 GMT  
		Size: 60.7 MB (60738241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2912631d641854e38546e76428eb259b076e4d737fc5ef8a27d790b7f6b5d85`  
		Last Modified: Wed, 05 Oct 2022 01:24:28 GMT  
		Size: 145.1 MB (145076594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:8e9c5845425de993e8a14f762a07ba75002b29b1a385b14ce0884f9d3055d449
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.8 MB (211802501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56f88acbe9e38aa875d1ccc4954298f23f43d45f8a3d373c5f13c22f1ba9223f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:44 GMT
ADD file:75870468a948359044fa3df6c07c80badfea3dcde4823d41a19285436c40cf76 in / 
# Wed, 05 Oct 2022 00:13:44 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:42:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:42:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:43:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:44:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e679d63f382033c15f8f921851bd71fb8a85a432c0a7a612bbef16e989075145`  
		Last Modified: Wed, 05 Oct 2022 00:15:44 GMT  
		Size: 24.6 MB (24590092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8314cec2c7a441a36532dc89979b531fd7dab365416e8d4f077f16c6322a222`  
		Last Modified: Wed, 05 Oct 2022 00:59:17 GMT  
		Size: 6.7 MB (6740274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b75361ec0073f1728c7bbc9fbf5e55f5ffc978176453aaccd3f3097a710904`  
		Last Modified: Wed, 05 Oct 2022 00:59:16 GMT  
		Size: 3.1 MB (3103607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0cd29b8c09506d2393921adb0cded05dba5f57e529ff475ad92160d2b38c475`  
		Last Modified: Wed, 05 Oct 2022 00:59:45 GMT  
		Size: 55.4 MB (55441138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1062ee353a76044d7056fa8d73eb9cc0e68c08ed4df3ef21e497189a70233c3`  
		Last Modified: Wed, 05 Oct 2022 01:00:24 GMT  
		Size: 121.9 MB (121927390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:445e10a7ae38f20373cd85399fc91f13053769747294e9d0edda602105168041
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.0 MB (235997220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3e5ee77d909660495f56fcdbf233971a6f13e03d21943ea5d5a8ea754e140a3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:09:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:09:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:10:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:13:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f7d42f1359bed862a992a062b3c7cf025e6bf6625dc1ca56ae2c66d7250fba`  
		Last Modified: Tue, 25 Oct 2022 08:34:12 GMT  
		Size: 7.6 MB (7616212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc75acb9c1e02b10ddc3966608ccbac66c6fd9eeb3bff80797f9983f268a9b1a`  
		Last Modified: Tue, 25 Oct 2022 08:34:12 GMT  
		Size: 3.6 MB (3617606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d21db26b13141f20e7cce995a63f8234838277895d2d6d0e2ec4f35e659c78`  
		Last Modified: Tue, 25 Oct 2022 08:34:33 GMT  
		Size: 60.8 MB (60807384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de20e53c6129f32162fa091a310f594b29ebc675880357219b832913b9aa05b`  
		Last Modified: Tue, 25 Oct 2022 08:34:58 GMT  
		Size: 136.8 MB (136760020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:32c07eb6326ad1e49be450e350b8b21f2125e3ff69930bb973b7e82c886d2f12
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.6 MB (269600630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d09b001b9596b00fd30464d8345d01c8e29cc965f6afc931f6f78201fbac9c8c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:47 GMT
ADD file:013ddcea49540903962069a03762fe471452e8cf00bafeb530724940405797e1 in / 
# Tue, 25 Oct 2022 03:25:49 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:27:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:27:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:29:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:32:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:42e5f4d60d38e5070be91d6965be1cff1294e6dc275038002dc2ef1812233b0e`  
		Last Modified: Tue, 25 Oct 2022 03:27:44 GMT  
		Size: 33.3 MB (33300542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa48197ece6cedfce46328b98e2bd3ffa7f116e92dc0cd9aba21390a5edf11f`  
		Last Modified: Tue, 25 Oct 2022 06:54:02 GMT  
		Size: 8.7 MB (8705088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b91159ec91712ffe519d3e9624103d9ec7b58e6b1959cad0b77145851e14fc55`  
		Last Modified: Tue, 25 Oct 2022 06:54:01 GMT  
		Size: 4.5 MB (4486836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c68813dea6733b577ebd8f432367b30fab9f0639692bc2e99d633f9347aff6`  
		Last Modified: Tue, 25 Oct 2022 06:54:33 GMT  
		Size: 69.5 MB (69528310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f928b500f12d32eab804a83c4abf92c24bbba3f2da97a4be3a6502f4a8736507`  
		Last Modified: Tue, 25 Oct 2022 06:55:25 GMT  
		Size: 153.6 MB (153579854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:742a98177295e32b0bc88d6a1e64e2ff9abd71c350bfc3357830f4634a650bae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.4 MB (226379572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3144900fdfaa2b4486324df2ecd5a82c8f3e7987f46e44589b8e88418ffed7c5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:11 GMT
ADD file:c657b467ecb15f1f4a49a5f04a525f38924750c8187c9ef9f0b886d0264e21f1 in / 
# Tue, 25 Oct 2022 01:23:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:37:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:37:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 02:38:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:40:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a63328f08dbd14148b5ffe154c18846ead48e759779d007b78ec3fb19f5f43a5`  
		Last Modified: Tue, 25 Oct 2022 01:24:36 GMT  
		Size: 27.0 MB (27016028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc7f4256f9365e6546f5def4594e750767ee106712ba11997c58b0e9b15ab10a`  
		Last Modified: Tue, 25 Oct 2022 02:52:05 GMT  
		Size: 7.4 MB (7390068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c49cddcfee6d6315b4a734cc802ff8d05a8ecb16654aeca9cbd0076b7dec22f`  
		Last Modified: Tue, 25 Oct 2022 02:52:04 GMT  
		Size: 3.5 MB (3542342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8b09e3088369fc4b7c4afe1c6fa3627b4a08b7f6388e1e455d9bbb75dbe837`  
		Last Modified: Tue, 25 Oct 2022 02:52:20 GMT  
		Size: 60.0 MB (60019048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:182b0410bb16e1bb8d9c66620b8886fe5f6f64897e68159d3247d1ef9d1686a5`  
		Last Modified: Tue, 25 Oct 2022 02:52:43 GMT  
		Size: 128.4 MB (128412086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:focal-curl`

```console
$ docker pull buildpack-deps@sha256:26c49a9dc3d707e42cd1c397e82457dfe3a7e634512d308f107ac3ce2fbb8e11
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
$ docker pull buildpack-deps@sha256:577ab5375346239a411e7b8a20882febf76564a20092492c60089c9614bd58fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.9 MB (39946087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac3978effc4af1fb7f140324ee1b2ef790c7b87608d8633f6099ac4a442193e0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:04:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:04:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7215646fa628a9c18e31f7ea7321ae4140b44d69995ec4cdf3968cbce9a5c0b4`  
		Last Modified: Wed, 05 Oct 2022 01:23:38 GMT  
		Size: 7.7 MB (7747231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6c7ee6250b02a6cf0a3a3080d082e4ce4f858e2749921bc2623c896c487897`  
		Last Modified: Wed, 05 Oct 2022 01:23:37 GMT  
		Size: 3.6 MB (3624405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:8b15c3f4b12c531ad54a4129ad38bc19cb166573ec4213563fc6bf9ee949f5dd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34433973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3679946ffe22fbdc937f477ccad2f1008636611a792de1cc56c09bc3c310d8e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:44 GMT
ADD file:75870468a948359044fa3df6c07c80badfea3dcde4823d41a19285436c40cf76 in / 
# Wed, 05 Oct 2022 00:13:44 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:42:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:42:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e679d63f382033c15f8f921851bd71fb8a85a432c0a7a612bbef16e989075145`  
		Last Modified: Wed, 05 Oct 2022 00:15:44 GMT  
		Size: 24.6 MB (24590092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8314cec2c7a441a36532dc89979b531fd7dab365416e8d4f077f16c6322a222`  
		Last Modified: Wed, 05 Oct 2022 00:59:17 GMT  
		Size: 6.7 MB (6740274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b75361ec0073f1728c7bbc9fbf5e55f5ffc978176453aaccd3f3097a710904`  
		Last Modified: Wed, 05 Oct 2022 00:59:16 GMT  
		Size: 3.1 MB (3103607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:24ebe2372b2d4d6605c25b48eb53d26516e00fd2f83265e47a8412192928063b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.4 MB (38429816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bb123f8970cfe7554a7c140d5f8ef986976f115ef6e59c08649ff0a4772a7b9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:09:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:09:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f7d42f1359bed862a992a062b3c7cf025e6bf6625dc1ca56ae2c66d7250fba`  
		Last Modified: Tue, 25 Oct 2022 08:34:12 GMT  
		Size: 7.6 MB (7616212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc75acb9c1e02b10ddc3966608ccbac66c6fd9eeb3bff80797f9983f268a9b1a`  
		Last Modified: Tue, 25 Oct 2022 08:34:12 GMT  
		Size: 3.6 MB (3617606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:403b348e50e731cf4a159fec7726249774627b7984d345dd0e4bb9f472515693
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46492466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b086a827e90970916ae80203e8045e5d422fdac19df4dd7e561d8f844aaf5b96`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:47 GMT
ADD file:013ddcea49540903962069a03762fe471452e8cf00bafeb530724940405797e1 in / 
# Tue, 25 Oct 2022 03:25:49 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:27:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:27:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:42e5f4d60d38e5070be91d6965be1cff1294e6dc275038002dc2ef1812233b0e`  
		Last Modified: Tue, 25 Oct 2022 03:27:44 GMT  
		Size: 33.3 MB (33300542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa48197ece6cedfce46328b98e2bd3ffa7f116e92dc0cd9aba21390a5edf11f`  
		Last Modified: Tue, 25 Oct 2022 06:54:02 GMT  
		Size: 8.7 MB (8705088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b91159ec91712ffe519d3e9624103d9ec7b58e6b1959cad0b77145851e14fc55`  
		Last Modified: Tue, 25 Oct 2022 06:54:01 GMT  
		Size: 4.5 MB (4486836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:03f6b7e0468f3a039213527067a008db1cef213244a75d3406a175aa2d68b215
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34113041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:629e46285cd96bbf2061784773e791fccde26297e92c9cf51561f276b3c6fc5c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:12:13 GMT
ADD file:8c408c11e1eeed71fdd784404ddf9ac52b700161e6187e2313c2751d756e3442 in / 
# Wed, 05 Oct 2022 00:12:14 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:43:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:43:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:edcdeceb0859700b9f2e87516c30c0049092e29666696c30e6b862e0df3d4961`  
		Last Modified: Wed, 05 Oct 2022 00:29:16 GMT  
		Size: 24.2 MB (24242839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750231dc28469e93ce7c6e7d14be0b30332503e15a9a7516729ab0815bbeb749`  
		Last Modified: Wed, 05 Oct 2022 03:42:06 GMT  
		Size: 6.7 MB (6725280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3455cf9ca9db352ee4e1bdf9c1bd8bd85713203a5b2ae128f9a7d02af28fea50`  
		Last Modified: Wed, 05 Oct 2022 03:42:00 GMT  
		Size: 3.1 MB (3144922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:1a57b03716bdc4d36ffbc98cfc91f6bcf59d28fd7d79b1b189bfc0d6e8aeeeb2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37948438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45eb95eb88b1bfec442d1a02a64ad20f4424239eb7f44b117ae092061619489d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:11 GMT
ADD file:c657b467ecb15f1f4a49a5f04a525f38924750c8187c9ef9f0b886d0264e21f1 in / 
# Tue, 25 Oct 2022 01:23:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:37:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:37:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a63328f08dbd14148b5ffe154c18846ead48e759779d007b78ec3fb19f5f43a5`  
		Last Modified: Tue, 25 Oct 2022 01:24:36 GMT  
		Size: 27.0 MB (27016028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc7f4256f9365e6546f5def4594e750767ee106712ba11997c58b0e9b15ab10a`  
		Last Modified: Tue, 25 Oct 2022 02:52:05 GMT  
		Size: 7.4 MB (7390068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c49cddcfee6d6315b4a734cc802ff8d05a8ecb16654aeca9cbd0076b7dec22f`  
		Last Modified: Tue, 25 Oct 2022 02:52:04 GMT  
		Size: 3.5 MB (3542342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:focal-scm`

```console
$ docker pull buildpack-deps@sha256:aa83529c20e9637d81c8bb79ec8042bb08701d8e0aeb6700ce4bceddb07c2155
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
$ docker pull buildpack-deps@sha256:3fbf9b728805f4855a1e1714abd1122f590819c3c940af6add1e74b6edb1a583
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.7 MB (100684328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:556eaf86e2c531f983516419b73441c5850909052e50ab552d75a9d7b29130a5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:04:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:04:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:05:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7215646fa628a9c18e31f7ea7321ae4140b44d69995ec4cdf3968cbce9a5c0b4`  
		Last Modified: Wed, 05 Oct 2022 01:23:38 GMT  
		Size: 7.7 MB (7747231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6c7ee6250b02a6cf0a3a3080d082e4ce4f858e2749921bc2623c896c487897`  
		Last Modified: Wed, 05 Oct 2022 01:23:37 GMT  
		Size: 3.6 MB (3624405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927ce100b3517cefcb05b92b71a8c91e9881466e25f273c9ce8b59ade42ef3a3`  
		Last Modified: Wed, 05 Oct 2022 01:23:58 GMT  
		Size: 60.7 MB (60738241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ea745c791fe0fd9b6b7bf04130cdc270995b03279f2c411722ff840cd212ead9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.9 MB (89875111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddd42e22b4a80d23d5304ea494d56e753af1132c2869050e028ca61cc3f46c61`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:44 GMT
ADD file:75870468a948359044fa3df6c07c80badfea3dcde4823d41a19285436c40cf76 in / 
# Wed, 05 Oct 2022 00:13:44 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:42:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:42:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:43:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e679d63f382033c15f8f921851bd71fb8a85a432c0a7a612bbef16e989075145`  
		Last Modified: Wed, 05 Oct 2022 00:15:44 GMT  
		Size: 24.6 MB (24590092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8314cec2c7a441a36532dc89979b531fd7dab365416e8d4f077f16c6322a222`  
		Last Modified: Wed, 05 Oct 2022 00:59:17 GMT  
		Size: 6.7 MB (6740274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b75361ec0073f1728c7bbc9fbf5e55f5ffc978176453aaccd3f3097a710904`  
		Last Modified: Wed, 05 Oct 2022 00:59:16 GMT  
		Size: 3.1 MB (3103607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0cd29b8c09506d2393921adb0cded05dba5f57e529ff475ad92160d2b38c475`  
		Last Modified: Wed, 05 Oct 2022 00:59:45 GMT  
		Size: 55.4 MB (55441138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:328e8c05b0f0341747f5871823ad81ae7ac6e958a44be976bcca059cc132912e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99237200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:238b304b5e34bc73bb2557c4303d7a9380f67900d30cac408cfa2c46b7c6b625`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:09:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:09:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:10:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f7d42f1359bed862a992a062b3c7cf025e6bf6625dc1ca56ae2c66d7250fba`  
		Last Modified: Tue, 25 Oct 2022 08:34:12 GMT  
		Size: 7.6 MB (7616212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc75acb9c1e02b10ddc3966608ccbac66c6fd9eeb3bff80797f9983f268a9b1a`  
		Last Modified: Tue, 25 Oct 2022 08:34:12 GMT  
		Size: 3.6 MB (3617606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d21db26b13141f20e7cce995a63f8234838277895d2d6d0e2ec4f35e659c78`  
		Last Modified: Tue, 25 Oct 2022 08:34:33 GMT  
		Size: 60.8 MB (60807384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:0b5156fdea407f78ae8f5dd5a40c70d5686fd01e7a1316d3896a123aa5f2d1e8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (116020776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d728b216db5852c775762c0dbeb7021e76038e61147d6565e4df9ebaf321e554`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:47 GMT
ADD file:013ddcea49540903962069a03762fe471452e8cf00bafeb530724940405797e1 in / 
# Tue, 25 Oct 2022 03:25:49 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:27:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:27:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:29:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:42e5f4d60d38e5070be91d6965be1cff1294e6dc275038002dc2ef1812233b0e`  
		Last Modified: Tue, 25 Oct 2022 03:27:44 GMT  
		Size: 33.3 MB (33300542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa48197ece6cedfce46328b98e2bd3ffa7f116e92dc0cd9aba21390a5edf11f`  
		Last Modified: Tue, 25 Oct 2022 06:54:02 GMT  
		Size: 8.7 MB (8705088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b91159ec91712ffe519d3e9624103d9ec7b58e6b1959cad0b77145851e14fc55`  
		Last Modified: Tue, 25 Oct 2022 06:54:01 GMT  
		Size: 4.5 MB (4486836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c68813dea6733b577ebd8f432367b30fab9f0639692bc2e99d633f9347aff6`  
		Last Modified: Tue, 25 Oct 2022 06:54:33 GMT  
		Size: 69.5 MB (69528310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:6e1c097aaa5b10d603b3ca7af97305eb87efa8eb846c6b08fea8968c3a45fe4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.0 MB (97967486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01cb9f67e31afed0eb376d14ac80a2758ecbb81e5ccb14b069d1b33c9da0399f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:11 GMT
ADD file:c657b467ecb15f1f4a49a5f04a525f38924750c8187c9ef9f0b886d0264e21f1 in / 
# Tue, 25 Oct 2022 01:23:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:37:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:37:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 02:38:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a63328f08dbd14148b5ffe154c18846ead48e759779d007b78ec3fb19f5f43a5`  
		Last Modified: Tue, 25 Oct 2022 01:24:36 GMT  
		Size: 27.0 MB (27016028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc7f4256f9365e6546f5def4594e750767ee106712ba11997c58b0e9b15ab10a`  
		Last Modified: Tue, 25 Oct 2022 02:52:05 GMT  
		Size: 7.4 MB (7390068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c49cddcfee6d6315b4a734cc802ff8d05a8ecb16654aeca9cbd0076b7dec22f`  
		Last Modified: Tue, 25 Oct 2022 02:52:04 GMT  
		Size: 3.5 MB (3542342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8b09e3088369fc4b7c4afe1c6fa3627b4a08b7f6388e1e455d9bbb75dbe837`  
		Last Modified: Tue, 25 Oct 2022 02:52:20 GMT  
		Size: 60.0 MB (60019048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:jammy`

```console
$ docker pull buildpack-deps@sha256:4eb7cafc88b6230a8bed1a8b923d59335967af21faf91b258577a8c692bf4414
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
$ docker pull buildpack-deps@sha256:0a04bf1c7b7015264a105a127d437901cc38216b3e05f80652717d4fbffe1f49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.0 MB (249961758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:799867dd0caf9dc22795fd510b367612d8d37d5e1fc091eebea256c0f1fec1b4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:20 GMT
ADD file:6cd2e13356aa5339c1f2abd3c210a52f6ed74fae05cd61aa09f37b6a4764f65c in / 
# Tue, 04 Oct 2022 23:35:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:09:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:09:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:10:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:13:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cf92e523b49ea3d1fae59f5f082437a5f96c244fda6697995920142ff31d59cf`  
		Last Modified: Tue, 04 Oct 2022 03:04:01 GMT  
		Size: 30.4 MB (30428928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19b9364a5e7fea40b9e9eb4614f0e4533857b602c7fba30362889933ef14298`  
		Last Modified: Wed, 05 Oct 2022 01:24:38 GMT  
		Size: 3.8 MB (3804673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:856d49148d8882ac6866bcbcbaa08bacfe1f0d0d382b73675630ae29d44ae3f2`  
		Last Modified: Wed, 05 Oct 2022 01:24:38 GMT  
		Size: 3.6 MB (3561097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f83374f27f6992ee240fe68ce2e0c2d9db958dc2c9acf1864ef83040cc5387`  
		Last Modified: Wed, 05 Oct 2022 01:24:54 GMT  
		Size: 39.3 MB (39349072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be916118df24025fcea61e45a4784cdf94b7d69e7f9e78290268844a5b3869c`  
		Last Modified: Wed, 05 Oct 2022 01:25:27 GMT  
		Size: 172.8 MB (172817988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:b499e85bc82d56d7053e6deb96cc3a62b6f8b07cea61e9e79aab9378374bfa0f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.6 MB (216595227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99a929445888a8297e1d1e0a72a43df4e15b1986b48a95eab496a572b59cc70d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:57 GMT
ADD file:11e25fc4812528219464289700bb0495bf9298918899103c33d7ef9022690eb0 in / 
# Wed, 05 Oct 2022 00:13:57 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:44:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:45:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:45:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:47:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99b9c73338a7c0dbe41f9fc543fae706650a616453e1e330f870e20916c18a11`  
		Last Modified: Wed, 05 Oct 2022 00:16:02 GMT  
		Size: 27.0 MB (27018632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c337b77409c2e34b5e69df73a11e0ef62cd00b8b23e7d6776235d6491726ac80`  
		Last Modified: Wed, 05 Oct 2022 01:00:37 GMT  
		Size: 3.6 MB (3555370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a1dc485f1a7e2433bb9a4501dac3fb4727fb7708715e743277a50ba4933ca1`  
		Last Modified: Wed, 05 Oct 2022 01:00:37 GMT  
		Size: 3.7 MB (3712768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5595ebdf3f8239b659bdbfc55b5e0a70965f29a4e546cc5efdda43f8e3a4ef76`  
		Last Modified: Wed, 05 Oct 2022 01:01:00 GMT  
		Size: 41.9 MB (41900106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e2ea778678da62e1245bc9a3cc4044027e3903041d44869b3d3d6e1039ce53`  
		Last Modified: Wed, 05 Oct 2022 01:01:41 GMT  
		Size: 140.4 MB (140408351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3062403000f5efd37324066992c8bdb0d10becc4c9f71cda23a5964934215fe1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.3 MB (241329313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b53b6e726046563cf829cd77f37b736f5cac3bc10e64cc69c786796131519ce`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:55:02 GMT
ADD file:515177312f20fb1814b89bfccfe695fa2354bbb6d43fdb6e018bf5b1acc17e9f in / 
# Tue, 25 Oct 2022 05:55:02 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:14:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:14:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:15:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:18:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:56a2caa6b2c66e01954c1a013b37ea359b6e6af8989dbfb958124b6318771af4`  
		Last Modified: Tue, 25 Oct 2022 05:56:14 GMT  
		Size: 28.4 MB (28382489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85c75d65daee139419e66b36968af1443c6839bbfa07f1ff10f41c14059531f8`  
		Last Modified: Tue, 25 Oct 2022 08:35:08 GMT  
		Size: 3.8 MB (3776223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b571e5291fabe657fef93ed4c8e7109c81e0538a58853a65f33d52b4aa5a9f`  
		Last Modified: Tue, 25 Oct 2022 08:35:08 GMT  
		Size: 3.5 MB (3535453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d47a2b6e938e7cf8632d33777355c83ebf1eb36d91c3dc64efc269e15e34ddb`  
		Last Modified: Tue, 25 Oct 2022 08:35:23 GMT  
		Size: 39.2 MB (39236083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8135ee8a3cbc8d92cf867f078f0e7c23411bc10d28f13c3bac60472392514a98`  
		Last Modified: Tue, 25 Oct 2022 08:35:50 GMT  
		Size: 166.4 MB (166399065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:860ed8bcd4c5c4c962c3fdc88871467e7f44c8908c33faea5b7ceea1b6fb14b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.8 MB (271828709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:322a2cb433f862a334e63b1447de75d88df78488ae1653acc45c6d6672584436`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:26:00 GMT
ADD file:766b7743de4ed1a194fc749b7649d245b0cd545b03cc2c81f16a6c15e91c87e7 in / 
# Tue, 25 Oct 2022 03:26:02 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:33:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:33:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:34:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:39:09 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:aa33126e789290559dc146af02cbf168119ed23be1e30fd99fe8572956e50616`  
		Last Modified: Tue, 25 Oct 2022 03:28:08 GMT  
		Size: 35.7 MB (35709401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6373837e7f2a85c7283b43d7d1a07f2541140a0a6287dc704fdf1df6ed09c5e`  
		Last Modified: Tue, 25 Oct 2022 06:55:38 GMT  
		Size: 4.3 MB (4276445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:847050f2ae34b2e1019b09f2bdbac09fd4a3c7efcaf4545aa162094c15b7f016`  
		Last Modified: Tue, 25 Oct 2022 06:55:38 GMT  
		Size: 4.2 MB (4234460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186cf1c98556ab0c2ae47af200ed2f3a8f340ad4cd305379f23619197f2ec188`  
		Last Modified: Tue, 25 Oct 2022 06:56:02 GMT  
		Size: 43.8 MB (43753297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9009bf6240bebccdaeaec57cdd31c0023771a5c2e59499153ff583df56ad8429`  
		Last Modified: Tue, 25 Oct 2022 06:56:57 GMT  
		Size: 183.9 MB (183855106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:883d6acf11862386cb075d26a5eeb067aecd009e926bf289a86848849796adbc
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.9 MB (274910739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ccd65b0e2c99958523b95730fa70b845815fe14d64756c2e1dbf17d4eb51ba0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:14:15 GMT
ADD file:e1fa146cf8e97dd6a2f3ebb2dacba539556ef4a1e87dc53bd745a3cf0ba10aef in / 
# Wed, 05 Oct 2022 00:14:16 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:46:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:47:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 02:51:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:57:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cbeff255552ba792be63b343113968df42de6f599d1372edd4c7346d08dfeace`  
		Last Modified: Wed, 05 Oct 2022 00:31:39 GMT  
		Size: 27.7 MB (27747416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6129e2d138d3d5141f87ef04090f82aeeb874b1d1e3c6f6e94d843cd2447826`  
		Last Modified: Wed, 05 Oct 2022 03:43:29 GMT  
		Size: 3.6 MB (3598134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a1ba2d60715be154c4f520ac4f1ef149f66b921651ab2726a809c14316e55a`  
		Last Modified: Wed, 05 Oct 2022 03:43:27 GMT  
		Size: 3.8 MB (3778196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91414a4a50607595a5e83cc27ee8f8e885ea1d1c43848a3df1487911ae62cc19`  
		Last Modified: Wed, 05 Oct 2022 03:45:48 GMT  
		Size: 42.1 MB (42114477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b2617d47bf73f10f7e72de1aef1781f5db0ee40d20e6f41b05861a722e3d8e`  
		Last Modified: Wed, 05 Oct 2022 03:52:56 GMT  
		Size: 197.7 MB (197672516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a029d0d8ff77597549c4887e0b7c71c4c2dc6c5b837db8eaa6edbcbdf5c56729
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.7 MB (223702443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c21ca30b7fafab565f525a6aeb99324f35dad0e19bfc20af0c4aabe5d9f01f7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:21 GMT
ADD file:d9af7670f58e9478e400dac85a0fcb07a4209846dbd1ea560fdc6de6e2cb5e4e in / 
# Tue, 25 Oct 2022 01:23:22 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:40:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:40:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 02:41:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:43:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9aed974aece14dd3aed00810d58a89e87eb5be9ad1c6fbb1ed077dc3f145dccc`  
		Last Modified: Tue, 25 Oct 2022 01:24:48 GMT  
		Size: 28.6 MB (28641668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0474dffae2d1e16bb420718a81adc05c65e7cf46cfec815544e0ed630334ee45`  
		Last Modified: Tue, 25 Oct 2022 02:52:51 GMT  
		Size: 3.8 MB (3809925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdff4ace6c098f616aa6e4ddee394e5472cdf30f97f3b22e0dc26d42d42e234`  
		Last Modified: Tue, 25 Oct 2022 02:52:50 GMT  
		Size: 3.5 MB (3472443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92140a87366357bdb10310a5cb8497d894c21c28e686a09af051436e071d5075`  
		Last Modified: Tue, 25 Oct 2022 02:53:04 GMT  
		Size: 39.3 MB (39282461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbee90fa764eaad308daac34a4b01988b99caaacb98cb0406b358fbe0189c634`  
		Last Modified: Tue, 25 Oct 2022 02:53:28 GMT  
		Size: 148.5 MB (148495946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:jammy-curl`

```console
$ docker pull buildpack-deps@sha256:ddf553ac35b8e1c73edae378982907fffdf1efaa9b9feb2252bdf37fc789e1db
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
$ docker pull buildpack-deps@sha256:c7cae1ebcf24a005d9b891b12f383a883c7f895687513539d29e2bd2c232c277
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37794698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35f4a6fc9e8fc4a47f232b1e95bf6c08b6eebe56c156237c14846c8ca8cc33aa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:20 GMT
ADD file:6cd2e13356aa5339c1f2abd3c210a52f6ed74fae05cd61aa09f37b6a4764f65c in / 
# Tue, 04 Oct 2022 23:35:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:09:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:09:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:cf92e523b49ea3d1fae59f5f082437a5f96c244fda6697995920142ff31d59cf`  
		Last Modified: Tue, 04 Oct 2022 03:04:01 GMT  
		Size: 30.4 MB (30428928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19b9364a5e7fea40b9e9eb4614f0e4533857b602c7fba30362889933ef14298`  
		Last Modified: Wed, 05 Oct 2022 01:24:38 GMT  
		Size: 3.8 MB (3804673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:856d49148d8882ac6866bcbcbaa08bacfe1f0d0d382b73675630ae29d44ae3f2`  
		Last Modified: Wed, 05 Oct 2022 01:24:38 GMT  
		Size: 3.6 MB (3561097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:89e3caec70fda990f819f3531875b9b314c843b4dd840be4234868015633048e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34286770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ce49fd48b1ba4f7396facd63ca2177d567b41ea796aae1f686d42df955bc0e9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:57 GMT
ADD file:11e25fc4812528219464289700bb0495bf9298918899103c33d7ef9022690eb0 in / 
# Wed, 05 Oct 2022 00:13:57 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:44:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:45:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:99b9c73338a7c0dbe41f9fc543fae706650a616453e1e330f870e20916c18a11`  
		Last Modified: Wed, 05 Oct 2022 00:16:02 GMT  
		Size: 27.0 MB (27018632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c337b77409c2e34b5e69df73a11e0ef62cd00b8b23e7d6776235d6491726ac80`  
		Last Modified: Wed, 05 Oct 2022 01:00:37 GMT  
		Size: 3.6 MB (3555370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a1dc485f1a7e2433bb9a4501dac3fb4727fb7708715e743277a50ba4933ca1`  
		Last Modified: Wed, 05 Oct 2022 01:00:37 GMT  
		Size: 3.7 MB (3712768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:cde36d71bbe4425cd9a8fb5d75a26f77d01d71b9e6d658f8784a56d78df99760
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35694165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35a2b15ea2ec567cdf8db58cf77a502d8fe85f3a84932dc89b54aafc94a6d716`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:55:02 GMT
ADD file:515177312f20fb1814b89bfccfe695fa2354bbb6d43fdb6e018bf5b1acc17e9f in / 
# Tue, 25 Oct 2022 05:55:02 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:14:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:14:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:56a2caa6b2c66e01954c1a013b37ea359b6e6af8989dbfb958124b6318771af4`  
		Last Modified: Tue, 25 Oct 2022 05:56:14 GMT  
		Size: 28.4 MB (28382489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85c75d65daee139419e66b36968af1443c6839bbfa07f1ff10f41c14059531f8`  
		Last Modified: Tue, 25 Oct 2022 08:35:08 GMT  
		Size: 3.8 MB (3776223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b571e5291fabe657fef93ed4c8e7109c81e0538a58853a65f33d52b4aa5a9f`  
		Last Modified: Tue, 25 Oct 2022 08:35:08 GMT  
		Size: 3.5 MB (3535453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:e149ccd1fd8c23ad674ee2e9cb1640264f96480646dce6134a50c9e1f1e2755a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44220306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f1727c427b596139f4521abd4689b24bbfa286d1a6220a86f3a1705080d7778`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:26:00 GMT
ADD file:766b7743de4ed1a194fc749b7649d245b0cd545b03cc2c81f16a6c15e91c87e7 in / 
# Tue, 25 Oct 2022 03:26:02 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:33:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:33:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:aa33126e789290559dc146af02cbf168119ed23be1e30fd99fe8572956e50616`  
		Last Modified: Tue, 25 Oct 2022 03:28:08 GMT  
		Size: 35.7 MB (35709401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6373837e7f2a85c7283b43d7d1a07f2541140a0a6287dc704fdf1df6ed09c5e`  
		Last Modified: Tue, 25 Oct 2022 06:55:38 GMT  
		Size: 4.3 MB (4276445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:847050f2ae34b2e1019b09f2bdbac09fd4a3c7efcaf4545aa162094c15b7f016`  
		Last Modified: Tue, 25 Oct 2022 06:55:38 GMT  
		Size: 4.2 MB (4234460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:674baad7923a60a55b6a139740aa1dd03ec351bca096cec8eef67d577490dce6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35123746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:165bda599f3c7984f6273e3a5eccf5326245110c5394238add81f83ae779e6e6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:14:15 GMT
ADD file:e1fa146cf8e97dd6a2f3ebb2dacba539556ef4a1e87dc53bd745a3cf0ba10aef in / 
# Wed, 05 Oct 2022 00:14:16 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:46:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:47:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:cbeff255552ba792be63b343113968df42de6f599d1372edd4c7346d08dfeace`  
		Last Modified: Wed, 05 Oct 2022 00:31:39 GMT  
		Size: 27.7 MB (27747416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6129e2d138d3d5141f87ef04090f82aeeb874b1d1e3c6f6e94d843cd2447826`  
		Last Modified: Wed, 05 Oct 2022 03:43:29 GMT  
		Size: 3.6 MB (3598134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a1ba2d60715be154c4f520ac4f1ef149f66b921651ab2726a809c14316e55a`  
		Last Modified: Wed, 05 Oct 2022 03:43:27 GMT  
		Size: 3.8 MB (3778196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:c9f438fe30404f17ac10a8f79981bf6ab4f788d3706b23e99b92133fa1133a58
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35924036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13ac7d74d18b331d205348291551e18d9bd7010f18fc44d6f55875b60652fdf1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:21 GMT
ADD file:d9af7670f58e9478e400dac85a0fcb07a4209846dbd1ea560fdc6de6e2cb5e4e in / 
# Tue, 25 Oct 2022 01:23:22 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:40:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:40:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9aed974aece14dd3aed00810d58a89e87eb5be9ad1c6fbb1ed077dc3f145dccc`  
		Last Modified: Tue, 25 Oct 2022 01:24:48 GMT  
		Size: 28.6 MB (28641668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0474dffae2d1e16bb420718a81adc05c65e7cf46cfec815544e0ed630334ee45`  
		Last Modified: Tue, 25 Oct 2022 02:52:51 GMT  
		Size: 3.8 MB (3809925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdff4ace6c098f616aa6e4ddee394e5472cdf30f97f3b22e0dc26d42d42e234`  
		Last Modified: Tue, 25 Oct 2022 02:52:50 GMT  
		Size: 3.5 MB (3472443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:jammy-scm`

```console
$ docker pull buildpack-deps@sha256:6625116a3d22e3df460e9151fa87afc625bcee4797882f9fd56f946c8b7d587f
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
$ docker pull buildpack-deps@sha256:dd6a1375f1f144120e73c33263d15fad407cdf3af5700bf06b98c42e712a0d2a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77143770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da5fb79923d815372876a15ca9afa7294969ee8f6142ae8377dd987dd91de455`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:20 GMT
ADD file:6cd2e13356aa5339c1f2abd3c210a52f6ed74fae05cd61aa09f37b6a4764f65c in / 
# Tue, 04 Oct 2022 23:35:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:09:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:09:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:10:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cf92e523b49ea3d1fae59f5f082437a5f96c244fda6697995920142ff31d59cf`  
		Last Modified: Tue, 04 Oct 2022 03:04:01 GMT  
		Size: 30.4 MB (30428928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19b9364a5e7fea40b9e9eb4614f0e4533857b602c7fba30362889933ef14298`  
		Last Modified: Wed, 05 Oct 2022 01:24:38 GMT  
		Size: 3.8 MB (3804673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:856d49148d8882ac6866bcbcbaa08bacfe1f0d0d382b73675630ae29d44ae3f2`  
		Last Modified: Wed, 05 Oct 2022 01:24:38 GMT  
		Size: 3.6 MB (3561097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f83374f27f6992ee240fe68ce2e0c2d9db958dc2c9acf1864ef83040cc5387`  
		Last Modified: Wed, 05 Oct 2022 01:24:54 GMT  
		Size: 39.3 MB (39349072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:8ee2ceb7f89309d35af0ffd83a4e9f99593da3ebc818ef9db16edea6807e5999
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76186876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ac586f0d0ef3e15932beb867ebeae6c400aec079dbb4e9675345a7b3a0cfb07`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:57 GMT
ADD file:11e25fc4812528219464289700bb0495bf9298918899103c33d7ef9022690eb0 in / 
# Wed, 05 Oct 2022 00:13:57 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:44:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:45:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:45:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99b9c73338a7c0dbe41f9fc543fae706650a616453e1e330f870e20916c18a11`  
		Last Modified: Wed, 05 Oct 2022 00:16:02 GMT  
		Size: 27.0 MB (27018632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c337b77409c2e34b5e69df73a11e0ef62cd00b8b23e7d6776235d6491726ac80`  
		Last Modified: Wed, 05 Oct 2022 01:00:37 GMT  
		Size: 3.6 MB (3555370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a1dc485f1a7e2433bb9a4501dac3fb4727fb7708715e743277a50ba4933ca1`  
		Last Modified: Wed, 05 Oct 2022 01:00:37 GMT  
		Size: 3.7 MB (3712768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5595ebdf3f8239b659bdbfc55b5e0a70965f29a4e546cc5efdda43f8e3a4ef76`  
		Last Modified: Wed, 05 Oct 2022 01:01:00 GMT  
		Size: 41.9 MB (41900106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ba599423790494bb456afcac072a93c962e4ec9d980064386cabcee48af29d1c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.9 MB (74930248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:808e03b9a2c409feb946d3d926084d928f7da4f40a01604e98dafd06b7f57b9e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:55:02 GMT
ADD file:515177312f20fb1814b89bfccfe695fa2354bbb6d43fdb6e018bf5b1acc17e9f in / 
# Tue, 25 Oct 2022 05:55:02 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:14:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:14:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:15:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:56a2caa6b2c66e01954c1a013b37ea359b6e6af8989dbfb958124b6318771af4`  
		Last Modified: Tue, 25 Oct 2022 05:56:14 GMT  
		Size: 28.4 MB (28382489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85c75d65daee139419e66b36968af1443c6839bbfa07f1ff10f41c14059531f8`  
		Last Modified: Tue, 25 Oct 2022 08:35:08 GMT  
		Size: 3.8 MB (3776223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b571e5291fabe657fef93ed4c8e7109c81e0538a58853a65f33d52b4aa5a9f`  
		Last Modified: Tue, 25 Oct 2022 08:35:08 GMT  
		Size: 3.5 MB (3535453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d47a2b6e938e7cf8632d33777355c83ebf1eb36d91c3dc64efc269e15e34ddb`  
		Last Modified: Tue, 25 Oct 2022 08:35:23 GMT  
		Size: 39.2 MB (39236083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:9d256e35b3c4819a62e8a49fcf0872c6714d2d5ae957d9812046d42db0aa388b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.0 MB (87973603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b228d7257419ba62688701d08a6f0b18e366ccb8c7796bd83cc3c3b1ae61030b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:26:00 GMT
ADD file:766b7743de4ed1a194fc749b7649d245b0cd545b03cc2c81f16a6c15e91c87e7 in / 
# Tue, 25 Oct 2022 03:26:02 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:33:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:33:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:34:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:aa33126e789290559dc146af02cbf168119ed23be1e30fd99fe8572956e50616`  
		Last Modified: Tue, 25 Oct 2022 03:28:08 GMT  
		Size: 35.7 MB (35709401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6373837e7f2a85c7283b43d7d1a07f2541140a0a6287dc704fdf1df6ed09c5e`  
		Last Modified: Tue, 25 Oct 2022 06:55:38 GMT  
		Size: 4.3 MB (4276445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:847050f2ae34b2e1019b09f2bdbac09fd4a3c7efcaf4545aa162094c15b7f016`  
		Last Modified: Tue, 25 Oct 2022 06:55:38 GMT  
		Size: 4.2 MB (4234460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186cf1c98556ab0c2ae47af200ed2f3a8f340ad4cd305379f23619197f2ec188`  
		Last Modified: Tue, 25 Oct 2022 06:56:02 GMT  
		Size: 43.8 MB (43753297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:0b59c501076932d75abe6baf6b45272617ca658c00bea23c4c642ecf0cef54ad
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77238223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c179e15b046f9a7a277678332c1ba0ff71c2985288dede5b120f176dbd7b378`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:14:15 GMT
ADD file:e1fa146cf8e97dd6a2f3ebb2dacba539556ef4a1e87dc53bd745a3cf0ba10aef in / 
# Wed, 05 Oct 2022 00:14:16 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:46:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:47:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 02:51:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cbeff255552ba792be63b343113968df42de6f599d1372edd4c7346d08dfeace`  
		Last Modified: Wed, 05 Oct 2022 00:31:39 GMT  
		Size: 27.7 MB (27747416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6129e2d138d3d5141f87ef04090f82aeeb874b1d1e3c6f6e94d843cd2447826`  
		Last Modified: Wed, 05 Oct 2022 03:43:29 GMT  
		Size: 3.6 MB (3598134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a1ba2d60715be154c4f520ac4f1ef149f66b921651ab2726a809c14316e55a`  
		Last Modified: Wed, 05 Oct 2022 03:43:27 GMT  
		Size: 3.8 MB (3778196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91414a4a50607595a5e83cc27ee8f8e885ea1d1c43848a3df1487911ae62cc19`  
		Last Modified: Wed, 05 Oct 2022 03:45:48 GMT  
		Size: 42.1 MB (42114477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:1261bcd972c83821318a0ffbee775f7c50792bde771fc73c806e78a7af67b584
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75206497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44680731da527ce74344c9ff0197ff653c79174a875a4711b0b82402a398c303`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:21 GMT
ADD file:d9af7670f58e9478e400dac85a0fcb07a4209846dbd1ea560fdc6de6e2cb5e4e in / 
# Tue, 25 Oct 2022 01:23:22 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:40:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:40:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 02:41:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9aed974aece14dd3aed00810d58a89e87eb5be9ad1c6fbb1ed077dc3f145dccc`  
		Last Modified: Tue, 25 Oct 2022 01:24:48 GMT  
		Size: 28.6 MB (28641668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0474dffae2d1e16bb420718a81adc05c65e7cf46cfec815544e0ed630334ee45`  
		Last Modified: Tue, 25 Oct 2022 02:52:51 GMT  
		Size: 3.8 MB (3809925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdff4ace6c098f616aa6e4ddee394e5472cdf30f97f3b22e0dc26d42d42e234`  
		Last Modified: Tue, 25 Oct 2022 02:52:50 GMT  
		Size: 3.5 MB (3472443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92140a87366357bdb10310a5cb8497d894c21c28e686a09af051436e071d5075`  
		Last Modified: Tue, 25 Oct 2022 02:53:04 GMT  
		Size: 39.3 MB (39282461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:kinetic`

```console
$ docker pull buildpack-deps@sha256:4bb8f04c36a68d87bb5d569f8ef15acf77df7d6d27bb36b3b935211fddc8acd2
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
$ docker pull buildpack-deps@sha256:b33788a433b2f998ebd368f99762872a3c6c6009abe173f62fb4e1e94c9ae7a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.8 MB (265793471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:622366e2d78507bc25ad39ba5e3b6c6a4b43d982571e1a8250ba68d37223db3e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:28 GMT
ADD file:3384549425c94b92a7d7be15958e3ec7494bdf83242deb465d9059d4362d34d6 in / 
# Tue, 04 Oct 2022 23:35:28 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:13:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:13:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:14:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:16:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5887826a0d8b4c403d9bfaf57279fd8b585d272c3f450d374349365dc22cd8ef`  
		Last Modified: Tue, 04 Oct 2022 23:36:56 GMT  
		Size: 27.5 MB (27455077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b7fd9cb5adf6a195c3c2162caa409d926d4342598cad09f7fa4691e9ddd25f`  
		Last Modified: Wed, 05 Oct 2022 01:25:38 GMT  
		Size: 6.8 MB (6780586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9023f9ecbe71ceaba400cb934168d975ecabc157d85fe246f71d3d684947742d`  
		Last Modified: Wed, 05 Oct 2022 01:25:37 GMT  
		Size: 3.6 MB (3633909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d44eedd822ec1ffd1b32f87638bae3694f27cf99e85f8d3d8f6d1f2857fdc1`  
		Last Modified: Wed, 05 Oct 2022 01:25:54 GMT  
		Size: 39.7 MB (39713928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46cfc3a166e18ca21a45cacaeec49e724ff39c9215001117796bd74cb3b40410`  
		Last Modified: Wed, 05 Oct 2022 01:26:30 GMT  
		Size: 188.2 MB (188209971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:d55d7353e6aa732cad00a73a6c198a481ba08a5afd55721ac086a1017b1559ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.1 MB (228118532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10bca3a5fa8bf85ff72ac75e507466eacf465294389c059f87eb1ceaa37efa93`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:14:09 GMT
ADD file:4b538f2c7b46aa601d747159ce9e8c2c7a99b2b6e09e4efe1073ca58e47fbeed in / 
# Wed, 05 Oct 2022 00:14:09 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:47:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:47:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:48:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:49:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:788f7bb1e1d719f6a9a9b3b1530cc5bbe5b808a2ad77a65f23e2c6d15b8ae546`  
		Last Modified: Wed, 05 Oct 2022 00:16:28 GMT  
		Size: 25.9 MB (25873193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31aeed2022326b456329596b112851c2e027ba5773dab33fcd717efb1a016274`  
		Last Modified: Wed, 05 Oct 2022 01:01:56 GMT  
		Size: 6.0 MB (5955685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b8a4829745394c3402e5970b4558ef9fe23515f895e7f8a99fe24ae33a7c4f3`  
		Last Modified: Wed, 05 Oct 2022 01:01:55 GMT  
		Size: 3.8 MB (3801708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199fb45c30ad58843e78384afd22f7dec65ac55a285086da2083dea2426fd37e`  
		Last Modified: Wed, 05 Oct 2022 01:02:19 GMT  
		Size: 42.6 MB (42596389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd5d37220a8883d442a1686f49907c73299d8c1df3d5f6cc9a9d1b8c9012583`  
		Last Modified: Wed, 05 Oct 2022 01:03:07 GMT  
		Size: 149.9 MB (149891557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7f591bb67e4190e35105756af84f44d4bdd7c020d451632335a530a83e8e299a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.6 MB (246644046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:418c243a099dd8aadaf491de0633949554b9e17b02bb3dbecaeba22314be0c60`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:55:06 GMT
ADD file:30361063c284df6e20a85ff95b9c7b93648fe9e04ac935c9ff888e5c5f3af7ea in / 
# Tue, 25 Oct 2022 05:55:06 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:19:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:19:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:20:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:23:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a2e58a4bc1e52e3ab8904706a68a79146364ec32d8caf1bd106c3c9966a38fc`  
		Last Modified: Tue, 25 Oct 2022 05:56:30 GMT  
		Size: 26.7 MB (26676995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208c8913a9c66f64a1f5ca1349c8a8b9923f9eb9c8aed25bf3ec160a33e5a796`  
		Last Modified: Tue, 25 Oct 2022 08:36:03 GMT  
		Size: 6.6 MB (6607031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8491d7cc7a42af61771e26652e91532db813e380fa19339f7279420206df0290`  
		Last Modified: Tue, 25 Oct 2022 08:36:03 GMT  
		Size: 3.6 MB (3602476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2cf60ff33717c4a17f0ca2f77473b69d8d357e4dc81ef8bb8a5e24382aa106`  
		Last Modified: Tue, 25 Oct 2022 08:36:17 GMT  
		Size: 39.5 MB (39486568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2297c22e5e80de066ab641f5f47a060831dda9dbda728c9ffc0333ffd65aec38`  
		Last Modified: Tue, 25 Oct 2022 08:36:45 GMT  
		Size: 170.3 MB (170270976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:b85564067cd24e7645a51fcc5b5ee66f50498a7a4cad4db8f8e748271b4cbfe0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.3 MB (281263738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:402a9d4fffb8624f6fa449162bbd5c6ef48031ba4a3813d392416260f6ab5055`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:26:14 GMT
ADD file:60dd11bbfa9f1e2bc613c7f05cbbb83bca9e4b81550b6a0540a5d1d39f870cdd in / 
# Tue, 25 Oct 2022 03:26:16 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:40:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:40:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:41:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:44:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6d37bc653a986baef621c195bf8def80ca65133b8a3917bbd3a148b31bc1704f`  
		Last Modified: Tue, 25 Oct 2022 03:28:34 GMT  
		Size: 32.1 MB (32099941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc18decfda3085820c97e73c59dba18c534c4455c2eafc5812d29975ad7a9292`  
		Last Modified: Tue, 25 Oct 2022 06:57:12 GMT  
		Size: 7.8 MB (7752006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a931134d9aa21913f6400e3083b4c6955008f9fab7eae04019249a1d912c279`  
		Last Modified: Tue, 25 Oct 2022 06:57:10 GMT  
		Size: 4.4 MB (4361351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33eb213c2d45440f6da62e4c97dcc2936c1a9881896421d53a86927e2618b29`  
		Last Modified: Tue, 25 Oct 2022 06:57:35 GMT  
		Size: 44.1 MB (44120965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77829c624efe1a2e9a13f40cb1d0c0f4d7fe497125dbf87d40699e87a907c260`  
		Last Modified: Tue, 25 Oct 2022 06:58:34 GMT  
		Size: 192.9 MB (192929475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:5670cbeec0868228f4cbe82cc9abb1f3c09d621ebbf85c7bf0369b24642df074
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.6 MB (285585964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f98764f075d571c93930c9fbb0965fe3cfd34f36ad2840deac11698e7d1b51d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:16:49 GMT
ADD file:2d01ff45e6105658cf6791d4ade5cc3168c7d455422fc973a54a795907023c4e in / 
# Wed, 05 Oct 2022 00:16:51 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:00:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:01:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 03:04:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:11:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:69c33ccbf3d1b09c78fae3f88deb756ae33a9e4610a01fc9ab8b457ee6107d7f`  
		Last Modified: Wed, 05 Oct 2022 00:35:11 GMT  
		Size: 25.6 MB (25618700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6742bf73589f8dd7c6c3ba8c0c07b6783a8c31c40b8e815941b550d904b49030`  
		Last Modified: Wed, 05 Oct 2022 03:54:22 GMT  
		Size: 5.9 MB (5938180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039b60e6247434b31a05dcae8802e410a92a3e9e6f9f6472455a58d4c1d5e1b6`  
		Last Modified: Wed, 05 Oct 2022 03:54:18 GMT  
		Size: 3.9 MB (3881311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde1ee2ce8c7376ef3e85ac490d31dcdf52bf954c3186472c53f3404c2421078`  
		Last Modified: Wed, 05 Oct 2022 03:56:41 GMT  
		Size: 42.8 MB (42832698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5e3cc23193e77d3695c7e56f6e60082abbcf0e11af954a30dda857279c355b`  
		Last Modified: Wed, 05 Oct 2022 04:03:57 GMT  
		Size: 207.3 MB (207315075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:10403bdb366987e6b3d1e90233130b79cd5e6931553eebe344edb75b787b74d6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.6 MB (228553552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e5108db95c124c6268c561f7f0b5c01f26b48f3801c253310534a9736f474fd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:31 GMT
ADD file:9c0c4172b14f0d37b0b074729a4738aeb165efe5c83e2d9bfefc5b39e4a4fe0b in / 
# Tue, 25 Oct 2022 01:23:32 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:44:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:44:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 02:44:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:46:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cf61a33f110308ce64c1dd7a5dddf2a5587ee1c8ab2351219b925428957cbc10`  
		Last Modified: Tue, 25 Oct 2022 01:25:01 GMT  
		Size: 26.0 MB (26022178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df11273ce2e4ff8fbfe44b4708e1c3b2323d38c23cc29bfb9935c1788807165`  
		Last Modified: Tue, 25 Oct 2022 02:53:37 GMT  
		Size: 6.5 MB (6473357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36f51f919c9bd6bce882afd5ce69c1de2f32276ae54369c26ae41702ff241ce`  
		Last Modified: Tue, 25 Oct 2022 02:53:35 GMT  
		Size: 3.6 MB (3625569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69ad44ec319ab50167d51a4bd01dd344bd736541842217bc94d0c6da1960b16c`  
		Last Modified: Tue, 25 Oct 2022 02:53:49 GMT  
		Size: 39.5 MB (39548002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed2d65b37ea7643db5c4a31a4261ef32fbaa397af4762b1b8e36a5f997c79998`  
		Last Modified: Tue, 25 Oct 2022 02:54:14 GMT  
		Size: 152.9 MB (152884446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:kinetic-curl`

```console
$ docker pull buildpack-deps@sha256:d2ccc8013b79e84b3e20ef12b0baabd38c34272a9dbc9699d528528df2739163
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
$ docker pull buildpack-deps@sha256:2346451d88d35553f8bab367cb3a5e8de051d8da464fdcbf91e6030f07149fa2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37869572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb4b09635cfc10ef52385f01ae24c23a01d1531710e0aadd890ac70cde9de7c7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:28 GMT
ADD file:3384549425c94b92a7d7be15958e3ec7494bdf83242deb465d9059d4362d34d6 in / 
# Tue, 04 Oct 2022 23:35:28 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:13:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:13:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5887826a0d8b4c403d9bfaf57279fd8b585d272c3f450d374349365dc22cd8ef`  
		Last Modified: Tue, 04 Oct 2022 23:36:56 GMT  
		Size: 27.5 MB (27455077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b7fd9cb5adf6a195c3c2162caa409d926d4342598cad09f7fa4691e9ddd25f`  
		Last Modified: Wed, 05 Oct 2022 01:25:38 GMT  
		Size: 6.8 MB (6780586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9023f9ecbe71ceaba400cb934168d975ecabc157d85fe246f71d3d684947742d`  
		Last Modified: Wed, 05 Oct 2022 01:25:37 GMT  
		Size: 3.6 MB (3633909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:fff25ce4b7d7eb809d772ea4f8ad0b01880c3d7746627218ba716aacb733fd61
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.6 MB (35630586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1de0ca1a233d815d4617f6e298996b96f5857277214408cdde8ef90d1a4a38e0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:14:09 GMT
ADD file:4b538f2c7b46aa601d747159ce9e8c2c7a99b2b6e09e4efe1073ca58e47fbeed in / 
# Wed, 05 Oct 2022 00:14:09 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:47:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:47:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:788f7bb1e1d719f6a9a9b3b1530cc5bbe5b808a2ad77a65f23e2c6d15b8ae546`  
		Last Modified: Wed, 05 Oct 2022 00:16:28 GMT  
		Size: 25.9 MB (25873193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31aeed2022326b456329596b112851c2e027ba5773dab33fcd717efb1a016274`  
		Last Modified: Wed, 05 Oct 2022 01:01:56 GMT  
		Size: 6.0 MB (5955685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b8a4829745394c3402e5970b4558ef9fe23515f895e7f8a99fe24ae33a7c4f3`  
		Last Modified: Wed, 05 Oct 2022 01:01:55 GMT  
		Size: 3.8 MB (3801708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:373a282293140d34f364cb32917ccbfbb1b5657135e1d5b77becf7ec26d57437
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.9 MB (36886502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d0532ca7c686b7c5989d673e4c097b51d9fa7759a3b351e18ab993f11252e5d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:55:06 GMT
ADD file:30361063c284df6e20a85ff95b9c7b93648fe9e04ac935c9ff888e5c5f3af7ea in / 
# Tue, 25 Oct 2022 05:55:06 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:19:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:19:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:7a2e58a4bc1e52e3ab8904706a68a79146364ec32d8caf1bd106c3c9966a38fc`  
		Last Modified: Tue, 25 Oct 2022 05:56:30 GMT  
		Size: 26.7 MB (26676995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208c8913a9c66f64a1f5ca1349c8a8b9923f9eb9c8aed25bf3ec160a33e5a796`  
		Last Modified: Tue, 25 Oct 2022 08:36:03 GMT  
		Size: 6.6 MB (6607031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8491d7cc7a42af61771e26652e91532db813e380fa19339f7279420206df0290`  
		Last Modified: Tue, 25 Oct 2022 08:36:03 GMT  
		Size: 3.6 MB (3602476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:9144ea52e36fbf4e170dfe335aab6d5de9469737d3055aa70abfbed5e80d33fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44213298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9c8b0212d45ff3894e9e1dbc78bade496aa82a9c927fd6b5fd083714d2fa734`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:26:14 GMT
ADD file:60dd11bbfa9f1e2bc613c7f05cbbb83bca9e4b81550b6a0540a5d1d39f870cdd in / 
# Tue, 25 Oct 2022 03:26:16 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:40:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:40:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6d37bc653a986baef621c195bf8def80ca65133b8a3917bbd3a148b31bc1704f`  
		Last Modified: Tue, 25 Oct 2022 03:28:34 GMT  
		Size: 32.1 MB (32099941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc18decfda3085820c97e73c59dba18c534c4455c2eafc5812d29975ad7a9292`  
		Last Modified: Tue, 25 Oct 2022 06:57:12 GMT  
		Size: 7.8 MB (7752006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a931134d9aa21913f6400e3083b4c6955008f9fab7eae04019249a1d912c279`  
		Last Modified: Tue, 25 Oct 2022 06:57:10 GMT  
		Size: 4.4 MB (4361351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:4a2ac75c4ca1565140be2a5b2034effcf76de970fa53df98e47b6f6e7d58d3b5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.4 MB (35438191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b1442e7c0a8c0abe0dfc567219f3d6aa55e9adf597d425bff2605c64c8115bb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:16:49 GMT
ADD file:2d01ff45e6105658cf6791d4ade5cc3168c7d455422fc973a54a795907023c4e in / 
# Wed, 05 Oct 2022 00:16:51 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:00:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:01:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:69c33ccbf3d1b09c78fae3f88deb756ae33a9e4610a01fc9ab8b457ee6107d7f`  
		Last Modified: Wed, 05 Oct 2022 00:35:11 GMT  
		Size: 25.6 MB (25618700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6742bf73589f8dd7c6c3ba8c0c07b6783a8c31c40b8e815941b550d904b49030`  
		Last Modified: Wed, 05 Oct 2022 03:54:22 GMT  
		Size: 5.9 MB (5938180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039b60e6247434b31a05dcae8802e410a92a3e9e6f9f6472455a58d4c1d5e1b6`  
		Last Modified: Wed, 05 Oct 2022 03:54:18 GMT  
		Size: 3.9 MB (3881311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:75ab25d6d67c72f804bc2ecca53130abb5963b93b91371b24be4f8ab90b4b54a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.1 MB (36121104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:644ada4f863420e616b970ac64e228a95ba0993dfbee2c4fb59ad86e50b0566e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:31 GMT
ADD file:9c0c4172b14f0d37b0b074729a4738aeb165efe5c83e2d9bfefc5b39e4a4fe0b in / 
# Tue, 25 Oct 2022 01:23:32 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:44:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:44:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:cf61a33f110308ce64c1dd7a5dddf2a5587ee1c8ab2351219b925428957cbc10`  
		Last Modified: Tue, 25 Oct 2022 01:25:01 GMT  
		Size: 26.0 MB (26022178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df11273ce2e4ff8fbfe44b4708e1c3b2323d38c23cc29bfb9935c1788807165`  
		Last Modified: Tue, 25 Oct 2022 02:53:37 GMT  
		Size: 6.5 MB (6473357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36f51f919c9bd6bce882afd5ce69c1de2f32276ae54369c26ae41702ff241ce`  
		Last Modified: Tue, 25 Oct 2022 02:53:35 GMT  
		Size: 3.6 MB (3625569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:kinetic-scm`

```console
$ docker pull buildpack-deps@sha256:044006a56118d10d105fef337fa49803641ab52652693b35a7a4b6a22555ef48
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
$ docker pull buildpack-deps@sha256:d04920e171fddca160ba2431b2421bf49b424767a2a15f5be91bb9d94f21bb2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.6 MB (77583500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64ef1de29f63807a6093e6af698173335a81692ab641a3e02e63bc9df42ea5f9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:28 GMT
ADD file:3384549425c94b92a7d7be15958e3ec7494bdf83242deb465d9059d4362d34d6 in / 
# Tue, 04 Oct 2022 23:35:28 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:13:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:13:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:14:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5887826a0d8b4c403d9bfaf57279fd8b585d272c3f450d374349365dc22cd8ef`  
		Last Modified: Tue, 04 Oct 2022 23:36:56 GMT  
		Size: 27.5 MB (27455077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b7fd9cb5adf6a195c3c2162caa409d926d4342598cad09f7fa4691e9ddd25f`  
		Last Modified: Wed, 05 Oct 2022 01:25:38 GMT  
		Size: 6.8 MB (6780586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9023f9ecbe71ceaba400cb934168d975ecabc157d85fe246f71d3d684947742d`  
		Last Modified: Wed, 05 Oct 2022 01:25:37 GMT  
		Size: 3.6 MB (3633909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d44eedd822ec1ffd1b32f87638bae3694f27cf99e85f8d3d8f6d1f2857fdc1`  
		Last Modified: Wed, 05 Oct 2022 01:25:54 GMT  
		Size: 39.7 MB (39713928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:2965cc2f6b4e99430ed3e5dc6e19cff61861fd39ce9247198d0446c4ea18da12
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.2 MB (78226975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf87da53eb6a1926ffac398aa2b41ffc1c7ba4e19fa01b0c1e132a9fcfa6d7ad`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:14:09 GMT
ADD file:4b538f2c7b46aa601d747159ce9e8c2c7a99b2b6e09e4efe1073ca58e47fbeed in / 
# Wed, 05 Oct 2022 00:14:09 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:47:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:47:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:48:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:788f7bb1e1d719f6a9a9b3b1530cc5bbe5b808a2ad77a65f23e2c6d15b8ae546`  
		Last Modified: Wed, 05 Oct 2022 00:16:28 GMT  
		Size: 25.9 MB (25873193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31aeed2022326b456329596b112851c2e027ba5773dab33fcd717efb1a016274`  
		Last Modified: Wed, 05 Oct 2022 01:01:56 GMT  
		Size: 6.0 MB (5955685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b8a4829745394c3402e5970b4558ef9fe23515f895e7f8a99fe24ae33a7c4f3`  
		Last Modified: Wed, 05 Oct 2022 01:01:55 GMT  
		Size: 3.8 MB (3801708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199fb45c30ad58843e78384afd22f7dec65ac55a285086da2083dea2426fd37e`  
		Last Modified: Wed, 05 Oct 2022 01:02:19 GMT  
		Size: 42.6 MB (42596389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f9e6c255feb050995c15d584bed8b4ef31d7171ecc8f79741ce561d7ab013ce5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.4 MB (76373070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2e46d98faf0c177cab0e52968d9d062a3a4f181d3c42f5759c5eb9615ccd5b8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:55:06 GMT
ADD file:30361063c284df6e20a85ff95b9c7b93648fe9e04ac935c9ff888e5c5f3af7ea in / 
# Tue, 25 Oct 2022 05:55:06 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:19:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:19:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:20:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a2e58a4bc1e52e3ab8904706a68a79146364ec32d8caf1bd106c3c9966a38fc`  
		Last Modified: Tue, 25 Oct 2022 05:56:30 GMT  
		Size: 26.7 MB (26676995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208c8913a9c66f64a1f5ca1349c8a8b9923f9eb9c8aed25bf3ec160a33e5a796`  
		Last Modified: Tue, 25 Oct 2022 08:36:03 GMT  
		Size: 6.6 MB (6607031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8491d7cc7a42af61771e26652e91532db813e380fa19339f7279420206df0290`  
		Last Modified: Tue, 25 Oct 2022 08:36:03 GMT  
		Size: 3.6 MB (3602476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2cf60ff33717c4a17f0ca2f77473b69d8d357e4dc81ef8bb8a5e24382aa106`  
		Last Modified: Tue, 25 Oct 2022 08:36:17 GMT  
		Size: 39.5 MB (39486568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:ce93a24cd078d6b8c4f5f7301e8e03082dc0b280b7699a23b4a638e67ae2efdb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.3 MB (88334263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b98ffc392030e610f3af3f6119e1fda61df1f4b3d9ae0d893603fbbc1949cfc0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:26:14 GMT
ADD file:60dd11bbfa9f1e2bc613c7f05cbbb83bca9e4b81550b6a0540a5d1d39f870cdd in / 
# Tue, 25 Oct 2022 03:26:16 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:40:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:40:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:41:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6d37bc653a986baef621c195bf8def80ca65133b8a3917bbd3a148b31bc1704f`  
		Last Modified: Tue, 25 Oct 2022 03:28:34 GMT  
		Size: 32.1 MB (32099941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc18decfda3085820c97e73c59dba18c534c4455c2eafc5812d29975ad7a9292`  
		Last Modified: Tue, 25 Oct 2022 06:57:12 GMT  
		Size: 7.8 MB (7752006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a931134d9aa21913f6400e3083b4c6955008f9fab7eae04019249a1d912c279`  
		Last Modified: Tue, 25 Oct 2022 06:57:10 GMT  
		Size: 4.4 MB (4361351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33eb213c2d45440f6da62e4c97dcc2936c1a9881896421d53a86927e2618b29`  
		Last Modified: Tue, 25 Oct 2022 06:57:35 GMT  
		Size: 44.1 MB (44120965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:ab238169f3b08dc7c08c8e3ed46e6ad74014ba89c7d7d398a9038687df3104a5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78270889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bec2b637df9811eabf5c8c05afc79681031c55e2b577567a231be07852233f7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:16:49 GMT
ADD file:2d01ff45e6105658cf6791d4ade5cc3168c7d455422fc973a54a795907023c4e in / 
# Wed, 05 Oct 2022 00:16:51 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:00:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:01:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 03:04:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:69c33ccbf3d1b09c78fae3f88deb756ae33a9e4610a01fc9ab8b457ee6107d7f`  
		Last Modified: Wed, 05 Oct 2022 00:35:11 GMT  
		Size: 25.6 MB (25618700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6742bf73589f8dd7c6c3ba8c0c07b6783a8c31c40b8e815941b550d904b49030`  
		Last Modified: Wed, 05 Oct 2022 03:54:22 GMT  
		Size: 5.9 MB (5938180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039b60e6247434b31a05dcae8802e410a92a3e9e6f9f6472455a58d4c1d5e1b6`  
		Last Modified: Wed, 05 Oct 2022 03:54:18 GMT  
		Size: 3.9 MB (3881311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde1ee2ce8c7376ef3e85ac490d31dcdf52bf954c3186472c53f3404c2421078`  
		Last Modified: Wed, 05 Oct 2022 03:56:41 GMT  
		Size: 42.8 MB (42832698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:ca6937235c92176f4e66e5e83e654d8ac06099c69d6cdd2917dca4640643463c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75669106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15939ebf9f49b3608111d36fac9b9adb1584829b3dcfba4701e71c081de209c0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:31 GMT
ADD file:9c0c4172b14f0d37b0b074729a4738aeb165efe5c83e2d9bfefc5b39e4a4fe0b in / 
# Tue, 25 Oct 2022 01:23:32 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:44:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:44:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 02:44:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cf61a33f110308ce64c1dd7a5dddf2a5587ee1c8ab2351219b925428957cbc10`  
		Last Modified: Tue, 25 Oct 2022 01:25:01 GMT  
		Size: 26.0 MB (26022178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df11273ce2e4ff8fbfe44b4708e1c3b2323d38c23cc29bfb9935c1788807165`  
		Last Modified: Tue, 25 Oct 2022 02:53:37 GMT  
		Size: 6.5 MB (6473357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36f51f919c9bd6bce882afd5ce69c1de2f32276ae54369c26ae41702ff241ce`  
		Last Modified: Tue, 25 Oct 2022 02:53:35 GMT  
		Size: 3.6 MB (3625569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69ad44ec319ab50167d51a4bd01dd344bd736541842217bc94d0c6da1960b16c`  
		Last Modified: Tue, 25 Oct 2022 02:53:49 GMT  
		Size: 39.5 MB (39548002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:latest`

```console
$ docker pull buildpack-deps@sha256:4c611d88a39769ef8b4a77505f9377f74df78ae41bf9f81be47522d13549ba1b
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
$ docker pull buildpack-deps@sha256:da6442775441c5a43c9cdcbc18c633c9a94196521736ea0c04d3bc4ab6d24007
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.5 MB (322518570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c35b468f323a45e3ac977f6960f5657ec31473c3a183f96f5ff908fdfa3f9b8d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:27 GMT
ADD file:d1268789456d2cdace6e50149e60404ad5a849b7c61e8fc8bc7b6e0eb6eeb7ca in / 
# Tue, 04 Oct 2022 23:26:27 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:54:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:55:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:55:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:56:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f606d8928ed378229f2460b94b504cca239fb906efc57acbdf9340bd298d5ddf`  
		Last Modified: Tue, 04 Oct 2022 23:30:27 GMT  
		Size: 55.0 MB (55046248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47db815c6a4547dc224b75222193cb1851cf529d2cbdf26f854b9bbf97099b98`  
		Last Modified: Wed, 05 Oct 2022 01:19:13 GMT  
		Size: 5.2 MB (5163279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf48494000001a037b72870d2a6a2536f9da8bc5d1ceddd72d79f4a51fe7a60e`  
		Last Modified: Wed, 05 Oct 2022 01:19:13 GMT  
		Size: 10.9 MB (10876505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a572f7a256d36a93ab0777949771b120c5d7dce75ea2a2d3d9444793b26b2ef1`  
		Last Modified: Wed, 05 Oct 2022 01:19:34 GMT  
		Size: 54.6 MB (54584293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f7d0525895528fdb73153451e112bbd8e1854549bd1e0e6f4ac0b4a2ee98172`  
		Last Modified: Wed, 05 Oct 2022 01:20:11 GMT  
		Size: 196.8 MB (196848245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:e95f5a44cff65278e6f2df29eef9d7957e19ab74e610841ca613250500cfb07c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.6 MB (295556261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5fc1f9478434ff5825094db6336cb96abec3dff210ea3918afc05508b3b8389`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:06:19 GMT
ADD file:b314b98654e8532fd10a08a172ea5c3edb7d7a36c7faf85d06d14be12f7b83ef in / 
# Tue, 25 Oct 2022 03:06:19 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:12:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:12:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:12:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:14:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1f0ecb08923b99bef3f82c2e88603bb53e3ed084c13252275c05039cc279c158`  
		Last Modified: Tue, 25 Oct 2022 03:11:15 GMT  
		Size: 52.5 MB (52547473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b399c5eb53b4c35fa33682a82d73bdc4b096cd78ae95fe36c4ed81d18f6849`  
		Last Modified: Tue, 25 Oct 2022 06:19:02 GMT  
		Size: 5.1 MB (5072235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ccdd06393cd3873a3cc8b9cbe170a2032fd61d1d545b7045b649faf2f4e732`  
		Last Modified: Tue, 25 Oct 2022 06:19:02 GMT  
		Size: 10.6 MB (10574279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aafe0e287af4e488dcda51195e4eb1ae1386e3265989c457172f32f6357bf26`  
		Last Modified: Tue, 25 Oct 2022 06:19:28 GMT  
		Size: 52.3 MB (52322157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22771ccea19352dbb0e5ba44c17b8ef14425ff0a22c744bca41cdbde02bdfd9f`  
		Last Modified: Tue, 25 Oct 2022 06:20:12 GMT  
		Size: 175.0 MB (175040117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:4ef648e774c537efc33738cca9dfbc87771bbbaab19e36fffdc55e0f440c699a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.0 MB (283005348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe5e78b4d0fb86176858f424786c09b823ee34558e44538321f40a14100f6a57`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:28 GMT
ADD file:47a3f2948af18c39686ca59a88a439c25edaf286064d3a2ccc5dab47fee2fc52 in / 
# Tue, 04 Oct 2022 23:58:29 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:32:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:32:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:32:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:34:32 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e19342fb46cabf6147aec1d1c6af1f3a82736530cf3b067835fc8a09da092ce3`  
		Last Modified: Wed, 05 Oct 2022 00:04:36 GMT  
		Size: 50.2 MB (50209087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a49f93f990f17337480b5bdf526a6bb48d1ae63bd17f54be17cd2f6ebba4de7d`  
		Last Modified: Wed, 05 Oct 2022 00:53:28 GMT  
		Size: 4.9 MB (4931366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3989be0d7ed2f72fae0310039043f6ba76c24a45f9ec9689697ebd932845cc8`  
		Last Modified: Wed, 05 Oct 2022 00:53:28 GMT  
		Size: 10.2 MB (10217872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6487a2e4236617393a6184f0f89a360d295ab118da2ea4ad48fa8645ae211755`  
		Last Modified: Wed, 05 Oct 2022 00:53:57 GMT  
		Size: 50.3 MB (50343324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cb778b20f33d18ee7b4046bfd5685ddf5bb8750a2f3826f14408897c4d9db5`  
		Last Modified: Wed, 05 Oct 2022 00:54:45 GMT  
		Size: 167.3 MB (167303699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:bba56093d706c0b145e14ee726d81f59b1d09e069d3b84c30e9bee0af5a24687
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.2 MB (314172338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c2f1635631cecb5159531c9282693f4a86c19d02ec9f92e0f40baa073e51f5b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:45:55 GMT
ADD file:b16745ece8ef84c028d7e9ac4bf026ac64f885d4170bfcc9d435f237144a1b99 in / 
# Tue, 25 Oct 2022 05:45:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:58:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:58:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 07:59:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:00:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8e1d92e7d04d2a9a9880cb45dc3c32c2805912cd86abed96d0ada3ff28748205`  
		Last Modified: Tue, 25 Oct 2022 05:48:40 GMT  
		Size: 53.7 MB (53701966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66eadbf427bb41b3e329a95935c65b09c6d3b7a9c2fa8e08417e497df02ed996`  
		Last Modified: Tue, 25 Oct 2022 08:30:22 GMT  
		Size: 5.2 MB (5151506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9731f4e3bc3680179c10cece663cf0cfe0488918d6795406f4b76f07b787de`  
		Last Modified: Tue, 25 Oct 2022 08:30:22 GMT  
		Size: 10.9 MB (10874174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d337cb12fd7c6fe341850cd38e880f1806d49a65832c9804b06d00f9032382e0`  
		Last Modified: Tue, 25 Oct 2022 08:30:42 GMT  
		Size: 54.7 MB (54683990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a719597fe1ca78e1dc4c43fffc424754228514a791abcb0e0c06302ad022b8ca`  
		Last Modified: Tue, 25 Oct 2022 08:31:12 GMT  
		Size: 189.8 MB (189760702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; 386

```console
$ docker pull buildpack-deps@sha256:730efefe6d075835e0fede96affe8d8631d8212509b4c7003c32b47bf3c550b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.8 MB (327836520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d42762c45517dca640707932c4cfb4d4903431b010d2feb9a29f09b820a3ed5b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:22:19 GMT
ADD file:aa26f69b37c3e144d08e17bb9be7302ec89ae0579121c874a35f336d7077fd3b in / 
# Tue, 25 Oct 2022 02:22:19 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:15:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:15:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 05:15:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:16:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8caf426a2703f99fb0be4b03411ecaa580d102f7c47ef43b422b6d7c13c380e2`  
		Last Modified: Tue, 25 Oct 2022 02:27:54 GMT  
		Size: 56.0 MB (56023960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b92a2ff5c72653a0679aa7f5e2bc695011c0a71faa424229e560957d204dab`  
		Last Modified: Tue, 25 Oct 2022 05:27:37 GMT  
		Size: 5.1 MB (5086887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6856a3002e686ceb6d48d078731366f576ed3adcb73bd49dcb300057732904`  
		Last Modified: Tue, 25 Oct 2022 05:27:38 GMT  
		Size: 11.0 MB (11032526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e88080d3b5ba1edc8623a97d068bd040dfb89f2bc7bdfc0984d11fc35ff5885`  
		Last Modified: Tue, 25 Oct 2022 05:28:00 GMT  
		Size: 55.9 MB (55924404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b19879261038142328725a860507e23c40804ec5e04f1b7cf8f0dc88ded89d`  
		Last Modified: Tue, 25 Oct 2022 05:28:37 GMT  
		Size: 199.8 MB (199768743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:6088b9f6bed37906eecc152f8a3f642c5688b69f3c6c1ec283bd420ea0168585
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.1 MB (301112687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2991accb9ec37e952acae5a8759ce6006e7e1e39739799c51bab7c987e0d7867`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:09:48 GMT
ADD file:ca40db2df3dbc600910b8cd139c564cf5b8bd6c1a06cc517cae2c1c05cff6dde in / 
# Wed, 05 Oct 2022 00:09:51 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:11:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:12:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:14:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:19:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:25bcd35faf05f859c3077f0e2e7010d24e56cdcfb77efbdeda236e47dc08e14a`  
		Last Modified: Wed, 05 Oct 2022 00:17:52 GMT  
		Size: 53.3 MB (53265834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c44f381e4f9f5eb923a09cbd49bc86d3d36121137c1e063d30d73af518bf0f86`  
		Last Modified: Wed, 05 Oct 2022 01:32:02 GMT  
		Size: 4.9 MB (4918634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59260097f47eb21e87461a2a98c76f46372dd316b878bbd3d4d9c51cc28a62b7`  
		Last Modified: Wed, 05 Oct 2022 01:32:04 GMT  
		Size: 10.7 MB (10661237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f8a68e1316af16785650ca91231ed6373810fcdaff8fb5bec9f58e1ccc2a32`  
		Last Modified: Wed, 05 Oct 2022 01:32:53 GMT  
		Size: 53.3 MB (53304716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbf1a80df4f8f31f1ab3653fe8e3b40cb5a88a81ea4bc64c95e1b388fe7e2cc`  
		Last Modified: Wed, 05 Oct 2022 01:34:59 GMT  
		Size: 179.0 MB (178962266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:39252f001a267e36e8cc4cbd5a51b22eb6f6b8c862a0eebae0f84c115268f828
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.0 MB (331028350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fe0aa4188607937a62728cb0c6bb7d668f569b3384fecff44935b02408e9068`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:13:28 GMT
ADD file:c01a6cc4222fbeeda5c2d679c5b355539880a02c792c64861eb17b81a3678f45 in / 
# Tue, 25 Oct 2022 03:13:31 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:13:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:14:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:14:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:16:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ee5a342763ed1d31bef8cebe9f4cc5dd6d427f630da679a87da0427be7b22e3d`  
		Last Modified: Tue, 25 Oct 2022 03:18:52 GMT  
		Size: 58.9 MB (58916374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a4727f39cbcb19b39abdbd847eeceed842ef65f8514372024c48b913bc951a`  
		Last Modified: Tue, 25 Oct 2022 06:49:00 GMT  
		Size: 5.4 MB (5414507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe601e6c8a1ec9c69c49c65a53339202a65cea9d4f01d161fb34905c06a4a99`  
		Last Modified: Tue, 25 Oct 2022 06:49:01 GMT  
		Size: 11.6 MB (11630153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5055e27b58426c2b637b1c8c179e6abe306e3dfb55a9c170c73fb0d581c6cf3e`  
		Last Modified: Tue, 25 Oct 2022 06:49:31 GMT  
		Size: 58.9 MB (58867355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a503b0a90ce32a745c9586bc6c28360d8de222565d7105d079b530524e1e38`  
		Last Modified: Tue, 25 Oct 2022 06:50:32 GMT  
		Size: 196.2 MB (196199961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:56a7b6a421aea89e44c16d6526e1f2688c8b129fae975687ccdef4707e507432
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.1 MB (296088034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:172dabba1a37b7c132ad4884aca1fd3c1b63d62e29533b09589ac174b5c3f0f7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:14:24 GMT
ADD file:06f15d8a3c04752d271a052e820fb13fcdb76f0d18f6c9afb6e70391d10348ec in / 
# Tue, 25 Oct 2022 01:14:27 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:31:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:31:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 02:31:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:32:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a556186e8bea4ba9925d0c17bea2c12bfbb931653cfab1b980036800482cf0ad`  
		Last Modified: Tue, 25 Oct 2022 01:18:39 GMT  
		Size: 53.3 MB (53279106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1e8478a953d3a464d73e36e4032c979725bc79ce0eeb83aca30212de549b90`  
		Last Modified: Tue, 25 Oct 2022 02:49:32 GMT  
		Size: 5.1 MB (5148477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cdbee45ed722bfaf7e9ba90503afa7a0cf17b87fc1bfa1e87cbf49ca6bd7d9`  
		Last Modified: Tue, 25 Oct 2022 02:49:33 GMT  
		Size: 10.8 MB (10766704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76aacd12f54fec6c8f627f09641ea144eb6fefeebc8f9fc35de80c3e3ab11af7`  
		Last Modified: Tue, 25 Oct 2022 02:49:48 GMT  
		Size: 54.1 MB (54055853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f33c726ca8131121c45361c5d4789cbb8c58f1cf53f551af6b41f3857cb9847`  
		Last Modified: Tue, 25 Oct 2022 02:50:20 GMT  
		Size: 172.8 MB (172837894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldstable`

```console
$ docker pull buildpack-deps@sha256:23c324efadf9febfe2d46da3a96f2076678e8ad195ca7e84d328efd29ada237e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:oldstable` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:9bc85b7b437bfb4388f7160a92e96c24ff5591134dfcc45b5ce939c25923b81a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.6 MB (312646449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f94fc706b3e93d2101993d24cf5d6da5fb762d5475a4b62407e77f8a58088e35`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:56:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:57:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:58:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6315e893372434bf09990677f857fdd026ba0abdd98d435decc2ec5742cee4`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 7.9 MB (7857339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad12dd0da3ea9c59f4c4fc53d6a204e11e2930b9dc4143376024ed8fa5c71bb`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 10.0 MB (9998384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a0ceb4387f59959418bd2da17176107c9ce0ea542cf017ce14835999fa8437`  
		Last Modified: Wed, 05 Oct 2022 01:20:41 GMT  
		Size: 51.8 MB (51844142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0ae5ed3318e8db87d129f9c2652dddc78c89f223625a345ec1b7b84149a882`  
		Last Modified: Wed, 05 Oct 2022 01:21:16 GMT  
		Size: 192.5 MB (192505482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:2e18f1ba0b34255fb800df33fe54f2839e518f98e93129aa8fd87bd702595a12
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.5 MB (278453016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:332432940790fb96e3fd3a0b74f46e3a7df64c05ef7f1204784d6612c1896616`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:59:00 GMT
ADD file:b16f07fda9b8beecd7c275565d0ed135fb298c712482766c8f0e40fac932130c in / 
# Tue, 04 Oct 2022 23:59:01 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:34:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:35:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:35:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:37:59 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bba3a5db4dfa403d6e1db947629616e80fb4514e2190e6aa1fb6a2c828c32491`  
		Last Modified: Wed, 05 Oct 2022 00:05:35 GMT  
		Size: 45.9 MB (45914973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0469c30b40a2c26072c228ab2795c38de425870b9ee85d29a32a2f50db3c4f`  
		Last Modified: Wed, 05 Oct 2022 00:55:03 GMT  
		Size: 7.1 MB (7145345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5315d494a34df967f8f4db548d0b40754c70678b9357188c65dc0b9cfee4f7e`  
		Last Modified: Wed, 05 Oct 2022 00:55:03 GMT  
		Size: 9.3 MB (9344666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317e83f2e93982c08cca0dc1dc3456b7bdfa7cdc43011e894195ad828de7550c`  
		Last Modified: Wed, 05 Oct 2022 00:55:25 GMT  
		Size: 47.4 MB (47363676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2771890b0a61f6c6c34e9aa3b58a50e0cf5b1ac46cf3ddcfe77c70fc410d9d16`  
		Last Modified: Wed, 05 Oct 2022 00:56:10 GMT  
		Size: 168.7 MB (168684356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:4a600eea362e0bb4e0778ac365824e178ff6971f0eb2793d531a21927238697d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.2 MB (303229234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e913c5bd9a75ab5fa70ca778c3b9e620e92e01cd05ea666ccd918794ed90efd5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:07 GMT
ADD file:21afa32c0395cc5046d09741d6821d21cfd9b77bce46ebcfc8fd9aca57c73648 in / 
# Tue, 25 Oct 2022 05:46:08 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:00:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:00:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:01:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3ba81f4c3c21f92780061ee116827d64ac4edbcd02b056845c2aaa3097b730ed`  
		Last Modified: Tue, 25 Oct 2022 05:49:24 GMT  
		Size: 49.2 MB (49233280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5909a8b8cad57ca90fe69eaa8b350c722b820753f9caaa1f528f2337a71f38`  
		Last Modified: Tue, 25 Oct 2022 08:31:26 GMT  
		Size: 7.7 MB (7726424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a633475baeae1eb12baa14cc54f130d1e37ea520470ee16bb2dd23d779d08b4b`  
		Last Modified: Tue, 25 Oct 2022 08:31:25 GMT  
		Size: 10.0 MB (10003562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f22a2b8ddcb8bb5d37d3cd14e13998148d107dc8eb1d7c57c3220c1915fd9d1`  
		Last Modified: Tue, 25 Oct 2022 08:31:41 GMT  
		Size: 52.2 MB (52172864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985dd0945ed8d7e2674a61279668f6edeac4dc80a4a6a517fd01736884e37951`  
		Last Modified: Tue, 25 Oct 2022 08:32:08 GMT  
		Size: 184.1 MB (184093104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:986002256185ea6e031552f9961c582f79bc59cfd0480c91dc617e385c631089
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.8 MB (321844428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbf287ecacbd32c06e7567a97fa798639352e1b8ebee00ba2d94c64cebeee1c6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:22:47 GMT
ADD file:7e14d4afa5499129c959c5ae5dc270e2fa04659c2c9b0527094cda3494c02d0f in / 
# Tue, 25 Oct 2022 02:22:47 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:16:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:16:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 05:17:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:18:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76a731c42f665e7334a622f65117ef9389e97a878b7c74bb4a10dfe9cdb296c6`  
		Last Modified: Tue, 25 Oct 2022 02:28:50 GMT  
		Size: 51.2 MB (51207943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee1fc3722feabf994120ab8f7d4abab754206d1ca425b7274ce1db428f7a651`  
		Last Modified: Tue, 25 Oct 2022 05:28:54 GMT  
		Size: 8.0 MB (8025806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2019db6202a77d9f3c2e49a64c766b8b67d4290e0e66e1480fd8c576078914b2`  
		Last Modified: Tue, 25 Oct 2022 05:28:54 GMT  
		Size: 10.1 MB (10128021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79afff7d2fb8bbf10afd83b8f08278ed493a12e50a8262a18a1b3fc227667ec4`  
		Last Modified: Tue, 25 Oct 2022 05:29:13 GMT  
		Size: 53.4 MB (53442950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9206c74214dfb44ab3f4b75a12fcb6bf38c7e04c253e88ff3af265d2e33152f4`  
		Last Modified: Tue, 25 Oct 2022 05:29:47 GMT  
		Size: 199.0 MB (199039708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldstable-curl`

```console
$ docker pull buildpack-deps@sha256:97a9679f1baca57d6622f9e8757d4539e82686724aec4f5b48ba04bf854a9e00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:oldstable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:7f3fca26e9b1bb3ec6998a1a523cf586a2367e52c1231cdbe8bb4aaf8e8db8f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68296825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86d0d53a4b39e141ed1bb691a10b424c3dec11acdd8a74caad8dd92781d9be08`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:56:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6315e893372434bf09990677f857fdd026ba0abdd98d435decc2ec5742cee4`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 7.9 MB (7857339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad12dd0da3ea9c59f4c4fc53d6a204e11e2930b9dc4143376024ed8fa5c71bb`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 10.0 MB (9998384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:5cd59ddd6b9c9a97edda3c72bdcad4b5066c14becf62e1671a3d0941e6d67a9b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62404984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d022800d5a11e049d7a055e547960321c510573aabb0a90de07cb297f8f7d306`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:59:00 GMT
ADD file:b16f07fda9b8beecd7c275565d0ed135fb298c712482766c8f0e40fac932130c in / 
# Tue, 04 Oct 2022 23:59:01 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:34:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:35:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:bba3a5db4dfa403d6e1db947629616e80fb4514e2190e6aa1fb6a2c828c32491`  
		Last Modified: Wed, 05 Oct 2022 00:05:35 GMT  
		Size: 45.9 MB (45914973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0469c30b40a2c26072c228ab2795c38de425870b9ee85d29a32a2f50db3c4f`  
		Last Modified: Wed, 05 Oct 2022 00:55:03 GMT  
		Size: 7.1 MB (7145345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5315d494a34df967f8f4db548d0b40754c70678b9357188c65dc0b9cfee4f7e`  
		Last Modified: Wed, 05 Oct 2022 00:55:03 GMT  
		Size: 9.3 MB (9344666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:62e0978b8f23b168926fbaa2c7e965afe1b8c2f9425020b970f07a341589c10d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (66963266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ef5471fe2492bddb3a059378a30108a47836397b595e088e8385b2232a05668`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:07 GMT
ADD file:21afa32c0395cc5046d09741d6821d21cfd9b77bce46ebcfc8fd9aca57c73648 in / 
# Tue, 25 Oct 2022 05:46:08 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:00:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3ba81f4c3c21f92780061ee116827d64ac4edbcd02b056845c2aaa3097b730ed`  
		Last Modified: Tue, 25 Oct 2022 05:49:24 GMT  
		Size: 49.2 MB (49233280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5909a8b8cad57ca90fe69eaa8b350c722b820753f9caaa1f528f2337a71f38`  
		Last Modified: Tue, 25 Oct 2022 08:31:26 GMT  
		Size: 7.7 MB (7726424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a633475baeae1eb12baa14cc54f130d1e37ea520470ee16bb2dd23d779d08b4b`  
		Last Modified: Tue, 25 Oct 2022 08:31:25 GMT  
		Size: 10.0 MB (10003562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:141fff8c2ffcc8259e3a47678ed76429a31d347a408e2f2f0888e736c49898dd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69361770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff4a03bb5b5ce0fe0aa8976c8784fc059747d3be27552c0f8e0fe675b0862c4d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:22:47 GMT
ADD file:7e14d4afa5499129c959c5ae5dc270e2fa04659c2c9b0527094cda3494c02d0f in / 
# Tue, 25 Oct 2022 02:22:47 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:16:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:16:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:76a731c42f665e7334a622f65117ef9389e97a878b7c74bb4a10dfe9cdb296c6`  
		Last Modified: Tue, 25 Oct 2022 02:28:50 GMT  
		Size: 51.2 MB (51207943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee1fc3722feabf994120ab8f7d4abab754206d1ca425b7274ce1db428f7a651`  
		Last Modified: Tue, 25 Oct 2022 05:28:54 GMT  
		Size: 8.0 MB (8025806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2019db6202a77d9f3c2e49a64c766b8b67d4290e0e66e1480fd8c576078914b2`  
		Last Modified: Tue, 25 Oct 2022 05:28:54 GMT  
		Size: 10.1 MB (10128021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldstable-scm`

```console
$ docker pull buildpack-deps@sha256:a590ddff46a58a462abeb4c8d37ca4fcb4d0d2925cdbef377d1b09601e9fa644
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:oldstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:0fc5aaca490caf0a79503055fbc391b8853d761d5a03215be8be60f41e47e8aa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120140967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59e413a2b1e4e2663e043d48670e90c2884b194881af04864d37af34f210e6ce`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:56:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:57:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6315e893372434bf09990677f857fdd026ba0abdd98d435decc2ec5742cee4`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 7.9 MB (7857339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad12dd0da3ea9c59f4c4fc53d6a204e11e2930b9dc4143376024ed8fa5c71bb`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 10.0 MB (9998384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a0ceb4387f59959418bd2da17176107c9ce0ea542cf017ce14835999fa8437`  
		Last Modified: Wed, 05 Oct 2022 01:20:41 GMT  
		Size: 51.8 MB (51844142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1c44d4c649674b9e3e229b526b0a8c64d775b37ca77c49712dab1a29b053322c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109768660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a258170ac7140810e8320dd1407b51e91999966c0044a20c68c66fe1ea0b5f1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:59:00 GMT
ADD file:b16f07fda9b8beecd7c275565d0ed135fb298c712482766c8f0e40fac932130c in / 
# Tue, 04 Oct 2022 23:59:01 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:34:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:35:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:35:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bba3a5db4dfa403d6e1db947629616e80fb4514e2190e6aa1fb6a2c828c32491`  
		Last Modified: Wed, 05 Oct 2022 00:05:35 GMT  
		Size: 45.9 MB (45914973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0469c30b40a2c26072c228ab2795c38de425870b9ee85d29a32a2f50db3c4f`  
		Last Modified: Wed, 05 Oct 2022 00:55:03 GMT  
		Size: 7.1 MB (7145345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5315d494a34df967f8f4db548d0b40754c70678b9357188c65dc0b9cfee4f7e`  
		Last Modified: Wed, 05 Oct 2022 00:55:03 GMT  
		Size: 9.3 MB (9344666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317e83f2e93982c08cca0dc1dc3456b7bdfa7cdc43011e894195ad828de7550c`  
		Last Modified: Wed, 05 Oct 2022 00:55:25 GMT  
		Size: 47.4 MB (47363676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:9f6e569fb46b186c92f83439bc018e32747d464f7d9b2d8807c7416ef1b64a75
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.1 MB (119136130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:609ea79261cd59e82ef55f8c7c01da32dcad5b2ba53f83090793c43285265b76`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:07 GMT
ADD file:21afa32c0395cc5046d09741d6821d21cfd9b77bce46ebcfc8fd9aca57c73648 in / 
# Tue, 25 Oct 2022 05:46:08 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:00:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:00:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3ba81f4c3c21f92780061ee116827d64ac4edbcd02b056845c2aaa3097b730ed`  
		Last Modified: Tue, 25 Oct 2022 05:49:24 GMT  
		Size: 49.2 MB (49233280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5909a8b8cad57ca90fe69eaa8b350c722b820753f9caaa1f528f2337a71f38`  
		Last Modified: Tue, 25 Oct 2022 08:31:26 GMT  
		Size: 7.7 MB (7726424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a633475baeae1eb12baa14cc54f130d1e37ea520470ee16bb2dd23d779d08b4b`  
		Last Modified: Tue, 25 Oct 2022 08:31:25 GMT  
		Size: 10.0 MB (10003562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f22a2b8ddcb8bb5d37d3cd14e13998148d107dc8eb1d7c57c3220c1915fd9d1`  
		Last Modified: Tue, 25 Oct 2022 08:31:41 GMT  
		Size: 52.2 MB (52172864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:72528f8ffef6e01ca828a63747681ae454b493b4005d786376fa35f432a95d55
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.8 MB (122804720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81b4069d89bb74ef0eca45c2e785bf7ba4d17172c93d68cd25f65cbd17f76d46`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:22:47 GMT
ADD file:7e14d4afa5499129c959c5ae5dc270e2fa04659c2c9b0527094cda3494c02d0f in / 
# Tue, 25 Oct 2022 02:22:47 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:16:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:16:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 05:17:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76a731c42f665e7334a622f65117ef9389e97a878b7c74bb4a10dfe9cdb296c6`  
		Last Modified: Tue, 25 Oct 2022 02:28:50 GMT  
		Size: 51.2 MB (51207943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee1fc3722feabf994120ab8f7d4abab754206d1ca425b7274ce1db428f7a651`  
		Last Modified: Tue, 25 Oct 2022 05:28:54 GMT  
		Size: 8.0 MB (8025806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2019db6202a77d9f3c2e49a64c766b8b67d4290e0e66e1480fd8c576078914b2`  
		Last Modified: Tue, 25 Oct 2022 05:28:54 GMT  
		Size: 10.1 MB (10128021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79afff7d2fb8bbf10afd83b8f08278ed493a12e50a8262a18a1b3fc227667ec4`  
		Last Modified: Tue, 25 Oct 2022 05:29:13 GMT  
		Size: 53.4 MB (53442950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:scm`

```console
$ docker pull buildpack-deps@sha256:a7f1c200cd1fd667d3fec5bd3b69dd3672603ce21b7b67891fb7d3a5218874e2
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
$ docker pull buildpack-deps@sha256:fd04e21a45663223207243344f0ac8b1d9c0fe01b1b8601b25d5686a0fdbaa2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125670325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82ff4917fce4dadc637924ff195fcebb04273691c7152bcc869fb766c88d8e15`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:27 GMT
ADD file:d1268789456d2cdace6e50149e60404ad5a849b7c61e8fc8bc7b6e0eb6eeb7ca in / 
# Tue, 04 Oct 2022 23:26:27 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:54:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:55:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:55:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f606d8928ed378229f2460b94b504cca239fb906efc57acbdf9340bd298d5ddf`  
		Last Modified: Tue, 04 Oct 2022 23:30:27 GMT  
		Size: 55.0 MB (55046248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47db815c6a4547dc224b75222193cb1851cf529d2cbdf26f854b9bbf97099b98`  
		Last Modified: Wed, 05 Oct 2022 01:19:13 GMT  
		Size: 5.2 MB (5163279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf48494000001a037b72870d2a6a2536f9da8bc5d1ceddd72d79f4a51fe7a60e`  
		Last Modified: Wed, 05 Oct 2022 01:19:13 GMT  
		Size: 10.9 MB (10876505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a572f7a256d36a93ab0777949771b120c5d7dce75ea2a2d3d9444793b26b2ef1`  
		Last Modified: Wed, 05 Oct 2022 01:19:34 GMT  
		Size: 54.6 MB (54584293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:b510585c7c0379882b7436c2ba9f2bcdf9fa4cadd1aa9e71b177f1bb9bcc57e5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.5 MB (120516144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b46050aede040f8a40b0df16c1d9ec4720cde12aeb7b220cd6ac40588a3ddeb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:06:19 GMT
ADD file:b314b98654e8532fd10a08a172ea5c3edb7d7a36c7faf85d06d14be12f7b83ef in / 
# Tue, 25 Oct 2022 03:06:19 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:12:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:12:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:12:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1f0ecb08923b99bef3f82c2e88603bb53e3ed084c13252275c05039cc279c158`  
		Last Modified: Tue, 25 Oct 2022 03:11:15 GMT  
		Size: 52.5 MB (52547473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b399c5eb53b4c35fa33682a82d73bdc4b096cd78ae95fe36c4ed81d18f6849`  
		Last Modified: Tue, 25 Oct 2022 06:19:02 GMT  
		Size: 5.1 MB (5072235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ccdd06393cd3873a3cc8b9cbe170a2032fd61d1d545b7045b649faf2f4e732`  
		Last Modified: Tue, 25 Oct 2022 06:19:02 GMT  
		Size: 10.6 MB (10574279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aafe0e287af4e488dcda51195e4eb1ae1386e3265989c457172f32f6357bf26`  
		Last Modified: Tue, 25 Oct 2022 06:19:28 GMT  
		Size: 52.3 MB (52322157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:50a85a985b089ddf5972b836da6a0053b066b489827aa55bac5f7bec2bf93ffa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.7 MB (115701649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30f987ffe03e99e4f18811a3ed9c6b544fa00393058f4ef2abb83df5bc1d7673`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:28 GMT
ADD file:47a3f2948af18c39686ca59a88a439c25edaf286064d3a2ccc5dab47fee2fc52 in / 
# Tue, 04 Oct 2022 23:58:29 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:32:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:32:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:32:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e19342fb46cabf6147aec1d1c6af1f3a82736530cf3b067835fc8a09da092ce3`  
		Last Modified: Wed, 05 Oct 2022 00:04:36 GMT  
		Size: 50.2 MB (50209087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a49f93f990f17337480b5bdf526a6bb48d1ae63bd17f54be17cd2f6ebba4de7d`  
		Last Modified: Wed, 05 Oct 2022 00:53:28 GMT  
		Size: 4.9 MB (4931366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3989be0d7ed2f72fae0310039043f6ba76c24a45f9ec9689697ebd932845cc8`  
		Last Modified: Wed, 05 Oct 2022 00:53:28 GMT  
		Size: 10.2 MB (10217872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6487a2e4236617393a6184f0f89a360d295ab118da2ea4ad48fa8645ae211755`  
		Last Modified: Wed, 05 Oct 2022 00:53:57 GMT  
		Size: 50.3 MB (50343324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:8b048c050c2a3ff92ba38fbbe2ceb6d4523c5c2d90dc3ef032dbe78ce741b7c5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124411636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c203e5804baca6a5e5ee110aa8b5c855e1af7aa5b84d282751a6ee78a938f3e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:45:55 GMT
ADD file:b16745ece8ef84c028d7e9ac4bf026ac64f885d4170bfcc9d435f237144a1b99 in / 
# Tue, 25 Oct 2022 05:45:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:58:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:58:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 07:59:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8e1d92e7d04d2a9a9880cb45dc3c32c2805912cd86abed96d0ada3ff28748205`  
		Last Modified: Tue, 25 Oct 2022 05:48:40 GMT  
		Size: 53.7 MB (53701966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66eadbf427bb41b3e329a95935c65b09c6d3b7a9c2fa8e08417e497df02ed996`  
		Last Modified: Tue, 25 Oct 2022 08:30:22 GMT  
		Size: 5.2 MB (5151506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9731f4e3bc3680179c10cece663cf0cfe0488918d6795406f4b76f07b787de`  
		Last Modified: Tue, 25 Oct 2022 08:30:22 GMT  
		Size: 10.9 MB (10874174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d337cb12fd7c6fe341850cd38e880f1806d49a65832c9804b06d00f9032382e0`  
		Last Modified: Tue, 25 Oct 2022 08:30:42 GMT  
		Size: 54.7 MB (54683990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:af3f07f28271542b5cad16677fb8b3eca0cf0897adac022669fd5d2aabbf004d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.1 MB (128067777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41c2e7cc3bce85c55d7b854c187796f854d5d152784c6759eaa5aa5c6dbdc665`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:22:19 GMT
ADD file:aa26f69b37c3e144d08e17bb9be7302ec89ae0579121c874a35f336d7077fd3b in / 
# Tue, 25 Oct 2022 02:22:19 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:15:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:15:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 05:15:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8caf426a2703f99fb0be4b03411ecaa580d102f7c47ef43b422b6d7c13c380e2`  
		Last Modified: Tue, 25 Oct 2022 02:27:54 GMT  
		Size: 56.0 MB (56023960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b92a2ff5c72653a0679aa7f5e2bc695011c0a71faa424229e560957d204dab`  
		Last Modified: Tue, 25 Oct 2022 05:27:37 GMT  
		Size: 5.1 MB (5086887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6856a3002e686ceb6d48d078731366f576ed3adcb73bd49dcb300057732904`  
		Last Modified: Tue, 25 Oct 2022 05:27:38 GMT  
		Size: 11.0 MB (11032526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e88080d3b5ba1edc8623a97d068bd040dfb89f2bc7bdfc0984d11fc35ff5885`  
		Last Modified: Tue, 25 Oct 2022 05:28:00 GMT  
		Size: 55.9 MB (55924404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:a1acaa6746ce03d5ac1c9c184b9983adf517c0cc252294f448e9e9c51580b9c7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122150421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfa73d3a5551fa701da480cd6d0b3d216e9aace1ea0d1de8201cd9fe13f05ce5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:09:48 GMT
ADD file:ca40db2df3dbc600910b8cd139c564cf5b8bd6c1a06cc517cae2c1c05cff6dde in / 
# Wed, 05 Oct 2022 00:09:51 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:11:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:12:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:14:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:25bcd35faf05f859c3077f0e2e7010d24e56cdcfb77efbdeda236e47dc08e14a`  
		Last Modified: Wed, 05 Oct 2022 00:17:52 GMT  
		Size: 53.3 MB (53265834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c44f381e4f9f5eb923a09cbd49bc86d3d36121137c1e063d30d73af518bf0f86`  
		Last Modified: Wed, 05 Oct 2022 01:32:02 GMT  
		Size: 4.9 MB (4918634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59260097f47eb21e87461a2a98c76f46372dd316b878bbd3d4d9c51cc28a62b7`  
		Last Modified: Wed, 05 Oct 2022 01:32:04 GMT  
		Size: 10.7 MB (10661237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f8a68e1316af16785650ca91231ed6373810fcdaff8fb5bec9f58e1ccc2a32`  
		Last Modified: Wed, 05 Oct 2022 01:32:53 GMT  
		Size: 53.3 MB (53304716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:aa6dce1df8020e1e65a5969cd4d256313e3e6bf82526d3774527163c0d3d6b6f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134828389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd50ae9ad837d99d2a9f89b2818813787249d3ea2cd98a78affb4ac0a45caa6d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:13:28 GMT
ADD file:c01a6cc4222fbeeda5c2d679c5b355539880a02c792c64861eb17b81a3678f45 in / 
# Tue, 25 Oct 2022 03:13:31 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:13:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:14:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:14:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ee5a342763ed1d31bef8cebe9f4cc5dd6d427f630da679a87da0427be7b22e3d`  
		Last Modified: Tue, 25 Oct 2022 03:18:52 GMT  
		Size: 58.9 MB (58916374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a4727f39cbcb19b39abdbd847eeceed842ef65f8514372024c48b913bc951a`  
		Last Modified: Tue, 25 Oct 2022 06:49:00 GMT  
		Size: 5.4 MB (5414507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe601e6c8a1ec9c69c49c65a53339202a65cea9d4f01d161fb34905c06a4a99`  
		Last Modified: Tue, 25 Oct 2022 06:49:01 GMT  
		Size: 11.6 MB (11630153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5055e27b58426c2b637b1c8c179e6abe306e3dfb55a9c170c73fb0d581c6cf3e`  
		Last Modified: Tue, 25 Oct 2022 06:49:31 GMT  
		Size: 58.9 MB (58867355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:eba01f860d7d3264a146b7ec7242b3002fd04f91a81d12f89260377ac201f374
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.3 MB (123250140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d21933a18810ed510258d911e9f0408303556697f423746d2ecbcdb6d9df700`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:14:24 GMT
ADD file:06f15d8a3c04752d271a052e820fb13fcdb76f0d18f6c9afb6e70391d10348ec in / 
# Tue, 25 Oct 2022 01:14:27 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:31:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:31:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 02:31:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a556186e8bea4ba9925d0c17bea2c12bfbb931653cfab1b980036800482cf0ad`  
		Last Modified: Tue, 25 Oct 2022 01:18:39 GMT  
		Size: 53.3 MB (53279106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1e8478a953d3a464d73e36e4032c979725bc79ce0eeb83aca30212de549b90`  
		Last Modified: Tue, 25 Oct 2022 02:49:32 GMT  
		Size: 5.1 MB (5148477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cdbee45ed722bfaf7e9ba90503afa7a0cf17b87fc1bfa1e87cbf49ca6bd7d9`  
		Last Modified: Tue, 25 Oct 2022 02:49:33 GMT  
		Size: 10.8 MB (10766704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76aacd12f54fec6c8f627f09641ea144eb6fefeebc8f9fc35de80c3e3ab11af7`  
		Last Modified: Tue, 25 Oct 2022 02:49:48 GMT  
		Size: 54.1 MB (54055853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:sid`

```console
$ docker pull buildpack-deps@sha256:37ddbe39fcb9a1fe2dd11c2f9b2ce45d101b51ae6228ffd1825f50fe435a49a3
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
$ docker pull buildpack-deps@sha256:a5c9c277142466a2cb13602a341189d974508866b334634253b4cd510d06669b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.9 MB (351931474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b61eb60b50a71a4c3e73ad9d3d992525ea6f399f1983ef31929b5d74b86a19a9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:27:32 GMT
ADD file:b2f29ff1f75077ccce680becaa7bffdc9dfb9c7938188e93673e1b42bf418630 in / 
# Tue, 04 Oct 2022 23:27:32 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:58:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:59:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:59:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:00:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a9fedee3000f9dcc2b77410cd53420ec321135a3f7a6c688b43f31e503042e1e`  
		Last Modified: Tue, 04 Oct 2022 23:32:34 GMT  
		Size: 52.7 MB (52684279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dda17d2d1d2961ba6c7083d3013dde5fb5af68bd80ee1e40adbf7886b64df3c`  
		Last Modified: Wed, 05 Oct 2022 01:21:27 GMT  
		Size: 9.3 MB (9300772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809d617f2e2db52d55fec066a28a409d69e1dc40dd9f91f7f03c19ec8d16c587`  
		Last Modified: Wed, 05 Oct 2022 01:21:27 GMT  
		Size: 11.4 MB (11382118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15dd69568329cc8f49552e84cc7a6c0a0c112efb493830d52d7c1c6ed88af8f`  
		Last Modified: Wed, 05 Oct 2022 01:21:45 GMT  
		Size: 58.1 MB (58052906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5107ea815e7c65b0f723ec6d8f3b5ed3eb7461e8f79537b8c5e719f0a4b7ae59`  
		Last Modified: Wed, 05 Oct 2022 01:22:23 GMT  
		Size: 220.5 MB (220511399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:053914e76c7ba60fb11f8cc6b92d31100985ad00c304f22cdbd935f9d1ce6d11
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.4 MB (309384964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20043e26391a12bbe81aaa2a4a2e9f2aca2ae66853c067fdbe991c88c12d0d99`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:06:50 GMT
ADD file:829f8e96e527611e85aa710b19c01c75a4760a27c651fb439f8cdb5609db64aa in / 
# Tue, 25 Oct 2022 03:06:52 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:14:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:14:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:15:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:16:24 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:513ea4862e78a8cc07ed6d320f10e746ca770eb039dec1548c31a9de19d1f7ce`  
		Last Modified: Tue, 25 Oct 2022 03:12:19 GMT  
		Size: 49.6 MB (49578888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1ace4b71d48c3105e8f55674a41898f6b1df73d7ee8b05d5c3d3b3fea66077`  
		Last Modified: Tue, 25 Oct 2022 06:20:29 GMT  
		Size: 8.5 MB (8548544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:428ee02803cd3666baa3051b15b273e86d1d20710ddd79191fb1367a0dda5edc`  
		Last Modified: Tue, 25 Oct 2022 06:20:29 GMT  
		Size: 10.8 MB (10829764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecfb58f8aebfa286f964add0eb9b5f5bf243c4e6b5c934809df2c000acf0301c`  
		Last Modified: Tue, 25 Oct 2022 06:20:53 GMT  
		Size: 55.5 MB (55547745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f507c760cb7666ec153f5bbf4e7065ca52ffbd950406148854ca9ac024d521d1`  
		Last Modified: Tue, 25 Oct 2022 06:21:36 GMT  
		Size: 184.9 MB (184880023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:50db74bb547c5b2b61e9d0061572cf34d1f9a2691617b0af1f821bfee6452528
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.9 MB (305910529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae94c0dd0c97e61628259977275ebed18a549a46b30661e06c76d8622bde7b47`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:00:01 GMT
ADD file:41046e966f37a45410c2aa02920b78f877f5aacb6ee087b2c6c6642f4e7b474f in / 
# Wed, 05 Oct 2022 00:00:02 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:38:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:38:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:38:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:40:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1316bf5b10f256f27feadcb25edef6365e912773e60cc382610ef003daf37248`  
		Last Modified: Wed, 05 Oct 2022 00:07:10 GMT  
		Size: 49.4 MB (49436823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00270159c4caaec159e25e1eaca6209b11c838dd60b5e0f5194e2279c51cd70`  
		Last Modified: Wed, 05 Oct 2022 00:56:26 GMT  
		Size: 8.4 MB (8399366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8524fd9b0e923155334b98a655b41aa941eb210e3248b7cc375ee49257b2b929`  
		Last Modified: Wed, 05 Oct 2022 00:56:26 GMT  
		Size: 10.7 MB (10663790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92867f6312a37ef5d4d5b38b1944bbe65123c5127a3ace08db615300dfc442c7`  
		Last Modified: Wed, 05 Oct 2022 00:56:52 GMT  
		Size: 53.7 MB (53727748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a7e6fabe704d47681c59355edf9f588b8d1c66996c09a34a3fdb7c42e27a75`  
		Last Modified: Wed, 05 Oct 2022 00:57:45 GMT  
		Size: 183.7 MB (183682802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:b082ee07bc085a1f3753080188e9d8260690c44559ba4829f3bde8da53717a5a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.7 MB (330710877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a3c24ba1239020d15937993d74b20ef109f76f653bb0f857613a9ab6ccb9b80`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:29 GMT
ADD file:6a2d69a5a731490271c915d99634a89755f7236ef56712924ea061730d8552c4 in / 
# Tue, 25 Oct 2022 05:46:30 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:01:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:01:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:02:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:03:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:63a396bb133ce57141398b6c6d776ce17e3e973085b5a1b746d76407240a376a`  
		Last Modified: Tue, 25 Oct 2022 05:50:38 GMT  
		Size: 50.6 MB (50643735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a89cf1bf3c8da06b08672e8551d2511df312e843fb3acab24e31d9ba0afa866`  
		Last Modified: Tue, 25 Oct 2022 08:32:19 GMT  
		Size: 8.9 MB (8932959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e653e6dd7e514d68792b5ac0d2812dbc50a0e1d5c4842fd356c767031c54aec`  
		Last Modified: Tue, 25 Oct 2022 08:32:19 GMT  
		Size: 11.1 MB (11138995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c34d6a76d061ba3fc92256f8a3d68cb9c3d5840430072a886deb01b71229ceba`  
		Last Modified: Tue, 25 Oct 2022 08:32:40 GMT  
		Size: 57.7 MB (57715979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb1960dcbb4deabd508cdae7441ee09f50ac6dbb89cea1922d94adc49db752e`  
		Last Modified: Tue, 25 Oct 2022 08:33:09 GMT  
		Size: 202.3 MB (202279209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; 386

```console
$ docker pull buildpack-deps@sha256:5bd7bb5803c4f0ad919619492abe354c5ff051233d1fd15ab0b702dcd2fc099e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.9 MB (343886877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:881b4643c019f8a58e6490838d5a8ad00df910743f87b1a3e581433aa83888b0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:23:38 GMT
ADD file:80dabb60a37b1d88f3750adb85c9e159d00b55293f70ad93512f94bd3cfd99bc in / 
# Tue, 25 Oct 2022 02:23:39 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:18:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:18:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 05:19:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:20:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:367799113badd94b9683087d6086436649a1fb7127698c42b0d730f5bbedcf86`  
		Last Modified: Tue, 25 Oct 2022 02:30:22 GMT  
		Size: 51.6 MB (51625321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564d2fccc59969c0b37e3bb8384bc6545a4cce125daa11c7e8b599ec0acac788`  
		Last Modified: Tue, 25 Oct 2022 05:30:00 GMT  
		Size: 9.3 MB (9282393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09be9213196e288bdcccf553107591d6fe4f04fccea4da55faea35dd79cfff15`  
		Last Modified: Tue, 25 Oct 2022 05:30:00 GMT  
		Size: 11.4 MB (11379737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7cf8ff2ca1128a94c435416195c01bd46e7b32191a4a225527692f374d4e31e`  
		Last Modified: Tue, 25 Oct 2022 05:30:21 GMT  
		Size: 59.5 MB (59473844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d348a2548fad4997feadc2b7be7e32cc9412c27e3208c57b624b3263c3c096c3`  
		Last Modified: Tue, 25 Oct 2022 05:30:57 GMT  
		Size: 212.1 MB (212125582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:2caaf8b43b29ccbbe6df934dfce764b42a555f9dfc7c3e1a3cc7bf2a9100d322
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.9 MB (326920922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a616d7e3db3ce0164a507b56b89952f874fd85d67230fa9a2a34798f0270ae98`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:11:00 GMT
ADD file:a7d6f7226093388fbc662c6e3fa1bc8dc263ab630fe03ea088486e6b016474ff in / 
# Wed, 05 Oct 2022 00:11:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:20:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:21:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:22:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:28:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3110bff10f823ecdaa06d8f7c65ce83d7c99521680207da9d264aaa8823d5209`  
		Last Modified: Wed, 05 Oct 2022 00:19:21 GMT  
		Size: 52.7 MB (52669988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6422d53934b53541883e4d8479c0384974a4f8c2ca335b2e86b900b4cf761d7d`  
		Last Modified: Wed, 05 Oct 2022 01:35:18 GMT  
		Size: 8.7 MB (8665467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2fd86c88bcf963ae10ae57261059a1b2bdbad2590061f63513acf0308dacf1`  
		Last Modified: Wed, 05 Oct 2022 01:35:18 GMT  
		Size: 11.1 MB (11130537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408a6f9d0ef9c4902e1584d5a5ac4ed8e9e71594c69a06143ca94a9b42bfc026`  
		Last Modified: Wed, 05 Oct 2022 01:36:07 GMT  
		Size: 56.9 MB (56887661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7896915ee9ec5c0e37b59cfbe6d7cb364dff641bd4c04f0160f59fab6e46f072`  
		Last Modified: Wed, 05 Oct 2022 01:38:22 GMT  
		Size: 197.6 MB (197567269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:4a3598d62e23e3003db6e423ae264e43db2ff5657ec189e6f6d00f5c69e85a4b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.0 MB (352964297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:992be19844bb6ce728b69d6af195e74bad155d8b12433dacfa7ba1c518fffaa8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:14:07 GMT
ADD file:6e9efd6bb77c835520332c88cb412f38f0d8573ec3347b090b77965e17131780 in / 
# Tue, 25 Oct 2022 03:14:10 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:17:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:17:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:17:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:19:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a3962f6ac5b86fa159789ea1e9241ecbb956b3223e8312f7d92d7fbb8bf5485`  
		Last Modified: Tue, 25 Oct 2022 03:20:03 GMT  
		Size: 54.7 MB (54704717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c5225e6c97e35e08afc065bed0fb4156a1727da9a3e12b4a611189682c919a`  
		Last Modified: Tue, 25 Oct 2022 06:50:49 GMT  
		Size: 9.7 MB (9684744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39fe7c3b495d9320ca99478bfddf7a3fa0412a37c56ca95a4cc891ceb738e62`  
		Last Modified: Tue, 25 Oct 2022 06:50:49 GMT  
		Size: 11.9 MB (11937807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9270b45cd7087efea37438ff9651d0078e51c8b476b199cfc26770079313e3`  
		Last Modified: Tue, 25 Oct 2022 06:51:17 GMT  
		Size: 62.7 MB (62679073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652adf8e207d919d0f1ddc84ad9fa208e1ec7d27d5573d5c3348e681a13f65b5`  
		Last Modified: Tue, 25 Oct 2022 06:52:18 GMT  
		Size: 214.0 MB (213957956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:3a887968fe43226ca614e3bdfba591197b3593e08bde65a9a38a179bf5715812
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.9 MB (359929860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0617997a465ac3f99d967a05d654c18e959edee32e325b2b1dc07db26768495`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:39:40 GMT
ADD file:cff1e1a432929527e9bb64bde53e2b614c941bd4631b7bd3634fdda8a7240455 in / 
# Wed, 05 Oct 2022 00:39:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:26:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:27:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 02:31:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:40:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9cc6da93595cf4d9d589de999765cc4f1efa5e0d8e23ca6dd8b73b18afdc8189`  
		Last Modified: Wed, 05 Oct 2022 00:57:59 GMT  
		Size: 48.9 MB (48857821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554ce58712f86101a4716baede25ee43c9c1fc550b39fb4b3e5fa1622fd3b00b`  
		Last Modified: Wed, 05 Oct 2022 03:30:22 GMT  
		Size: 8.4 MB (8388012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd132871253f925889ef836099addcf830644843a64a1529bddc510390846a9b`  
		Last Modified: Wed, 05 Oct 2022 03:30:22 GMT  
		Size: 10.8 MB (10750715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bfc76b3f6f1ba447e697e6e2190cf70e757458cce81446b79426ae4cccdb03`  
		Last Modified: Wed, 05 Oct 2022 03:33:00 GMT  
		Size: 54.0 MB (54018661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58e7099a4ad88bc20a780df4c500b9445dc2cb39e8ac84d70a11e8903e5b6448`  
		Last Modified: Wed, 05 Oct 2022 03:40:39 GMT  
		Size: 237.9 MB (237914651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:f3a95238e9fb25bdb30cf9bac9a31017e573719ecc1390cb196795031f399a69
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.9 MB (308907690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b76b4efc93df24f2f1e78a196a448ee70d9bf65a4f671e9a7d61ee0a29bad85`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:14:54 GMT
ADD file:7dba2ae439c9f5da3fe962e867cee94eafc0b12a74939e13fdf987965ef8191c in / 
# Tue, 25 Oct 2022 01:14:57 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:32:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:32:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 02:33:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:33:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1430653806baea9ab2928a0d226c10ba8e7bf4b9b93398f9082ba16edfb2d4b8`  
		Last Modified: Tue, 25 Oct 2022 01:19:17 GMT  
		Size: 49.0 MB (49012977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa67452e329e71787509a1583923b8e1e83b22a2fb76e48111393a03205d4c20`  
		Last Modified: Tue, 25 Oct 2022 02:50:30 GMT  
		Size: 8.7 MB (8738304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7be163526b121ed701b3595b33b6d8755aba04a12b0fd801f9c899cbd3ebd0`  
		Last Modified: Tue, 25 Oct 2022 02:50:30 GMT  
		Size: 11.0 MB (11041665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ea6534b4c7c78beb071314cf02af39dc48f27dffa56b6182c538fc47d868d4`  
		Last Modified: Tue, 25 Oct 2022 02:50:45 GMT  
		Size: 56.9 MB (56939890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e73095f949aa471b5db609eab93348cee45f8092aba617f080c27c32b8c06c`  
		Last Modified: Tue, 25 Oct 2022 02:51:14 GMT  
		Size: 183.2 MB (183174854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:d73594bc7e05039d42fa3ad9c5b2daabadc46b38fafe9e9e545616f582643259
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
$ docker pull buildpack-deps@sha256:cc22c156446c9313c4680623e26c6e48bba2f98ec6ce87c8ed3a0d52e716c0a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.4 MB (73367169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87b8c38f75980c2def43a2d61e770ccc0b3c9955ae57c722bb79d7f977a21e31`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:27:32 GMT
ADD file:b2f29ff1f75077ccce680becaa7bffdc9dfb9c7938188e93673e1b42bf418630 in / 
# Tue, 04 Oct 2022 23:27:32 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:58:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:59:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a9fedee3000f9dcc2b77410cd53420ec321135a3f7a6c688b43f31e503042e1e`  
		Last Modified: Tue, 04 Oct 2022 23:32:34 GMT  
		Size: 52.7 MB (52684279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dda17d2d1d2961ba6c7083d3013dde5fb5af68bd80ee1e40adbf7886b64df3c`  
		Last Modified: Wed, 05 Oct 2022 01:21:27 GMT  
		Size: 9.3 MB (9300772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809d617f2e2db52d55fec066a28a409d69e1dc40dd9f91f7f03c19ec8d16c587`  
		Last Modified: Wed, 05 Oct 2022 01:21:27 GMT  
		Size: 11.4 MB (11382118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:003e17008ddaf3d07c54f0e22bf1740953332445e88af588740603583bd313ef
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (68957196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:735e2d1a8b82054ce8ae48afcdbd6e7bd00b34f6107e66adc81d2023c1a0c787`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:06:50 GMT
ADD file:829f8e96e527611e85aa710b19c01c75a4760a27c651fb439f8cdb5609db64aa in / 
# Tue, 25 Oct 2022 03:06:52 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:14:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:14:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:513ea4862e78a8cc07ed6d320f10e746ca770eb039dec1548c31a9de19d1f7ce`  
		Last Modified: Tue, 25 Oct 2022 03:12:19 GMT  
		Size: 49.6 MB (49578888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1ace4b71d48c3105e8f55674a41898f6b1df73d7ee8b05d5c3d3b3fea66077`  
		Last Modified: Tue, 25 Oct 2022 06:20:29 GMT  
		Size: 8.5 MB (8548544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:428ee02803cd3666baa3051b15b273e86d1d20710ddd79191fb1367a0dda5edc`  
		Last Modified: Tue, 25 Oct 2022 06:20:29 GMT  
		Size: 10.8 MB (10829764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:67e81d32e4a379ebc001840f12d827e5f67833629cc8d825dc7e62681fdec972
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68499979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ead5cdfb9f5e5c275759c55be9d11eb1dc155f3aa55dad5b5be0cb66efd70376`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:00:01 GMT
ADD file:41046e966f37a45410c2aa02920b78f877f5aacb6ee087b2c6c6642f4e7b474f in / 
# Wed, 05 Oct 2022 00:00:02 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:38:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:38:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1316bf5b10f256f27feadcb25edef6365e912773e60cc382610ef003daf37248`  
		Last Modified: Wed, 05 Oct 2022 00:07:10 GMT  
		Size: 49.4 MB (49436823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00270159c4caaec159e25e1eaca6209b11c838dd60b5e0f5194e2279c51cd70`  
		Last Modified: Wed, 05 Oct 2022 00:56:26 GMT  
		Size: 8.4 MB (8399366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8524fd9b0e923155334b98a655b41aa941eb210e3248b7cc375ee49257b2b929`  
		Last Modified: Wed, 05 Oct 2022 00:56:26 GMT  
		Size: 10.7 MB (10663790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a0fa7918450dd9fe388abd5681d138ceac42806881b9f01ab9773a5a6cfce977
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.7 MB (70715689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d50f6af0113bc54f7f717b62c4be946ce8984d31d0e202389ef84720e47a647`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:29 GMT
ADD file:6a2d69a5a731490271c915d99634a89755f7236ef56712924ea061730d8552c4 in / 
# Tue, 25 Oct 2022 05:46:30 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:01:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:01:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:63a396bb133ce57141398b6c6d776ce17e3e973085b5a1b746d76407240a376a`  
		Last Modified: Tue, 25 Oct 2022 05:50:38 GMT  
		Size: 50.6 MB (50643735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a89cf1bf3c8da06b08672e8551d2511df312e843fb3acab24e31d9ba0afa866`  
		Last Modified: Tue, 25 Oct 2022 08:32:19 GMT  
		Size: 8.9 MB (8932959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e653e6dd7e514d68792b5ac0d2812dbc50a0e1d5c4842fd356c767031c54aec`  
		Last Modified: Tue, 25 Oct 2022 08:32:19 GMT  
		Size: 11.1 MB (11138995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:7a92edc5d0d1d9b005fc402881b8f8eddac8e13c8f5adf57fb62e1a26d00983d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.3 MB (72287451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b1893a81cbf84a850be47ff4f28e1dd4035b9c2256bdedf86584fb4079c771d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:23:38 GMT
ADD file:80dabb60a37b1d88f3750adb85c9e159d00b55293f70ad93512f94bd3cfd99bc in / 
# Tue, 25 Oct 2022 02:23:39 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:18:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:18:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:367799113badd94b9683087d6086436649a1fb7127698c42b0d730f5bbedcf86`  
		Last Modified: Tue, 25 Oct 2022 02:30:22 GMT  
		Size: 51.6 MB (51625321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564d2fccc59969c0b37e3bb8384bc6545a4cce125daa11c7e8b599ec0acac788`  
		Last Modified: Tue, 25 Oct 2022 05:30:00 GMT  
		Size: 9.3 MB (9282393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09be9213196e288bdcccf553107591d6fe4f04fccea4da55faea35dd79cfff15`  
		Last Modified: Tue, 25 Oct 2022 05:30:00 GMT  
		Size: 11.4 MB (11379737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:177c731ad458bb98287f9b7f0ff300408fc1a53c32e1d406bb638c4c00719d21
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72465992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50d48d0070c45b656746927bfe7b8ec4a82c7b00acdd9cce150d2c20e17feb87`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:11:00 GMT
ADD file:a7d6f7226093388fbc662c6e3fa1bc8dc263ab630fe03ea088486e6b016474ff in / 
# Wed, 05 Oct 2022 00:11:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:20:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:21:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3110bff10f823ecdaa06d8f7c65ce83d7c99521680207da9d264aaa8823d5209`  
		Last Modified: Wed, 05 Oct 2022 00:19:21 GMT  
		Size: 52.7 MB (52669988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6422d53934b53541883e4d8479c0384974a4f8c2ca335b2e86b900b4cf761d7d`  
		Last Modified: Wed, 05 Oct 2022 01:35:18 GMT  
		Size: 8.7 MB (8665467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2fd86c88bcf963ae10ae57261059a1b2bdbad2590061f63513acf0308dacf1`  
		Last Modified: Wed, 05 Oct 2022 01:35:18 GMT  
		Size: 11.1 MB (11130537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:124e076bd786711b687044fd136c24af7bc4500c1e67e6e1f0f4086eedfced08
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.3 MB (76327268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce644126cccec0395c556b7c4763b65ccbe0344029fc1fc5a5a1c93e9d1c4787`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:14:07 GMT
ADD file:6e9efd6bb77c835520332c88cb412f38f0d8573ec3347b090b77965e17131780 in / 
# Tue, 25 Oct 2022 03:14:10 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:17:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:17:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:7a3962f6ac5b86fa159789ea1e9241ecbb956b3223e8312f7d92d7fbb8bf5485`  
		Last Modified: Tue, 25 Oct 2022 03:20:03 GMT  
		Size: 54.7 MB (54704717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c5225e6c97e35e08afc065bed0fb4156a1727da9a3e12b4a611189682c919a`  
		Last Modified: Tue, 25 Oct 2022 06:50:49 GMT  
		Size: 9.7 MB (9684744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39fe7c3b495d9320ca99478bfddf7a3fa0412a37c56ca95a4cc891ceb738e62`  
		Last Modified: Tue, 25 Oct 2022 06:50:49 GMT  
		Size: 11.9 MB (11937807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:91c41397454a62656ddc234f54c6ce9bc6eebb7463198b379aec9760ef9f5ce3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.0 MB (67996548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c82f669a88d6376397cb790855001ce2a2328184d9fc8f1fbf316b588cd40e4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:39:40 GMT
ADD file:cff1e1a432929527e9bb64bde53e2b614c941bd4631b7bd3634fdda8a7240455 in / 
# Wed, 05 Oct 2022 00:39:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:26:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:27:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9cc6da93595cf4d9d589de999765cc4f1efa5e0d8e23ca6dd8b73b18afdc8189`  
		Last Modified: Wed, 05 Oct 2022 00:57:59 GMT  
		Size: 48.9 MB (48857821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554ce58712f86101a4716baede25ee43c9c1fc550b39fb4b3e5fa1622fd3b00b`  
		Last Modified: Wed, 05 Oct 2022 03:30:22 GMT  
		Size: 8.4 MB (8388012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd132871253f925889ef836099addcf830644843a64a1529bddc510390846a9b`  
		Last Modified: Wed, 05 Oct 2022 03:30:22 GMT  
		Size: 10.8 MB (10750715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:459e259ac9d973e273d44f4977a901a7c57dce7f749c5caf0ade7837350bf940
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68792946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8919e63d46a3758bb8046627e26a7d852ed8e26e8b044f56948b519863d33fd4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:14:54 GMT
ADD file:7dba2ae439c9f5da3fe962e867cee94eafc0b12a74939e13fdf987965ef8191c in / 
# Tue, 25 Oct 2022 01:14:57 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:32:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:32:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1430653806baea9ab2928a0d226c10ba8e7bf4b9b93398f9082ba16edfb2d4b8`  
		Last Modified: Tue, 25 Oct 2022 01:19:17 GMT  
		Size: 49.0 MB (49012977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa67452e329e71787509a1583923b8e1e83b22a2fb76e48111393a03205d4c20`  
		Last Modified: Tue, 25 Oct 2022 02:50:30 GMT  
		Size: 8.7 MB (8738304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7be163526b121ed701b3595b33b6d8755aba04a12b0fd801f9c899cbd3ebd0`  
		Last Modified: Tue, 25 Oct 2022 02:50:30 GMT  
		Size: 11.0 MB (11041665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:sid-scm`

```console
$ docker pull buildpack-deps@sha256:b50c4e396c237f001ad110bae4dc336d4385072144bbcc70545e1aac7afc164e
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
$ docker pull buildpack-deps@sha256:25c732971a707c1aa513e89ebe69d3167742941a1926860949186f4665a61e90
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131420075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f4ee86a7ab5c87f3ca76cf99bb43f859974dcabaee4095c54ee36e61f14f963`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:27:32 GMT
ADD file:b2f29ff1f75077ccce680becaa7bffdc9dfb9c7938188e93673e1b42bf418630 in / 
# Tue, 04 Oct 2022 23:27:32 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:58:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:59:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:59:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a9fedee3000f9dcc2b77410cd53420ec321135a3f7a6c688b43f31e503042e1e`  
		Last Modified: Tue, 04 Oct 2022 23:32:34 GMT  
		Size: 52.7 MB (52684279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dda17d2d1d2961ba6c7083d3013dde5fb5af68bd80ee1e40adbf7886b64df3c`  
		Last Modified: Wed, 05 Oct 2022 01:21:27 GMT  
		Size: 9.3 MB (9300772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809d617f2e2db52d55fec066a28a409d69e1dc40dd9f91f7f03c19ec8d16c587`  
		Last Modified: Wed, 05 Oct 2022 01:21:27 GMT  
		Size: 11.4 MB (11382118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15dd69568329cc8f49552e84cc7a6c0a0c112efb493830d52d7c1c6ed88af8f`  
		Last Modified: Wed, 05 Oct 2022 01:21:45 GMT  
		Size: 58.1 MB (58052906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:a8b12521cd98493a261a1f55e4e49770685b571e6386be3381e830a332b0fb77
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.5 MB (124504941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71f6828f20558d795c5704b92e9a7aa0d14089cfce9c332cbeddd096e880fb9e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:06:50 GMT
ADD file:829f8e96e527611e85aa710b19c01c75a4760a27c651fb439f8cdb5609db64aa in / 
# Tue, 25 Oct 2022 03:06:52 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:14:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:14:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:15:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:513ea4862e78a8cc07ed6d320f10e746ca770eb039dec1548c31a9de19d1f7ce`  
		Last Modified: Tue, 25 Oct 2022 03:12:19 GMT  
		Size: 49.6 MB (49578888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1ace4b71d48c3105e8f55674a41898f6b1df73d7ee8b05d5c3d3b3fea66077`  
		Last Modified: Tue, 25 Oct 2022 06:20:29 GMT  
		Size: 8.5 MB (8548544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:428ee02803cd3666baa3051b15b273e86d1d20710ddd79191fb1367a0dda5edc`  
		Last Modified: Tue, 25 Oct 2022 06:20:29 GMT  
		Size: 10.8 MB (10829764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecfb58f8aebfa286f964add0eb9b5f5bf243c4e6b5c934809df2c000acf0301c`  
		Last Modified: Tue, 25 Oct 2022 06:20:53 GMT  
		Size: 55.5 MB (55547745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:40c9e410a265ce99ab8112cf900f9fa0daef54cf9234ad867c88266563924307
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122227727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d951a42d8333c4774860fbaa9e0b184cb41f258db3b954eb1f6cbfae9610cf4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:00:01 GMT
ADD file:41046e966f37a45410c2aa02920b78f877f5aacb6ee087b2c6c6642f4e7b474f in / 
# Wed, 05 Oct 2022 00:00:02 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:38:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:38:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:38:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1316bf5b10f256f27feadcb25edef6365e912773e60cc382610ef003daf37248`  
		Last Modified: Wed, 05 Oct 2022 00:07:10 GMT  
		Size: 49.4 MB (49436823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00270159c4caaec159e25e1eaca6209b11c838dd60b5e0f5194e2279c51cd70`  
		Last Modified: Wed, 05 Oct 2022 00:56:26 GMT  
		Size: 8.4 MB (8399366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8524fd9b0e923155334b98a655b41aa941eb210e3248b7cc375ee49257b2b929`  
		Last Modified: Wed, 05 Oct 2022 00:56:26 GMT  
		Size: 10.7 MB (10663790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92867f6312a37ef5d4d5b38b1944bbe65123c5127a3ace08db615300dfc442c7`  
		Last Modified: Wed, 05 Oct 2022 00:56:52 GMT  
		Size: 53.7 MB (53727748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:009fc52c030c01267bd65a2028550fb986ff9a24369ae3d7ef56602a860c7962
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128431668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:401058bc5bd559766e08995d18ca3833502c6c103700576f37a012f933754edf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:29 GMT
ADD file:6a2d69a5a731490271c915d99634a89755f7236ef56712924ea061730d8552c4 in / 
# Tue, 25 Oct 2022 05:46:30 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:01:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:01:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:02:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:63a396bb133ce57141398b6c6d776ce17e3e973085b5a1b746d76407240a376a`  
		Last Modified: Tue, 25 Oct 2022 05:50:38 GMT  
		Size: 50.6 MB (50643735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a89cf1bf3c8da06b08672e8551d2511df312e843fb3acab24e31d9ba0afa866`  
		Last Modified: Tue, 25 Oct 2022 08:32:19 GMT  
		Size: 8.9 MB (8932959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e653e6dd7e514d68792b5ac0d2812dbc50a0e1d5c4842fd356c767031c54aec`  
		Last Modified: Tue, 25 Oct 2022 08:32:19 GMT  
		Size: 11.1 MB (11138995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c34d6a76d061ba3fc92256f8a3d68cb9c3d5840430072a886deb01b71229ceba`  
		Last Modified: Tue, 25 Oct 2022 08:32:40 GMT  
		Size: 57.7 MB (57715979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:727397e319709783655de941e122470c8e5580ec96e62fbc532fce0166e10ea4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131761295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbf8113ad39378aabee953d3468724d3c1eb3ab375b04cb1942f60a917ec3e0f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:23:38 GMT
ADD file:80dabb60a37b1d88f3750adb85c9e159d00b55293f70ad93512f94bd3cfd99bc in / 
# Tue, 25 Oct 2022 02:23:39 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:18:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:18:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 05:19:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:367799113badd94b9683087d6086436649a1fb7127698c42b0d730f5bbedcf86`  
		Last Modified: Tue, 25 Oct 2022 02:30:22 GMT  
		Size: 51.6 MB (51625321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564d2fccc59969c0b37e3bb8384bc6545a4cce125daa11c7e8b599ec0acac788`  
		Last Modified: Tue, 25 Oct 2022 05:30:00 GMT  
		Size: 9.3 MB (9282393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09be9213196e288bdcccf553107591d6fe4f04fccea4da55faea35dd79cfff15`  
		Last Modified: Tue, 25 Oct 2022 05:30:00 GMT  
		Size: 11.4 MB (11379737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7cf8ff2ca1128a94c435416195c01bd46e7b32191a4a225527692f374d4e31e`  
		Last Modified: Tue, 25 Oct 2022 05:30:21 GMT  
		Size: 59.5 MB (59473844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:c9c05846a233f3706bbd7659030113b2c11cb85bcbc85f0b7b52ceb249609d45
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.4 MB (129353653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33fe28a49a8569202e6d59224f55c96afa8a526b2d020c759bf8a9e89b40f50f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:11:00 GMT
ADD file:a7d6f7226093388fbc662c6e3fa1bc8dc263ab630fe03ea088486e6b016474ff in / 
# Wed, 05 Oct 2022 00:11:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:20:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:21:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:22:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3110bff10f823ecdaa06d8f7c65ce83d7c99521680207da9d264aaa8823d5209`  
		Last Modified: Wed, 05 Oct 2022 00:19:21 GMT  
		Size: 52.7 MB (52669988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6422d53934b53541883e4d8479c0384974a4f8c2ca335b2e86b900b4cf761d7d`  
		Last Modified: Wed, 05 Oct 2022 01:35:18 GMT  
		Size: 8.7 MB (8665467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2fd86c88bcf963ae10ae57261059a1b2bdbad2590061f63513acf0308dacf1`  
		Last Modified: Wed, 05 Oct 2022 01:35:18 GMT  
		Size: 11.1 MB (11130537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408a6f9d0ef9c4902e1584d5a5ac4ed8e9e71594c69a06143ca94a9b42bfc026`  
		Last Modified: Wed, 05 Oct 2022 01:36:07 GMT  
		Size: 56.9 MB (56887661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:b752fc221f409b6cdab8b2847838e201ce3d7c95856590870fa67391d109b85c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.0 MB (139006341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6da31aa88a012fc286c9e83bfe13f29518d53fa4afd44a2356ddc53ddc827f65`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:14:07 GMT
ADD file:6e9efd6bb77c835520332c88cb412f38f0d8573ec3347b090b77965e17131780 in / 
# Tue, 25 Oct 2022 03:14:10 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:17:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:17:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:17:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a3962f6ac5b86fa159789ea1e9241ecbb956b3223e8312f7d92d7fbb8bf5485`  
		Last Modified: Tue, 25 Oct 2022 03:20:03 GMT  
		Size: 54.7 MB (54704717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c5225e6c97e35e08afc065bed0fb4156a1727da9a3e12b4a611189682c919a`  
		Last Modified: Tue, 25 Oct 2022 06:50:49 GMT  
		Size: 9.7 MB (9684744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39fe7c3b495d9320ca99478bfddf7a3fa0412a37c56ca95a4cc891ceb738e62`  
		Last Modified: Tue, 25 Oct 2022 06:50:49 GMT  
		Size: 11.9 MB (11937807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9270b45cd7087efea37438ff9651d0078e51c8b476b199cfc26770079313e3`  
		Last Modified: Tue, 25 Oct 2022 06:51:17 GMT  
		Size: 62.7 MB (62679073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:80fe5d929462fbcb8fb502564ba1c94f3a1fb305aff0e201341b695be50f3fd5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.0 MB (122015209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3095c5914c0792da561d083de7026417fc5bec6e01a866d86b2f8f8d796eac27`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:39:40 GMT
ADD file:cff1e1a432929527e9bb64bde53e2b614c941bd4631b7bd3634fdda8a7240455 in / 
# Wed, 05 Oct 2022 00:39:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:26:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:27:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 02:31:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9cc6da93595cf4d9d589de999765cc4f1efa5e0d8e23ca6dd8b73b18afdc8189`  
		Last Modified: Wed, 05 Oct 2022 00:57:59 GMT  
		Size: 48.9 MB (48857821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554ce58712f86101a4716baede25ee43c9c1fc550b39fb4b3e5fa1622fd3b00b`  
		Last Modified: Wed, 05 Oct 2022 03:30:22 GMT  
		Size: 8.4 MB (8388012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd132871253f925889ef836099addcf830644843a64a1529bddc510390846a9b`  
		Last Modified: Wed, 05 Oct 2022 03:30:22 GMT  
		Size: 10.8 MB (10750715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bfc76b3f6f1ba447e697e6e2190cf70e757458cce81446b79426ae4cccdb03`  
		Last Modified: Wed, 05 Oct 2022 03:33:00 GMT  
		Size: 54.0 MB (54018661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:4030ace049550e7266628c08a838e0658e705dad4f0491dac2535698df26107b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125732836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78d8337e348ae8954f28173bf3c8248b38c98bf8c64e684b15d1dc50a21089c7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:14:54 GMT
ADD file:7dba2ae439c9f5da3fe962e867cee94eafc0b12a74939e13fdf987965ef8191c in / 
# Tue, 25 Oct 2022 01:14:57 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:32:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:32:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 02:33:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1430653806baea9ab2928a0d226c10ba8e7bf4b9b93398f9082ba16edfb2d4b8`  
		Last Modified: Tue, 25 Oct 2022 01:19:17 GMT  
		Size: 49.0 MB (49012977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa67452e329e71787509a1583923b8e1e83b22a2fb76e48111393a03205d4c20`  
		Last Modified: Tue, 25 Oct 2022 02:50:30 GMT  
		Size: 8.7 MB (8738304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7be163526b121ed701b3595b33b6d8755aba04a12b0fd801f9c899cbd3ebd0`  
		Last Modified: Tue, 25 Oct 2022 02:50:30 GMT  
		Size: 11.0 MB (11041665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ea6534b4c7c78beb071314cf02af39dc48f27dffa56b6182c538fc47d868d4`  
		Last Modified: Tue, 25 Oct 2022 02:50:45 GMT  
		Size: 56.9 MB (56939890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stable`

```console
$ docker pull buildpack-deps@sha256:4c611d88a39769ef8b4a77505f9377f74df78ae41bf9f81be47522d13549ba1b
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
$ docker pull buildpack-deps@sha256:da6442775441c5a43c9cdcbc18c633c9a94196521736ea0c04d3bc4ab6d24007
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.5 MB (322518570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c35b468f323a45e3ac977f6960f5657ec31473c3a183f96f5ff908fdfa3f9b8d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:27 GMT
ADD file:d1268789456d2cdace6e50149e60404ad5a849b7c61e8fc8bc7b6e0eb6eeb7ca in / 
# Tue, 04 Oct 2022 23:26:27 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:54:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:55:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:55:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:56:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f606d8928ed378229f2460b94b504cca239fb906efc57acbdf9340bd298d5ddf`  
		Last Modified: Tue, 04 Oct 2022 23:30:27 GMT  
		Size: 55.0 MB (55046248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47db815c6a4547dc224b75222193cb1851cf529d2cbdf26f854b9bbf97099b98`  
		Last Modified: Wed, 05 Oct 2022 01:19:13 GMT  
		Size: 5.2 MB (5163279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf48494000001a037b72870d2a6a2536f9da8bc5d1ceddd72d79f4a51fe7a60e`  
		Last Modified: Wed, 05 Oct 2022 01:19:13 GMT  
		Size: 10.9 MB (10876505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a572f7a256d36a93ab0777949771b120c5d7dce75ea2a2d3d9444793b26b2ef1`  
		Last Modified: Wed, 05 Oct 2022 01:19:34 GMT  
		Size: 54.6 MB (54584293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f7d0525895528fdb73153451e112bbd8e1854549bd1e0e6f4ac0b4a2ee98172`  
		Last Modified: Wed, 05 Oct 2022 01:20:11 GMT  
		Size: 196.8 MB (196848245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:e95f5a44cff65278e6f2df29eef9d7957e19ab74e610841ca613250500cfb07c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.6 MB (295556261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5fc1f9478434ff5825094db6336cb96abec3dff210ea3918afc05508b3b8389`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:06:19 GMT
ADD file:b314b98654e8532fd10a08a172ea5c3edb7d7a36c7faf85d06d14be12f7b83ef in / 
# Tue, 25 Oct 2022 03:06:19 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:12:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:12:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:12:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:14:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1f0ecb08923b99bef3f82c2e88603bb53e3ed084c13252275c05039cc279c158`  
		Last Modified: Tue, 25 Oct 2022 03:11:15 GMT  
		Size: 52.5 MB (52547473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b399c5eb53b4c35fa33682a82d73bdc4b096cd78ae95fe36c4ed81d18f6849`  
		Last Modified: Tue, 25 Oct 2022 06:19:02 GMT  
		Size: 5.1 MB (5072235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ccdd06393cd3873a3cc8b9cbe170a2032fd61d1d545b7045b649faf2f4e732`  
		Last Modified: Tue, 25 Oct 2022 06:19:02 GMT  
		Size: 10.6 MB (10574279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aafe0e287af4e488dcda51195e4eb1ae1386e3265989c457172f32f6357bf26`  
		Last Modified: Tue, 25 Oct 2022 06:19:28 GMT  
		Size: 52.3 MB (52322157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22771ccea19352dbb0e5ba44c17b8ef14425ff0a22c744bca41cdbde02bdfd9f`  
		Last Modified: Tue, 25 Oct 2022 06:20:12 GMT  
		Size: 175.0 MB (175040117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:4ef648e774c537efc33738cca9dfbc87771bbbaab19e36fffdc55e0f440c699a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.0 MB (283005348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe5e78b4d0fb86176858f424786c09b823ee34558e44538321f40a14100f6a57`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:28 GMT
ADD file:47a3f2948af18c39686ca59a88a439c25edaf286064d3a2ccc5dab47fee2fc52 in / 
# Tue, 04 Oct 2022 23:58:29 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:32:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:32:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:32:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:34:32 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e19342fb46cabf6147aec1d1c6af1f3a82736530cf3b067835fc8a09da092ce3`  
		Last Modified: Wed, 05 Oct 2022 00:04:36 GMT  
		Size: 50.2 MB (50209087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a49f93f990f17337480b5bdf526a6bb48d1ae63bd17f54be17cd2f6ebba4de7d`  
		Last Modified: Wed, 05 Oct 2022 00:53:28 GMT  
		Size: 4.9 MB (4931366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3989be0d7ed2f72fae0310039043f6ba76c24a45f9ec9689697ebd932845cc8`  
		Last Modified: Wed, 05 Oct 2022 00:53:28 GMT  
		Size: 10.2 MB (10217872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6487a2e4236617393a6184f0f89a360d295ab118da2ea4ad48fa8645ae211755`  
		Last Modified: Wed, 05 Oct 2022 00:53:57 GMT  
		Size: 50.3 MB (50343324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cb778b20f33d18ee7b4046bfd5685ddf5bb8750a2f3826f14408897c4d9db5`  
		Last Modified: Wed, 05 Oct 2022 00:54:45 GMT  
		Size: 167.3 MB (167303699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:bba56093d706c0b145e14ee726d81f59b1d09e069d3b84c30e9bee0af5a24687
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.2 MB (314172338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c2f1635631cecb5159531c9282693f4a86c19d02ec9f92e0f40baa073e51f5b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:45:55 GMT
ADD file:b16745ece8ef84c028d7e9ac4bf026ac64f885d4170bfcc9d435f237144a1b99 in / 
# Tue, 25 Oct 2022 05:45:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:58:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:58:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 07:59:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:00:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8e1d92e7d04d2a9a9880cb45dc3c32c2805912cd86abed96d0ada3ff28748205`  
		Last Modified: Tue, 25 Oct 2022 05:48:40 GMT  
		Size: 53.7 MB (53701966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66eadbf427bb41b3e329a95935c65b09c6d3b7a9c2fa8e08417e497df02ed996`  
		Last Modified: Tue, 25 Oct 2022 08:30:22 GMT  
		Size: 5.2 MB (5151506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9731f4e3bc3680179c10cece663cf0cfe0488918d6795406f4b76f07b787de`  
		Last Modified: Tue, 25 Oct 2022 08:30:22 GMT  
		Size: 10.9 MB (10874174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d337cb12fd7c6fe341850cd38e880f1806d49a65832c9804b06d00f9032382e0`  
		Last Modified: Tue, 25 Oct 2022 08:30:42 GMT  
		Size: 54.7 MB (54683990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a719597fe1ca78e1dc4c43fffc424754228514a791abcb0e0c06302ad022b8ca`  
		Last Modified: Tue, 25 Oct 2022 08:31:12 GMT  
		Size: 189.8 MB (189760702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:730efefe6d075835e0fede96affe8d8631d8212509b4c7003c32b47bf3c550b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.8 MB (327836520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d42762c45517dca640707932c4cfb4d4903431b010d2feb9a29f09b820a3ed5b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:22:19 GMT
ADD file:aa26f69b37c3e144d08e17bb9be7302ec89ae0579121c874a35f336d7077fd3b in / 
# Tue, 25 Oct 2022 02:22:19 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:15:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:15:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 05:15:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:16:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8caf426a2703f99fb0be4b03411ecaa580d102f7c47ef43b422b6d7c13c380e2`  
		Last Modified: Tue, 25 Oct 2022 02:27:54 GMT  
		Size: 56.0 MB (56023960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b92a2ff5c72653a0679aa7f5e2bc695011c0a71faa424229e560957d204dab`  
		Last Modified: Tue, 25 Oct 2022 05:27:37 GMT  
		Size: 5.1 MB (5086887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6856a3002e686ceb6d48d078731366f576ed3adcb73bd49dcb300057732904`  
		Last Modified: Tue, 25 Oct 2022 05:27:38 GMT  
		Size: 11.0 MB (11032526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e88080d3b5ba1edc8623a97d068bd040dfb89f2bc7bdfc0984d11fc35ff5885`  
		Last Modified: Tue, 25 Oct 2022 05:28:00 GMT  
		Size: 55.9 MB (55924404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b19879261038142328725a860507e23c40804ec5e04f1b7cf8f0dc88ded89d`  
		Last Modified: Tue, 25 Oct 2022 05:28:37 GMT  
		Size: 199.8 MB (199768743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:6088b9f6bed37906eecc152f8a3f642c5688b69f3c6c1ec283bd420ea0168585
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.1 MB (301112687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2991accb9ec37e952acae5a8759ce6006e7e1e39739799c51bab7c987e0d7867`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:09:48 GMT
ADD file:ca40db2df3dbc600910b8cd139c564cf5b8bd6c1a06cc517cae2c1c05cff6dde in / 
# Wed, 05 Oct 2022 00:09:51 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:11:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:12:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:14:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:19:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:25bcd35faf05f859c3077f0e2e7010d24e56cdcfb77efbdeda236e47dc08e14a`  
		Last Modified: Wed, 05 Oct 2022 00:17:52 GMT  
		Size: 53.3 MB (53265834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c44f381e4f9f5eb923a09cbd49bc86d3d36121137c1e063d30d73af518bf0f86`  
		Last Modified: Wed, 05 Oct 2022 01:32:02 GMT  
		Size: 4.9 MB (4918634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59260097f47eb21e87461a2a98c76f46372dd316b878bbd3d4d9c51cc28a62b7`  
		Last Modified: Wed, 05 Oct 2022 01:32:04 GMT  
		Size: 10.7 MB (10661237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f8a68e1316af16785650ca91231ed6373810fcdaff8fb5bec9f58e1ccc2a32`  
		Last Modified: Wed, 05 Oct 2022 01:32:53 GMT  
		Size: 53.3 MB (53304716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbf1a80df4f8f31f1ab3653fe8e3b40cb5a88a81ea4bc64c95e1b388fe7e2cc`  
		Last Modified: Wed, 05 Oct 2022 01:34:59 GMT  
		Size: 179.0 MB (178962266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:39252f001a267e36e8cc4cbd5a51b22eb6f6b8c862a0eebae0f84c115268f828
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.0 MB (331028350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fe0aa4188607937a62728cb0c6bb7d668f569b3384fecff44935b02408e9068`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:13:28 GMT
ADD file:c01a6cc4222fbeeda5c2d679c5b355539880a02c792c64861eb17b81a3678f45 in / 
# Tue, 25 Oct 2022 03:13:31 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:13:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:14:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:14:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:16:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ee5a342763ed1d31bef8cebe9f4cc5dd6d427f630da679a87da0427be7b22e3d`  
		Last Modified: Tue, 25 Oct 2022 03:18:52 GMT  
		Size: 58.9 MB (58916374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a4727f39cbcb19b39abdbd847eeceed842ef65f8514372024c48b913bc951a`  
		Last Modified: Tue, 25 Oct 2022 06:49:00 GMT  
		Size: 5.4 MB (5414507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe601e6c8a1ec9c69c49c65a53339202a65cea9d4f01d161fb34905c06a4a99`  
		Last Modified: Tue, 25 Oct 2022 06:49:01 GMT  
		Size: 11.6 MB (11630153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5055e27b58426c2b637b1c8c179e6abe306e3dfb55a9c170c73fb0d581c6cf3e`  
		Last Modified: Tue, 25 Oct 2022 06:49:31 GMT  
		Size: 58.9 MB (58867355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a503b0a90ce32a745c9586bc6c28360d8de222565d7105d079b530524e1e38`  
		Last Modified: Tue, 25 Oct 2022 06:50:32 GMT  
		Size: 196.2 MB (196199961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:56a7b6a421aea89e44c16d6526e1f2688c8b129fae975687ccdef4707e507432
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.1 MB (296088034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:172dabba1a37b7c132ad4884aca1fd3c1b63d62e29533b09589ac174b5c3f0f7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:14:24 GMT
ADD file:06f15d8a3c04752d271a052e820fb13fcdb76f0d18f6c9afb6e70391d10348ec in / 
# Tue, 25 Oct 2022 01:14:27 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:31:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:31:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 02:31:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:32:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a556186e8bea4ba9925d0c17bea2c12bfbb931653cfab1b980036800482cf0ad`  
		Last Modified: Tue, 25 Oct 2022 01:18:39 GMT  
		Size: 53.3 MB (53279106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1e8478a953d3a464d73e36e4032c979725bc79ce0eeb83aca30212de549b90`  
		Last Modified: Tue, 25 Oct 2022 02:49:32 GMT  
		Size: 5.1 MB (5148477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cdbee45ed722bfaf7e9ba90503afa7a0cf17b87fc1bfa1e87cbf49ca6bd7d9`  
		Last Modified: Tue, 25 Oct 2022 02:49:33 GMT  
		Size: 10.8 MB (10766704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76aacd12f54fec6c8f627f09641ea144eb6fefeebc8f9fc35de80c3e3ab11af7`  
		Last Modified: Tue, 25 Oct 2022 02:49:48 GMT  
		Size: 54.1 MB (54055853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f33c726ca8131121c45361c5d4789cbb8c58f1cf53f551af6b41f3857cb9847`  
		Last Modified: Tue, 25 Oct 2022 02:50:20 GMT  
		Size: 172.8 MB (172837894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stable-curl`

```console
$ docker pull buildpack-deps@sha256:f0bc68399bc76e1d562de8399f0fb2990e3bd6cc04aab46bb2eb6d789905caef
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
$ docker pull buildpack-deps@sha256:cb9a3f7bd43628db1b3695a6e7b28d561bf4df306ab1f63a0c232397690bf2dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.1 MB (71086032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1e2c1abde86fb7ff272adfa86162471d1bfa52060a0dec82087fecebdcb31e5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:27 GMT
ADD file:d1268789456d2cdace6e50149e60404ad5a849b7c61e8fc8bc7b6e0eb6eeb7ca in / 
# Tue, 04 Oct 2022 23:26:27 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:54:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:55:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f606d8928ed378229f2460b94b504cca239fb906efc57acbdf9340bd298d5ddf`  
		Last Modified: Tue, 04 Oct 2022 23:30:27 GMT  
		Size: 55.0 MB (55046248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47db815c6a4547dc224b75222193cb1851cf529d2cbdf26f854b9bbf97099b98`  
		Last Modified: Wed, 05 Oct 2022 01:19:13 GMT  
		Size: 5.2 MB (5163279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf48494000001a037b72870d2a6a2536f9da8bc5d1ceddd72d79f4a51fe7a60e`  
		Last Modified: Wed, 05 Oct 2022 01:19:13 GMT  
		Size: 10.9 MB (10876505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:c4307444787732144220d75296f55023fa4114b856df149c28e78559c50359d4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.2 MB (68193987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e39186554e8bc668aa17c37b50cd6803d4a408a41ad404ba37b3e10e2ed96267`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:06:19 GMT
ADD file:b314b98654e8532fd10a08a172ea5c3edb7d7a36c7faf85d06d14be12f7b83ef in / 
# Tue, 25 Oct 2022 03:06:19 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:12:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:12:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1f0ecb08923b99bef3f82c2e88603bb53e3ed084c13252275c05039cc279c158`  
		Last Modified: Tue, 25 Oct 2022 03:11:15 GMT  
		Size: 52.5 MB (52547473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b399c5eb53b4c35fa33682a82d73bdc4b096cd78ae95fe36c4ed81d18f6849`  
		Last Modified: Tue, 25 Oct 2022 06:19:02 GMT  
		Size: 5.1 MB (5072235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ccdd06393cd3873a3cc8b9cbe170a2032fd61d1d545b7045b649faf2f4e732`  
		Last Modified: Tue, 25 Oct 2022 06:19:02 GMT  
		Size: 10.6 MB (10574279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:fa161c8e7935e0810bcd3ca45a9746cf6e3fdc6025c5362e8bc2648f7fae6239
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65358325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b86ef37d02c678f38add592f5f88e1f266a851783e8f323eb1837a5ee7352ac7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:28 GMT
ADD file:47a3f2948af18c39686ca59a88a439c25edaf286064d3a2ccc5dab47fee2fc52 in / 
# Tue, 04 Oct 2022 23:58:29 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:32:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:32:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e19342fb46cabf6147aec1d1c6af1f3a82736530cf3b067835fc8a09da092ce3`  
		Last Modified: Wed, 05 Oct 2022 00:04:36 GMT  
		Size: 50.2 MB (50209087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a49f93f990f17337480b5bdf526a6bb48d1ae63bd17f54be17cd2f6ebba4de7d`  
		Last Modified: Wed, 05 Oct 2022 00:53:28 GMT  
		Size: 4.9 MB (4931366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3989be0d7ed2f72fae0310039043f6ba76c24a45f9ec9689697ebd932845cc8`  
		Last Modified: Wed, 05 Oct 2022 00:53:28 GMT  
		Size: 10.2 MB (10217872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:bc7e9978ee6d44bb721af5cba9e40ee69de8d269140ec556a0c40cbeee8979bb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.7 MB (69727646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c88b9fd10ad56e7d5bac1e3cb67021a7765c589e6e7d144f46d1c76d2811413d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:45:55 GMT
ADD file:b16745ece8ef84c028d7e9ac4bf026ac64f885d4170bfcc9d435f237144a1b99 in / 
# Tue, 25 Oct 2022 05:45:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:58:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:58:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8e1d92e7d04d2a9a9880cb45dc3c32c2805912cd86abed96d0ada3ff28748205`  
		Last Modified: Tue, 25 Oct 2022 05:48:40 GMT  
		Size: 53.7 MB (53701966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66eadbf427bb41b3e329a95935c65b09c6d3b7a9c2fa8e08417e497df02ed996`  
		Last Modified: Tue, 25 Oct 2022 08:30:22 GMT  
		Size: 5.2 MB (5151506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9731f4e3bc3680179c10cece663cf0cfe0488918d6795406f4b76f07b787de`  
		Last Modified: Tue, 25 Oct 2022 08:30:22 GMT  
		Size: 10.9 MB (10874174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:bf477637cd09b9031cd034fff22d013e90a3101df053d80729d928601fb7c14a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.1 MB (72143373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b4b083b9d9929246daf9a5fe0622f9a1e88bfb618b352807b23b97d75ff5a38`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:22:19 GMT
ADD file:aa26f69b37c3e144d08e17bb9be7302ec89ae0579121c874a35f336d7077fd3b in / 
# Tue, 25 Oct 2022 02:22:19 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:15:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:15:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8caf426a2703f99fb0be4b03411ecaa580d102f7c47ef43b422b6d7c13c380e2`  
		Last Modified: Tue, 25 Oct 2022 02:27:54 GMT  
		Size: 56.0 MB (56023960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b92a2ff5c72653a0679aa7f5e2bc695011c0a71faa424229e560957d204dab`  
		Last Modified: Tue, 25 Oct 2022 05:27:37 GMT  
		Size: 5.1 MB (5086887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6856a3002e686ceb6d48d078731366f576ed3adcb73bd49dcb300057732904`  
		Last Modified: Tue, 25 Oct 2022 05:27:38 GMT  
		Size: 11.0 MB (11032526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:668f750c6d59a65e45714ebe9fd3c02e2b07e166cf39df660a4b93a59449e9ad
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68845705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e70040762c35b1ea015572f262495cddda025b3d915f9fbfa15e0a0f6b02130`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:09:48 GMT
ADD file:ca40db2df3dbc600910b8cd139c564cf5b8bd6c1a06cc517cae2c1c05cff6dde in / 
# Wed, 05 Oct 2022 00:09:51 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:11:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:12:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:25bcd35faf05f859c3077f0e2e7010d24e56cdcfb77efbdeda236e47dc08e14a`  
		Last Modified: Wed, 05 Oct 2022 00:17:52 GMT  
		Size: 53.3 MB (53265834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c44f381e4f9f5eb923a09cbd49bc86d3d36121137c1e063d30d73af518bf0f86`  
		Last Modified: Wed, 05 Oct 2022 01:32:02 GMT  
		Size: 4.9 MB (4918634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59260097f47eb21e87461a2a98c76f46372dd316b878bbd3d4d9c51cc28a62b7`  
		Last Modified: Wed, 05 Oct 2022 01:32:04 GMT  
		Size: 10.7 MB (10661237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:469e7517e99c19831cea091b8ba496389124880b75d31d2718cc6c1999060b8e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.0 MB (75961034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5cb6ede5f74b2e5a7f231d8ef2d1f5728c8b419020b8d7640b6aaef3bdfe00e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:13:28 GMT
ADD file:c01a6cc4222fbeeda5c2d679c5b355539880a02c792c64861eb17b81a3678f45 in / 
# Tue, 25 Oct 2022 03:13:31 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:13:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:14:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ee5a342763ed1d31bef8cebe9f4cc5dd6d427f630da679a87da0427be7b22e3d`  
		Last Modified: Tue, 25 Oct 2022 03:18:52 GMT  
		Size: 58.9 MB (58916374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a4727f39cbcb19b39abdbd847eeceed842ef65f8514372024c48b913bc951a`  
		Last Modified: Tue, 25 Oct 2022 06:49:00 GMT  
		Size: 5.4 MB (5414507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe601e6c8a1ec9c69c49c65a53339202a65cea9d4f01d161fb34905c06a4a99`  
		Last Modified: Tue, 25 Oct 2022 06:49:01 GMT  
		Size: 11.6 MB (11630153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:809d9d381f46cf97b2154255bf1ab72c6c7126ca14bef3939630abde9638783d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69194287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14cce275c18bfdc19a1e7f27773751920f1a720c0ccd64c54a8ace1b33e0cf31`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:14:24 GMT
ADD file:06f15d8a3c04752d271a052e820fb13fcdb76f0d18f6c9afb6e70391d10348ec in / 
# Tue, 25 Oct 2022 01:14:27 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:31:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:31:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a556186e8bea4ba9925d0c17bea2c12bfbb931653cfab1b980036800482cf0ad`  
		Last Modified: Tue, 25 Oct 2022 01:18:39 GMT  
		Size: 53.3 MB (53279106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1e8478a953d3a464d73e36e4032c979725bc79ce0eeb83aca30212de549b90`  
		Last Modified: Tue, 25 Oct 2022 02:49:32 GMT  
		Size: 5.1 MB (5148477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cdbee45ed722bfaf7e9ba90503afa7a0cf17b87fc1bfa1e87cbf49ca6bd7d9`  
		Last Modified: Tue, 25 Oct 2022 02:49:33 GMT  
		Size: 10.8 MB (10766704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stable-scm`

```console
$ docker pull buildpack-deps@sha256:a7f1c200cd1fd667d3fec5bd3b69dd3672603ce21b7b67891fb7d3a5218874e2
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
$ docker pull buildpack-deps@sha256:fd04e21a45663223207243344f0ac8b1d9c0fe01b1b8601b25d5686a0fdbaa2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125670325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82ff4917fce4dadc637924ff195fcebb04273691c7152bcc869fb766c88d8e15`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:27 GMT
ADD file:d1268789456d2cdace6e50149e60404ad5a849b7c61e8fc8bc7b6e0eb6eeb7ca in / 
# Tue, 04 Oct 2022 23:26:27 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:54:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:55:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:55:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f606d8928ed378229f2460b94b504cca239fb906efc57acbdf9340bd298d5ddf`  
		Last Modified: Tue, 04 Oct 2022 23:30:27 GMT  
		Size: 55.0 MB (55046248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47db815c6a4547dc224b75222193cb1851cf529d2cbdf26f854b9bbf97099b98`  
		Last Modified: Wed, 05 Oct 2022 01:19:13 GMT  
		Size: 5.2 MB (5163279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf48494000001a037b72870d2a6a2536f9da8bc5d1ceddd72d79f4a51fe7a60e`  
		Last Modified: Wed, 05 Oct 2022 01:19:13 GMT  
		Size: 10.9 MB (10876505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a572f7a256d36a93ab0777949771b120c5d7dce75ea2a2d3d9444793b26b2ef1`  
		Last Modified: Wed, 05 Oct 2022 01:19:34 GMT  
		Size: 54.6 MB (54584293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:b510585c7c0379882b7436c2ba9f2bcdf9fa4cadd1aa9e71b177f1bb9bcc57e5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.5 MB (120516144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b46050aede040f8a40b0df16c1d9ec4720cde12aeb7b220cd6ac40588a3ddeb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:06:19 GMT
ADD file:b314b98654e8532fd10a08a172ea5c3edb7d7a36c7faf85d06d14be12f7b83ef in / 
# Tue, 25 Oct 2022 03:06:19 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:12:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:12:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:12:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1f0ecb08923b99bef3f82c2e88603bb53e3ed084c13252275c05039cc279c158`  
		Last Modified: Tue, 25 Oct 2022 03:11:15 GMT  
		Size: 52.5 MB (52547473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b399c5eb53b4c35fa33682a82d73bdc4b096cd78ae95fe36c4ed81d18f6849`  
		Last Modified: Tue, 25 Oct 2022 06:19:02 GMT  
		Size: 5.1 MB (5072235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ccdd06393cd3873a3cc8b9cbe170a2032fd61d1d545b7045b649faf2f4e732`  
		Last Modified: Tue, 25 Oct 2022 06:19:02 GMT  
		Size: 10.6 MB (10574279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aafe0e287af4e488dcda51195e4eb1ae1386e3265989c457172f32f6357bf26`  
		Last Modified: Tue, 25 Oct 2022 06:19:28 GMT  
		Size: 52.3 MB (52322157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:50a85a985b089ddf5972b836da6a0053b066b489827aa55bac5f7bec2bf93ffa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.7 MB (115701649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30f987ffe03e99e4f18811a3ed9c6b544fa00393058f4ef2abb83df5bc1d7673`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:28 GMT
ADD file:47a3f2948af18c39686ca59a88a439c25edaf286064d3a2ccc5dab47fee2fc52 in / 
# Tue, 04 Oct 2022 23:58:29 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:32:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:32:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:32:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e19342fb46cabf6147aec1d1c6af1f3a82736530cf3b067835fc8a09da092ce3`  
		Last Modified: Wed, 05 Oct 2022 00:04:36 GMT  
		Size: 50.2 MB (50209087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a49f93f990f17337480b5bdf526a6bb48d1ae63bd17f54be17cd2f6ebba4de7d`  
		Last Modified: Wed, 05 Oct 2022 00:53:28 GMT  
		Size: 4.9 MB (4931366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3989be0d7ed2f72fae0310039043f6ba76c24a45f9ec9689697ebd932845cc8`  
		Last Modified: Wed, 05 Oct 2022 00:53:28 GMT  
		Size: 10.2 MB (10217872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6487a2e4236617393a6184f0f89a360d295ab118da2ea4ad48fa8645ae211755`  
		Last Modified: Wed, 05 Oct 2022 00:53:57 GMT  
		Size: 50.3 MB (50343324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:8b048c050c2a3ff92ba38fbbe2ceb6d4523c5c2d90dc3ef032dbe78ce741b7c5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124411636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c203e5804baca6a5e5ee110aa8b5c855e1af7aa5b84d282751a6ee78a938f3e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:45:55 GMT
ADD file:b16745ece8ef84c028d7e9ac4bf026ac64f885d4170bfcc9d435f237144a1b99 in / 
# Tue, 25 Oct 2022 05:45:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:58:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:58:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 07:59:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8e1d92e7d04d2a9a9880cb45dc3c32c2805912cd86abed96d0ada3ff28748205`  
		Last Modified: Tue, 25 Oct 2022 05:48:40 GMT  
		Size: 53.7 MB (53701966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66eadbf427bb41b3e329a95935c65b09c6d3b7a9c2fa8e08417e497df02ed996`  
		Last Modified: Tue, 25 Oct 2022 08:30:22 GMT  
		Size: 5.2 MB (5151506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9731f4e3bc3680179c10cece663cf0cfe0488918d6795406f4b76f07b787de`  
		Last Modified: Tue, 25 Oct 2022 08:30:22 GMT  
		Size: 10.9 MB (10874174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d337cb12fd7c6fe341850cd38e880f1806d49a65832c9804b06d00f9032382e0`  
		Last Modified: Tue, 25 Oct 2022 08:30:42 GMT  
		Size: 54.7 MB (54683990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:af3f07f28271542b5cad16677fb8b3eca0cf0897adac022669fd5d2aabbf004d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.1 MB (128067777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41c2e7cc3bce85c55d7b854c187796f854d5d152784c6759eaa5aa5c6dbdc665`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:22:19 GMT
ADD file:aa26f69b37c3e144d08e17bb9be7302ec89ae0579121c874a35f336d7077fd3b in / 
# Tue, 25 Oct 2022 02:22:19 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:15:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:15:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 05:15:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8caf426a2703f99fb0be4b03411ecaa580d102f7c47ef43b422b6d7c13c380e2`  
		Last Modified: Tue, 25 Oct 2022 02:27:54 GMT  
		Size: 56.0 MB (56023960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b92a2ff5c72653a0679aa7f5e2bc695011c0a71faa424229e560957d204dab`  
		Last Modified: Tue, 25 Oct 2022 05:27:37 GMT  
		Size: 5.1 MB (5086887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6856a3002e686ceb6d48d078731366f576ed3adcb73bd49dcb300057732904`  
		Last Modified: Tue, 25 Oct 2022 05:27:38 GMT  
		Size: 11.0 MB (11032526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e88080d3b5ba1edc8623a97d068bd040dfb89f2bc7bdfc0984d11fc35ff5885`  
		Last Modified: Tue, 25 Oct 2022 05:28:00 GMT  
		Size: 55.9 MB (55924404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:a1acaa6746ce03d5ac1c9c184b9983adf517c0cc252294f448e9e9c51580b9c7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122150421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfa73d3a5551fa701da480cd6d0b3d216e9aace1ea0d1de8201cd9fe13f05ce5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:09:48 GMT
ADD file:ca40db2df3dbc600910b8cd139c564cf5b8bd6c1a06cc517cae2c1c05cff6dde in / 
# Wed, 05 Oct 2022 00:09:51 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:11:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:12:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:14:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:25bcd35faf05f859c3077f0e2e7010d24e56cdcfb77efbdeda236e47dc08e14a`  
		Last Modified: Wed, 05 Oct 2022 00:17:52 GMT  
		Size: 53.3 MB (53265834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c44f381e4f9f5eb923a09cbd49bc86d3d36121137c1e063d30d73af518bf0f86`  
		Last Modified: Wed, 05 Oct 2022 01:32:02 GMT  
		Size: 4.9 MB (4918634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59260097f47eb21e87461a2a98c76f46372dd316b878bbd3d4d9c51cc28a62b7`  
		Last Modified: Wed, 05 Oct 2022 01:32:04 GMT  
		Size: 10.7 MB (10661237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f8a68e1316af16785650ca91231ed6373810fcdaff8fb5bec9f58e1ccc2a32`  
		Last Modified: Wed, 05 Oct 2022 01:32:53 GMT  
		Size: 53.3 MB (53304716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:aa6dce1df8020e1e65a5969cd4d256313e3e6bf82526d3774527163c0d3d6b6f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134828389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd50ae9ad837d99d2a9f89b2818813787249d3ea2cd98a78affb4ac0a45caa6d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:13:28 GMT
ADD file:c01a6cc4222fbeeda5c2d679c5b355539880a02c792c64861eb17b81a3678f45 in / 
# Tue, 25 Oct 2022 03:13:31 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:13:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:14:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:14:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ee5a342763ed1d31bef8cebe9f4cc5dd6d427f630da679a87da0427be7b22e3d`  
		Last Modified: Tue, 25 Oct 2022 03:18:52 GMT  
		Size: 58.9 MB (58916374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a4727f39cbcb19b39abdbd847eeceed842ef65f8514372024c48b913bc951a`  
		Last Modified: Tue, 25 Oct 2022 06:49:00 GMT  
		Size: 5.4 MB (5414507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe601e6c8a1ec9c69c49c65a53339202a65cea9d4f01d161fb34905c06a4a99`  
		Last Modified: Tue, 25 Oct 2022 06:49:01 GMT  
		Size: 11.6 MB (11630153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5055e27b58426c2b637b1c8c179e6abe306e3dfb55a9c170c73fb0d581c6cf3e`  
		Last Modified: Tue, 25 Oct 2022 06:49:31 GMT  
		Size: 58.9 MB (58867355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:eba01f860d7d3264a146b7ec7242b3002fd04f91a81d12f89260377ac201f374
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.3 MB (123250140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d21933a18810ed510258d911e9f0408303556697f423746d2ecbcdb6d9df700`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:14:24 GMT
ADD file:06f15d8a3c04752d271a052e820fb13fcdb76f0d18f6c9afb6e70391d10348ec in / 
# Tue, 25 Oct 2022 01:14:27 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:31:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:31:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 02:31:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a556186e8bea4ba9925d0c17bea2c12bfbb931653cfab1b980036800482cf0ad`  
		Last Modified: Tue, 25 Oct 2022 01:18:39 GMT  
		Size: 53.3 MB (53279106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1e8478a953d3a464d73e36e4032c979725bc79ce0eeb83aca30212de549b90`  
		Last Modified: Tue, 25 Oct 2022 02:49:32 GMT  
		Size: 5.1 MB (5148477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cdbee45ed722bfaf7e9ba90503afa7a0cf17b87fc1bfa1e87cbf49ca6bd7d9`  
		Last Modified: Tue, 25 Oct 2022 02:49:33 GMT  
		Size: 10.8 MB (10766704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76aacd12f54fec6c8f627f09641ea144eb6fefeebc8f9fc35de80c3e3ab11af7`  
		Last Modified: Tue, 25 Oct 2022 02:49:48 GMT  
		Size: 54.1 MB (54055853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:testing`

```console
$ docker pull buildpack-deps@sha256:2b1077fc56cdca828f6c4f2fa98e5d65c4b046f877a626cca060199cb08b551e
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
$ docker pull buildpack-deps@sha256:d02593a621ee4f4e7e1fcf39298988b2d0ed222e1d591c59c1d473821d34b6f0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.9 MB (344906770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f0c0cbc5ed6d6e7cc27ef5c4f8b20fdb7085d85320252f8db1c8f63fc75f111`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:03 GMT
ADD file:ca5a5911d0951e5c75f1790eb644a6fd41dcb9712fa2af0fb6d3a537a72e6ad8 in / 
# Tue, 04 Oct 2022 23:26:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:52:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:52:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:52:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:54:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6674a3ae4f8f54c2f747bad2069e50ce00e352d650887729310d984cebecea22`  
		Last Modified: Tue, 04 Oct 2022 23:29:50 GMT  
		Size: 53.0 MB (52962415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e064222ce493e48ae4ceac8f18316e08d2afb963ad57bd63b8630a0ae009f8`  
		Last Modified: Wed, 05 Oct 2022 01:18:07 GMT  
		Size: 9.3 MB (9298646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab229472e3a483409ce2bbc4d461fc6512c03c687daf6546b52705bc7f18961`  
		Last Modified: Wed, 05 Oct 2022 01:18:08 GMT  
		Size: 11.4 MB (11381655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93a5a87ebbd4472db252972521c82b5789bcc45b6bf1ff4d5e59ab129a4847a`  
		Last Modified: Wed, 05 Oct 2022 01:18:25 GMT  
		Size: 57.2 MB (57201277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:685ee8ce50d5fd303a9b0b6cb4cdf889b35afe78677a8c5006983f396b8fca18`  
		Last Modified: Wed, 05 Oct 2022 01:19:02 GMT  
		Size: 214.1 MB (214062777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:d7f420e4177af2c9b91b120ebe9e979d0dcad3966763acb1ed21525041e635fe
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.9 MB (309899153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9046c47430ebdd5f5d55eed0c00fd443d2e16476c60f2500fb777b7b45a350e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:05:47 GMT
ADD file:226ff5e5e8066a03822e2865c6f72c554de94710c5664ee8bebd127d8aa32388 in / 
# Tue, 25 Oct 2022 03:05:48 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:08:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:08:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:09:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:11:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cff7bd795d206b13b585de0da179a0c9616a5278eb7d74a97c97746085567403`  
		Last Modified: Tue, 25 Oct 2022 03:10:30 GMT  
		Size: 50.2 MB (50178371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40202823259eac4be0260092f1fb5f25fa9d866c32ec384dcadb0c7bb6bf8363`  
		Last Modified: Tue, 25 Oct 2022 06:17:42 GMT  
		Size: 8.6 MB (8599297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72794c6cd90917676f9d44ebd1f1f244c5564c41ea99e25ce09ad37df455551`  
		Last Modified: Tue, 25 Oct 2022 06:17:42 GMT  
		Size: 11.5 MB (11507226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0eb73f65f06d3ba6bd41e6c61146c374cf595cc07b9da8e8d08207cdff5b13c`  
		Last Modified: Tue, 25 Oct 2022 06:18:06 GMT  
		Size: 54.8 MB (54848363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7ed4a8a2ecd9b8eaf5a1622f101fd89785ada6f5b963abb9d8a661f9a06bc76`  
		Last Modified: Tue, 25 Oct 2022 06:18:49 GMT  
		Size: 184.8 MB (184765896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f8a1f3a13a8adaaea5da7e387c0c6867d981753b39f1e85cc607bb0e97fa47a7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.6 MB (298606196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:922e36dda65d9735b5f1feb9124dfafb756dd2899076bce2617b826416afae3c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:57:54 GMT
ADD file:9f3a74b8856c0affe36dd4e0700a8a2686a9d2275934fd9af95135f13731d10e in / 
# Tue, 04 Oct 2022 23:57:54 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:29:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:29:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:29:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:32:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b2ee1685df1bf13149eece9e0085c6befe355f21deeea69484a3ab1fab51e40c`  
		Last Modified: Wed, 05 Oct 2022 00:03:53 GMT  
		Size: 49.7 MB (49692608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237b865ef48770b9d41964e18461ec2d393677f4fc653a0953e9f0b9773d47ac`  
		Last Modified: Wed, 05 Oct 2022 00:52:01 GMT  
		Size: 8.4 MB (8396889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902b8eea02f53006b302a3dbae787275ce520ccf78df670e0dcafbfd1c4e17cd`  
		Last Modified: Wed, 05 Oct 2022 00:52:01 GMT  
		Size: 10.7 MB (10661490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540119c620ce1fcebd013dc72077ca8f4751440b9eb633b56bd350f29e749420`  
		Last Modified: Wed, 05 Oct 2022 00:52:26 GMT  
		Size: 53.0 MB (53011353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a5488439a4130d35884d12b04702afc44c003d55109f1c35f807bec217827a`  
		Last Modified: Wed, 05 Oct 2022 00:53:14 GMT  
		Size: 176.8 MB (176843856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ee5b64f7e30f64d230a9ff27700194f9626fb19c2c73fe165d174212296040a2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.6 MB (331564773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84aff2caea9cce7230accd474a102aed797b4fe65257864e59b236a314318e71`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:45:44 GMT
ADD file:83253dd857c3f1ea456b2b77494a2d865a467a36c188ecaeaf493faa5afb4c1c in / 
# Tue, 25 Oct 2022 05:45:44 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:56:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:56:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 07:57:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:58:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bec7a4c1eec818efa32bedb19eba072edfb65db7384f73efc2a6ee7b13a3ca49`  
		Last Modified: Tue, 25 Oct 2022 05:48:08 GMT  
		Size: 51.3 MB (51263048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4dc154ad7b510114eae26976432c9de05c3e285368849cc3bf60481e326fa2`  
		Last Modified: Tue, 25 Oct 2022 08:29:25 GMT  
		Size: 9.0 MB (8982532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4415de5e6c24b057c96d4d8d3d21d5834d4e30729a87dda8eb4f92335d108f53`  
		Last Modified: Tue, 25 Oct 2022 08:29:25 GMT  
		Size: 11.8 MB (11833453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2f80dfabd19f4d09eacf6b535eddbd31119db80916887d34ccb44789d2c48d`  
		Last Modified: Tue, 25 Oct 2022 08:29:42 GMT  
		Size: 57.0 MB (57038097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d56771029d9a89dd111cdb7504b5beb3d00b15609edb9efb094397bcd1b35b`  
		Last Modified: Tue, 25 Oct 2022 08:30:12 GMT  
		Size: 202.4 MB (202447643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; 386

```console
$ docker pull buildpack-deps@sha256:cd231c46916a59c2c2bc5835368b83385c4b55bf48767e2a85292860022b37aa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.5 MB (344545856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a75efaa56b01dda2b7cfee3829312128b18b88f8201eb147e8e83c442bfb2e2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:21:54 GMT
ADD file:f47fc1d53965bb08e38b482e78bd79e3cbeecc53e586ffd88bff0e6fed0a1f3c in / 
# Tue, 25 Oct 2022 02:21:55 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:12:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:12:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 05:13:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:14:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11f88873ba86e184f57ba78457d36c4f22e16eaffb9c293964adc7905e18bfe5`  
		Last Modified: Tue, 25 Oct 2022 02:27:09 GMT  
		Size: 52.2 MB (52224672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:683bf09527f61248ec1a0fa70be7388069c28d961ae31bd3a05c43ae41192a7a`  
		Last Modified: Tue, 25 Oct 2022 05:26:29 GMT  
		Size: 9.3 MB (9330348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823ddfa7a0daf2e9e0c4b6ce038b2e2cce83bde4ba9aef56fb6911d8241ca03d`  
		Last Modified: Tue, 25 Oct 2022 05:26:29 GMT  
		Size: 12.1 MB (12094186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f47813fb488b28b2af09c6f4d188832f52b886546c7885a3bb2d1b67b0d69be`  
		Last Modified: Tue, 25 Oct 2022 05:26:48 GMT  
		Size: 58.6 MB (58616294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7ff00f1ad533c8fdcd88e287626a678680009104d15d1e1eadf92ce8d913b96`  
		Last Modified: Tue, 25 Oct 2022 05:27:25 GMT  
		Size: 212.3 MB (212280356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:e96c56d3802f1d03989d4afc1c9e54f75b256e0ab531932a5452aefc857c2b97
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **319.9 MB (319903659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d117325794165da4de7ce6de9904f16f3847ebfa03ff1dbda099d1546e9c8aba`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:08:36 GMT
ADD file:f17f2d6b2018174ed9b628a69ee630ae6e011a3022bb5a0f3196ef9009d39270 in / 
# Wed, 05 Oct 2022 00:08:41 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:01:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:02:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:04:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:11:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:17006ab86ecbcadb62dabb0d565c7783b28660c51cccb5d7b46f01518a3753a3`  
		Last Modified: Wed, 05 Oct 2022 00:16:34 GMT  
		Size: 53.0 MB (52966979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cc6e8e3ab563929336c7963595d1f292897822342a96c95dcb7cff4bc403b4`  
		Last Modified: Wed, 05 Oct 2022 01:28:47 GMT  
		Size: 8.7 MB (8663556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018c7dae3a16e88ec9bace52486f5c77ed5891921868e64784dd35f09d55ab46`  
		Last Modified: Wed, 05 Oct 2022 01:28:47 GMT  
		Size: 11.1 MB (11128331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e031ef7803b56989f08a0276998fb1edfcabb65ab13ea4a75513a55ad575bc42`  
		Last Modified: Wed, 05 Oct 2022 01:29:37 GMT  
		Size: 56.0 MB (56034915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc6482afe3cbf6106cb4fac04ae9d8ed471a7830e0984fba53bec6d8616c441`  
		Last Modified: Wed, 05 Oct 2022 01:31:49 GMT  
		Size: 191.1 MB (191109878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:10b2439d4c94fc7a0ba39b4e84eaed23c271b8710fe08cfbd1ae8d6f6670d842
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.8 MB (353751941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c23610f60883dea822eec2be63953e6e838d90afc6601ab133f664b2867939f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:12:50 GMT
ADD file:1f55ca9aa64d69398e6bff99fdfd63dbf022ecefc46450a6fd32ae46e9718557 in / 
# Tue, 25 Oct 2022 03:12:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:09:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:09:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:10:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:13:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:264fa02db63011b604885c7feecaeb78fbee4ce4d8191fa5050f4fef88c74001`  
		Last Modified: Tue, 25 Oct 2022 03:18:00 GMT  
		Size: 55.3 MB (55338800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1baf225de572024a1c39187c5ece555fd8056d94bb80d56f889f4e825aa70b`  
		Last Modified: Tue, 25 Oct 2022 06:47:11 GMT  
		Size: 9.7 MB (9732694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55c6a98be02e0940d4fe69cf5b8ef19e3e86304cda7170f1dd085e4a01338a2`  
		Last Modified: Tue, 25 Oct 2022 06:47:11 GMT  
		Size: 12.7 MB (12677561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e65982f752eb81f7771ff52e7dc61db3a43a5e7b89882ff7934a391492daaae`  
		Last Modified: Tue, 25 Oct 2022 06:47:45 GMT  
		Size: 61.9 MB (61899359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3848d68d34827501ccc99d058522edfc766c2b8e572d9746ee9fe584768e46a6`  
		Last Modified: Tue, 25 Oct 2022 06:48:47 GMT  
		Size: 214.1 MB (214103527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3187110300a65451f0ac705920a497de95773130cd67d6e0c464fcd99b688388
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.8 MB (309800763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fa4a44fa173102a4106d3d5e3dafaaa3a72e2769418c8076d5f4f047a14ef7c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:13:56 GMT
ADD file:92a462945d4b32c30f41478992b9ab30d452ac37b0ecef64e2325e4e99296ea8 in / 
# Tue, 25 Oct 2022 01:13:58 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:29:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:29:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 02:30:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:30:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e544dc28605cf962b36f5ba4703f824c022460d64f8973e49764cd76163df5ff`  
		Last Modified: Tue, 25 Oct 2022 01:18:08 GMT  
		Size: 49.6 MB (49578501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50715b09b75ed5a3b59f5532be8529ac130746e899c823894a3ee91fc976a5ed`  
		Last Modified: Tue, 25 Oct 2022 02:48:44 GMT  
		Size: 8.8 MB (8785586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09bb8ed5a6b2d134cb7b866721196b0adaa54ab94d27c13c65773f16fffc143d`  
		Last Modified: Tue, 25 Oct 2022 02:48:44 GMT  
		Size: 11.7 MB (11727044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094b78b28a264fd0d8e36e29b1b3e4c349049eedd6af26957228a4bb291b7f90`  
		Last Modified: Tue, 25 Oct 2022 02:48:58 GMT  
		Size: 56.4 MB (56393185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7928bcdca7e0273482c1c8420378652a6c34aba7f44c83eef04a283ed7cb46da`  
		Last Modified: Tue, 25 Oct 2022 02:49:25 GMT  
		Size: 183.3 MB (183316447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:testing-curl`

```console
$ docker pull buildpack-deps@sha256:e5a6600893bb6c0ca5d5ca3f2563e5500212cced47a82394304054187061a5de
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
$ docker pull buildpack-deps@sha256:65f4152e56d007d77c7d77e60f052056273d3a9ecd93ec0ee27f03e9d06c15a2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73642716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4264bd0b8285ea524f31b2355c6cd723c750a6c269a38987e6a7776185b1666`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:03 GMT
ADD file:ca5a5911d0951e5c75f1790eb644a6fd41dcb9712fa2af0fb6d3a537a72e6ad8 in / 
# Tue, 04 Oct 2022 23:26:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:52:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:52:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6674a3ae4f8f54c2f747bad2069e50ce00e352d650887729310d984cebecea22`  
		Last Modified: Tue, 04 Oct 2022 23:29:50 GMT  
		Size: 53.0 MB (52962415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e064222ce493e48ae4ceac8f18316e08d2afb963ad57bd63b8630a0ae009f8`  
		Last Modified: Wed, 05 Oct 2022 01:18:07 GMT  
		Size: 9.3 MB (9298646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab229472e3a483409ce2bbc4d461fc6512c03c687daf6546b52705bc7f18961`  
		Last Modified: Wed, 05 Oct 2022 01:18:08 GMT  
		Size: 11.4 MB (11381655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:20a4a8343b1da71a409f34e1f00df05ec1afb92deef31bf069ccfcba95ef865a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.3 MB (70284894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50b5509fe779851e321daf80c976e594a6bc3082ea32eb4bd672f0808170781a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:05:47 GMT
ADD file:226ff5e5e8066a03822e2865c6f72c554de94710c5664ee8bebd127d8aa32388 in / 
# Tue, 25 Oct 2022 03:05:48 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:08:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:08:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:cff7bd795d206b13b585de0da179a0c9616a5278eb7d74a97c97746085567403`  
		Last Modified: Tue, 25 Oct 2022 03:10:30 GMT  
		Size: 50.2 MB (50178371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40202823259eac4be0260092f1fb5f25fa9d866c32ec384dcadb0c7bb6bf8363`  
		Last Modified: Tue, 25 Oct 2022 06:17:42 GMT  
		Size: 8.6 MB (8599297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72794c6cd90917676f9d44ebd1f1f244c5564c41ea99e25ce09ad37df455551`  
		Last Modified: Tue, 25 Oct 2022 06:17:42 GMT  
		Size: 11.5 MB (11507226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:5b0dee0e2cc0e1938cf13bff64e7e8012209764899a65e170b1d0ebc91e645e3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68750987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d654a5ab6c7cd35f5bd3a5856e37d1f2b004dd7fd02791250fb62401d704090`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:57:54 GMT
ADD file:9f3a74b8856c0affe36dd4e0700a8a2686a9d2275934fd9af95135f13731d10e in / 
# Tue, 04 Oct 2022 23:57:54 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:29:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:29:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b2ee1685df1bf13149eece9e0085c6befe355f21deeea69484a3ab1fab51e40c`  
		Last Modified: Wed, 05 Oct 2022 00:03:53 GMT  
		Size: 49.7 MB (49692608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237b865ef48770b9d41964e18461ec2d393677f4fc653a0953e9f0b9773d47ac`  
		Last Modified: Wed, 05 Oct 2022 00:52:01 GMT  
		Size: 8.4 MB (8396889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902b8eea02f53006b302a3dbae787275ce520ccf78df670e0dcafbfd1c4e17cd`  
		Last Modified: Wed, 05 Oct 2022 00:52:01 GMT  
		Size: 10.7 MB (10661490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:2ccd628358c05a1df1a611b3f2ddb74940265bbf961c494a44ad3dcdd8faf922
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.1 MB (72079033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bf40f5b1eb3957c789e1c4d10270c32dd0616f31b280461f8d4e00e823a5552`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:45:44 GMT
ADD file:83253dd857c3f1ea456b2b77494a2d865a467a36c188ecaeaf493faa5afb4c1c in / 
# Tue, 25 Oct 2022 05:45:44 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:56:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:56:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:bec7a4c1eec818efa32bedb19eba072edfb65db7384f73efc2a6ee7b13a3ca49`  
		Last Modified: Tue, 25 Oct 2022 05:48:08 GMT  
		Size: 51.3 MB (51263048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4dc154ad7b510114eae26976432c9de05c3e285368849cc3bf60481e326fa2`  
		Last Modified: Tue, 25 Oct 2022 08:29:25 GMT  
		Size: 9.0 MB (8982532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4415de5e6c24b057c96d4d8d3d21d5834d4e30729a87dda8eb4f92335d108f53`  
		Last Modified: Tue, 25 Oct 2022 08:29:25 GMT  
		Size: 11.8 MB (11833453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:167dce0d41220877a7d69d1e1e4402a1f7db01d68c2ede73609723628b0d8d40
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73649206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e11ce92eb7a28e68b38ee4db9094ad80ebf756d2c10f5310aacf4d6fe927bfc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:21:54 GMT
ADD file:f47fc1d53965bb08e38b482e78bd79e3cbeecc53e586ffd88bff0e6fed0a1f3c in / 
# Tue, 25 Oct 2022 02:21:55 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:12:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:12:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:11f88873ba86e184f57ba78457d36c4f22e16eaffb9c293964adc7905e18bfe5`  
		Last Modified: Tue, 25 Oct 2022 02:27:09 GMT  
		Size: 52.2 MB (52224672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:683bf09527f61248ec1a0fa70be7388069c28d961ae31bd3a05c43ae41192a7a`  
		Last Modified: Tue, 25 Oct 2022 05:26:29 GMT  
		Size: 9.3 MB (9330348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823ddfa7a0daf2e9e0c4b6ce038b2e2cce83bde4ba9aef56fb6911d8241ca03d`  
		Last Modified: Tue, 25 Oct 2022 05:26:29 GMT  
		Size: 12.1 MB (12094186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:493af583c74bf77e0b891e256e7da2871572e0ac49991ed4bd9ffed3bc97e620
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.8 MB (72758866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:478aeba09b867d6194866aa4f12b4d9bfb445ad80db4cd1a7f24338c467bc945`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:08:36 GMT
ADD file:f17f2d6b2018174ed9b628a69ee630ae6e011a3022bb5a0f3196ef9009d39270 in / 
# Wed, 05 Oct 2022 00:08:41 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:01:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:02:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:17006ab86ecbcadb62dabb0d565c7783b28660c51cccb5d7b46f01518a3753a3`  
		Last Modified: Wed, 05 Oct 2022 00:16:34 GMT  
		Size: 53.0 MB (52966979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cc6e8e3ab563929336c7963595d1f292897822342a96c95dcb7cff4bc403b4`  
		Last Modified: Wed, 05 Oct 2022 01:28:47 GMT  
		Size: 8.7 MB (8663556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018c7dae3a16e88ec9bace52486f5c77ed5891921868e64784dd35f09d55ab46`  
		Last Modified: Wed, 05 Oct 2022 01:28:47 GMT  
		Size: 11.1 MB (11128331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:8e9cde9494655880ad5e98d1f19c1e7753f180d5e1350dc775dd60d8d1f98846
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.7 MB (77749055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3320b26d31e084b5b012dcb3b58bcd0cddfcb8d3c6ed8349cebe37bed468b61`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:12:50 GMT
ADD file:1f55ca9aa64d69398e6bff99fdfd63dbf022ecefc46450a6fd32ae46e9718557 in / 
# Tue, 25 Oct 2022 03:12:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:09:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:09:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:264fa02db63011b604885c7feecaeb78fbee4ce4d8191fa5050f4fef88c74001`  
		Last Modified: Tue, 25 Oct 2022 03:18:00 GMT  
		Size: 55.3 MB (55338800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1baf225de572024a1c39187c5ece555fd8056d94bb80d56f889f4e825aa70b`  
		Last Modified: Tue, 25 Oct 2022 06:47:11 GMT  
		Size: 9.7 MB (9732694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55c6a98be02e0940d4fe69cf5b8ef19e3e86304cda7170f1dd085e4a01338a2`  
		Last Modified: Tue, 25 Oct 2022 06:47:11 GMT  
		Size: 12.7 MB (12677561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:894b1261a23e6de74babe1ee3f40ba9e50b5c66394124baddfddd8c053c67ccf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.1 MB (70091131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0d41791c8becaef1121c6430e271e2135e1dc7887ebe7a1da86fdacbd5a8eaa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:13:56 GMT
ADD file:92a462945d4b32c30f41478992b9ab30d452ac37b0ecef64e2325e4e99296ea8 in / 
# Tue, 25 Oct 2022 01:13:58 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:29:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:29:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e544dc28605cf962b36f5ba4703f824c022460d64f8973e49764cd76163df5ff`  
		Last Modified: Tue, 25 Oct 2022 01:18:08 GMT  
		Size: 49.6 MB (49578501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50715b09b75ed5a3b59f5532be8529ac130746e899c823894a3ee91fc976a5ed`  
		Last Modified: Tue, 25 Oct 2022 02:48:44 GMT  
		Size: 8.8 MB (8785586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09bb8ed5a6b2d134cb7b866721196b0adaa54ab94d27c13c65773f16fffc143d`  
		Last Modified: Tue, 25 Oct 2022 02:48:44 GMT  
		Size: 11.7 MB (11727044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:testing-scm`

```console
$ docker pull buildpack-deps@sha256:b9e0da7d52fc1e1ef0815334215b86b36631a7e6608bced2cd595865dfa67fea
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
$ docker pull buildpack-deps@sha256:000ac73bce79972e52d53c962a31162be24fdc559f0538904ee6a0150d222c68
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.8 MB (130843993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7945f5e0e10aedb5f27374316d0f3c7b5531582fae4f0662e75f879cc562a3f4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:03 GMT
ADD file:ca5a5911d0951e5c75f1790eb644a6fd41dcb9712fa2af0fb6d3a537a72e6ad8 in / 
# Tue, 04 Oct 2022 23:26:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:52:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:52:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:52:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6674a3ae4f8f54c2f747bad2069e50ce00e352d650887729310d984cebecea22`  
		Last Modified: Tue, 04 Oct 2022 23:29:50 GMT  
		Size: 53.0 MB (52962415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e064222ce493e48ae4ceac8f18316e08d2afb963ad57bd63b8630a0ae009f8`  
		Last Modified: Wed, 05 Oct 2022 01:18:07 GMT  
		Size: 9.3 MB (9298646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab229472e3a483409ce2bbc4d461fc6512c03c687daf6546b52705bc7f18961`  
		Last Modified: Wed, 05 Oct 2022 01:18:08 GMT  
		Size: 11.4 MB (11381655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93a5a87ebbd4472db252972521c82b5789bcc45b6bf1ff4d5e59ab129a4847a`  
		Last Modified: Wed, 05 Oct 2022 01:18:25 GMT  
		Size: 57.2 MB (57201277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:bd890e3ac7fa16b49f774875a45a77bb1e7ae1299879970541ab68e599add920
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.1 MB (125133257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a3ab1b7aecdfddcde09b5a928e85f6963370f7286f701da119d78dd0fe10c85`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:05:47 GMT
ADD file:226ff5e5e8066a03822e2865c6f72c554de94710c5664ee8bebd127d8aa32388 in / 
# Tue, 25 Oct 2022 03:05:48 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:08:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:08:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:09:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cff7bd795d206b13b585de0da179a0c9616a5278eb7d74a97c97746085567403`  
		Last Modified: Tue, 25 Oct 2022 03:10:30 GMT  
		Size: 50.2 MB (50178371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40202823259eac4be0260092f1fb5f25fa9d866c32ec384dcadb0c7bb6bf8363`  
		Last Modified: Tue, 25 Oct 2022 06:17:42 GMT  
		Size: 8.6 MB (8599297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72794c6cd90917676f9d44ebd1f1f244c5564c41ea99e25ce09ad37df455551`  
		Last Modified: Tue, 25 Oct 2022 06:17:42 GMT  
		Size: 11.5 MB (11507226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0eb73f65f06d3ba6bd41e6c61146c374cf595cc07b9da8e8d08207cdff5b13c`  
		Last Modified: Tue, 25 Oct 2022 06:18:06 GMT  
		Size: 54.8 MB (54848363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:2daee8056defbefb7c44552cd1459e5679697f2c0b0d6dcea2ec5040b4ea1137
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121762340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65bd8e30ab8ce2052ff48b213f632b23717eb24125bc8a555a52332d56a64ce4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:57:54 GMT
ADD file:9f3a74b8856c0affe36dd4e0700a8a2686a9d2275934fd9af95135f13731d10e in / 
# Tue, 04 Oct 2022 23:57:54 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:29:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:29:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:29:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b2ee1685df1bf13149eece9e0085c6befe355f21deeea69484a3ab1fab51e40c`  
		Last Modified: Wed, 05 Oct 2022 00:03:53 GMT  
		Size: 49.7 MB (49692608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237b865ef48770b9d41964e18461ec2d393677f4fc653a0953e9f0b9773d47ac`  
		Last Modified: Wed, 05 Oct 2022 00:52:01 GMT  
		Size: 8.4 MB (8396889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902b8eea02f53006b302a3dbae787275ce520ccf78df670e0dcafbfd1c4e17cd`  
		Last Modified: Wed, 05 Oct 2022 00:52:01 GMT  
		Size: 10.7 MB (10661490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540119c620ce1fcebd013dc72077ca8f4751440b9eb633b56bd350f29e749420`  
		Last Modified: Wed, 05 Oct 2022 00:52:26 GMT  
		Size: 53.0 MB (53011353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:04516cc98d3556b69d602a778fcc926cd176190c038ce4d315c5cf14d37b282a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.1 MB (129117130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41da76e26040b5bf1fc2bcaf32382c780d6103a841e405cfa8abb0442b2e3c87`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:45:44 GMT
ADD file:83253dd857c3f1ea456b2b77494a2d865a467a36c188ecaeaf493faa5afb4c1c in / 
# Tue, 25 Oct 2022 05:45:44 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:56:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:56:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 07:57:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bec7a4c1eec818efa32bedb19eba072edfb65db7384f73efc2a6ee7b13a3ca49`  
		Last Modified: Tue, 25 Oct 2022 05:48:08 GMT  
		Size: 51.3 MB (51263048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4dc154ad7b510114eae26976432c9de05c3e285368849cc3bf60481e326fa2`  
		Last Modified: Tue, 25 Oct 2022 08:29:25 GMT  
		Size: 9.0 MB (8982532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4415de5e6c24b057c96d4d8d3d21d5834d4e30729a87dda8eb4f92335d108f53`  
		Last Modified: Tue, 25 Oct 2022 08:29:25 GMT  
		Size: 11.8 MB (11833453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2f80dfabd19f4d09eacf6b535eddbd31119db80916887d34ccb44789d2c48d`  
		Last Modified: Tue, 25 Oct 2022 08:29:42 GMT  
		Size: 57.0 MB (57038097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:bb8f335fbccf0d2040d44a9901f5d5892fddf6faf56f84c2699db34d21e91570
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.3 MB (132265500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:533c3f4baead23baa420e1ab640834843dc1a50aec17fc4a2c085177b12d89ce`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:21:54 GMT
ADD file:f47fc1d53965bb08e38b482e78bd79e3cbeecc53e586ffd88bff0e6fed0a1f3c in / 
# Tue, 25 Oct 2022 02:21:55 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:12:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:12:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 05:13:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11f88873ba86e184f57ba78457d36c4f22e16eaffb9c293964adc7905e18bfe5`  
		Last Modified: Tue, 25 Oct 2022 02:27:09 GMT  
		Size: 52.2 MB (52224672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:683bf09527f61248ec1a0fa70be7388069c28d961ae31bd3a05c43ae41192a7a`  
		Last Modified: Tue, 25 Oct 2022 05:26:29 GMT  
		Size: 9.3 MB (9330348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823ddfa7a0daf2e9e0c4b6ce038b2e2cce83bde4ba9aef56fb6911d8241ca03d`  
		Last Modified: Tue, 25 Oct 2022 05:26:29 GMT  
		Size: 12.1 MB (12094186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f47813fb488b28b2af09c6f4d188832f52b886546c7885a3bb2d1b67b0d69be`  
		Last Modified: Tue, 25 Oct 2022 05:26:48 GMT  
		Size: 58.6 MB (58616294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:c942e931db31d5c2e72264278254cf3270324e3f44fb7f1395d1bb1521d12600
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.8 MB (128793781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40553f8f691301cee00d5f713fbac8c57b59252c2dd9245ae7f5714fe6e1495d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:08:36 GMT
ADD file:f17f2d6b2018174ed9b628a69ee630ae6e011a3022bb5a0f3196ef9009d39270 in / 
# Wed, 05 Oct 2022 00:08:41 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:01:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:02:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:04:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:17006ab86ecbcadb62dabb0d565c7783b28660c51cccb5d7b46f01518a3753a3`  
		Last Modified: Wed, 05 Oct 2022 00:16:34 GMT  
		Size: 53.0 MB (52966979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cc6e8e3ab563929336c7963595d1f292897822342a96c95dcb7cff4bc403b4`  
		Last Modified: Wed, 05 Oct 2022 01:28:47 GMT  
		Size: 8.7 MB (8663556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018c7dae3a16e88ec9bace52486f5c77ed5891921868e64784dd35f09d55ab46`  
		Last Modified: Wed, 05 Oct 2022 01:28:47 GMT  
		Size: 11.1 MB (11128331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e031ef7803b56989f08a0276998fb1edfcabb65ab13ea4a75513a55ad575bc42`  
		Last Modified: Wed, 05 Oct 2022 01:29:37 GMT  
		Size: 56.0 MB (56034915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:8aedd3f69ab37457552ec526445326e02d180a5e2d4fcd5e9921b0acccee7f55
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.6 MB (139648414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06e4d95381966110ef09af6732f8433a26f7b8e7f0895481c387ea2612e84de8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:12:50 GMT
ADD file:1f55ca9aa64d69398e6bff99fdfd63dbf022ecefc46450a6fd32ae46e9718557 in / 
# Tue, 25 Oct 2022 03:12:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:09:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:09:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:10:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:264fa02db63011b604885c7feecaeb78fbee4ce4d8191fa5050f4fef88c74001`  
		Last Modified: Tue, 25 Oct 2022 03:18:00 GMT  
		Size: 55.3 MB (55338800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1baf225de572024a1c39187c5ece555fd8056d94bb80d56f889f4e825aa70b`  
		Last Modified: Tue, 25 Oct 2022 06:47:11 GMT  
		Size: 9.7 MB (9732694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55c6a98be02e0940d4fe69cf5b8ef19e3e86304cda7170f1dd085e4a01338a2`  
		Last Modified: Tue, 25 Oct 2022 06:47:11 GMT  
		Size: 12.7 MB (12677561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e65982f752eb81f7771ff52e7dc61db3a43a5e7b89882ff7934a391492daaae`  
		Last Modified: Tue, 25 Oct 2022 06:47:45 GMT  
		Size: 61.9 MB (61899359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:221812309a8315f40e7a00439dfae7b687e3828c543190683390eec5bc6263dd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126484316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c27b9f13f925e68613971e6806d863cbc335c648a119e6ce33664f7874816557`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:13:56 GMT
ADD file:92a462945d4b32c30f41478992b9ab30d452ac37b0ecef64e2325e4e99296ea8 in / 
# Tue, 25 Oct 2022 01:13:58 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:29:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:29:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 02:30:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e544dc28605cf962b36f5ba4703f824c022460d64f8973e49764cd76163df5ff`  
		Last Modified: Tue, 25 Oct 2022 01:18:08 GMT  
		Size: 49.6 MB (49578501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50715b09b75ed5a3b59f5532be8529ac130746e899c823894a3ee91fc976a5ed`  
		Last Modified: Tue, 25 Oct 2022 02:48:44 GMT  
		Size: 8.8 MB (8785586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09bb8ed5a6b2d134cb7b866721196b0adaa54ab94d27c13c65773f16fffc143d`  
		Last Modified: Tue, 25 Oct 2022 02:48:44 GMT  
		Size: 11.7 MB (11727044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094b78b28a264fd0d8e36e29b1b3e4c349049eedd6af26957228a4bb291b7f90`  
		Last Modified: Tue, 25 Oct 2022 02:48:58 GMT  
		Size: 56.4 MB (56393185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:unstable`

```console
$ docker pull buildpack-deps@sha256:37ddbe39fcb9a1fe2dd11c2f9b2ce45d101b51ae6228ffd1825f50fe435a49a3
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
$ docker pull buildpack-deps@sha256:a5c9c277142466a2cb13602a341189d974508866b334634253b4cd510d06669b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.9 MB (351931474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b61eb60b50a71a4c3e73ad9d3d992525ea6f399f1983ef31929b5d74b86a19a9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:27:32 GMT
ADD file:b2f29ff1f75077ccce680becaa7bffdc9dfb9c7938188e93673e1b42bf418630 in / 
# Tue, 04 Oct 2022 23:27:32 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:58:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:59:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:59:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:00:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a9fedee3000f9dcc2b77410cd53420ec321135a3f7a6c688b43f31e503042e1e`  
		Last Modified: Tue, 04 Oct 2022 23:32:34 GMT  
		Size: 52.7 MB (52684279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dda17d2d1d2961ba6c7083d3013dde5fb5af68bd80ee1e40adbf7886b64df3c`  
		Last Modified: Wed, 05 Oct 2022 01:21:27 GMT  
		Size: 9.3 MB (9300772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809d617f2e2db52d55fec066a28a409d69e1dc40dd9f91f7f03c19ec8d16c587`  
		Last Modified: Wed, 05 Oct 2022 01:21:27 GMT  
		Size: 11.4 MB (11382118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15dd69568329cc8f49552e84cc7a6c0a0c112efb493830d52d7c1c6ed88af8f`  
		Last Modified: Wed, 05 Oct 2022 01:21:45 GMT  
		Size: 58.1 MB (58052906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5107ea815e7c65b0f723ec6d8f3b5ed3eb7461e8f79537b8c5e719f0a4b7ae59`  
		Last Modified: Wed, 05 Oct 2022 01:22:23 GMT  
		Size: 220.5 MB (220511399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:053914e76c7ba60fb11f8cc6b92d31100985ad00c304f22cdbd935f9d1ce6d11
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.4 MB (309384964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20043e26391a12bbe81aaa2a4a2e9f2aca2ae66853c067fdbe991c88c12d0d99`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:06:50 GMT
ADD file:829f8e96e527611e85aa710b19c01c75a4760a27c651fb439f8cdb5609db64aa in / 
# Tue, 25 Oct 2022 03:06:52 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:14:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:14:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:15:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:16:24 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:513ea4862e78a8cc07ed6d320f10e746ca770eb039dec1548c31a9de19d1f7ce`  
		Last Modified: Tue, 25 Oct 2022 03:12:19 GMT  
		Size: 49.6 MB (49578888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1ace4b71d48c3105e8f55674a41898f6b1df73d7ee8b05d5c3d3b3fea66077`  
		Last Modified: Tue, 25 Oct 2022 06:20:29 GMT  
		Size: 8.5 MB (8548544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:428ee02803cd3666baa3051b15b273e86d1d20710ddd79191fb1367a0dda5edc`  
		Last Modified: Tue, 25 Oct 2022 06:20:29 GMT  
		Size: 10.8 MB (10829764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecfb58f8aebfa286f964add0eb9b5f5bf243c4e6b5c934809df2c000acf0301c`  
		Last Modified: Tue, 25 Oct 2022 06:20:53 GMT  
		Size: 55.5 MB (55547745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f507c760cb7666ec153f5bbf4e7065ca52ffbd950406148854ca9ac024d521d1`  
		Last Modified: Tue, 25 Oct 2022 06:21:36 GMT  
		Size: 184.9 MB (184880023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:50db74bb547c5b2b61e9d0061572cf34d1f9a2691617b0af1f821bfee6452528
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.9 MB (305910529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae94c0dd0c97e61628259977275ebed18a549a46b30661e06c76d8622bde7b47`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:00:01 GMT
ADD file:41046e966f37a45410c2aa02920b78f877f5aacb6ee087b2c6c6642f4e7b474f in / 
# Wed, 05 Oct 2022 00:00:02 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:38:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:38:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:38:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:40:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1316bf5b10f256f27feadcb25edef6365e912773e60cc382610ef003daf37248`  
		Last Modified: Wed, 05 Oct 2022 00:07:10 GMT  
		Size: 49.4 MB (49436823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00270159c4caaec159e25e1eaca6209b11c838dd60b5e0f5194e2279c51cd70`  
		Last Modified: Wed, 05 Oct 2022 00:56:26 GMT  
		Size: 8.4 MB (8399366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8524fd9b0e923155334b98a655b41aa941eb210e3248b7cc375ee49257b2b929`  
		Last Modified: Wed, 05 Oct 2022 00:56:26 GMT  
		Size: 10.7 MB (10663790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92867f6312a37ef5d4d5b38b1944bbe65123c5127a3ace08db615300dfc442c7`  
		Last Modified: Wed, 05 Oct 2022 00:56:52 GMT  
		Size: 53.7 MB (53727748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a7e6fabe704d47681c59355edf9f588b8d1c66996c09a34a3fdb7c42e27a75`  
		Last Modified: Wed, 05 Oct 2022 00:57:45 GMT  
		Size: 183.7 MB (183682802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:b082ee07bc085a1f3753080188e9d8260690c44559ba4829f3bde8da53717a5a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.7 MB (330710877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a3c24ba1239020d15937993d74b20ef109f76f653bb0f857613a9ab6ccb9b80`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:29 GMT
ADD file:6a2d69a5a731490271c915d99634a89755f7236ef56712924ea061730d8552c4 in / 
# Tue, 25 Oct 2022 05:46:30 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:01:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:01:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:02:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:03:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:63a396bb133ce57141398b6c6d776ce17e3e973085b5a1b746d76407240a376a`  
		Last Modified: Tue, 25 Oct 2022 05:50:38 GMT  
		Size: 50.6 MB (50643735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a89cf1bf3c8da06b08672e8551d2511df312e843fb3acab24e31d9ba0afa866`  
		Last Modified: Tue, 25 Oct 2022 08:32:19 GMT  
		Size: 8.9 MB (8932959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e653e6dd7e514d68792b5ac0d2812dbc50a0e1d5c4842fd356c767031c54aec`  
		Last Modified: Tue, 25 Oct 2022 08:32:19 GMT  
		Size: 11.1 MB (11138995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c34d6a76d061ba3fc92256f8a3d68cb9c3d5840430072a886deb01b71229ceba`  
		Last Modified: Tue, 25 Oct 2022 08:32:40 GMT  
		Size: 57.7 MB (57715979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb1960dcbb4deabd508cdae7441ee09f50ac6dbb89cea1922d94adc49db752e`  
		Last Modified: Tue, 25 Oct 2022 08:33:09 GMT  
		Size: 202.3 MB (202279209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:5bd7bb5803c4f0ad919619492abe354c5ff051233d1fd15ab0b702dcd2fc099e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.9 MB (343886877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:881b4643c019f8a58e6490838d5a8ad00df910743f87b1a3e581433aa83888b0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:23:38 GMT
ADD file:80dabb60a37b1d88f3750adb85c9e159d00b55293f70ad93512f94bd3cfd99bc in / 
# Tue, 25 Oct 2022 02:23:39 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:18:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:18:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 05:19:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:20:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:367799113badd94b9683087d6086436649a1fb7127698c42b0d730f5bbedcf86`  
		Last Modified: Tue, 25 Oct 2022 02:30:22 GMT  
		Size: 51.6 MB (51625321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564d2fccc59969c0b37e3bb8384bc6545a4cce125daa11c7e8b599ec0acac788`  
		Last Modified: Tue, 25 Oct 2022 05:30:00 GMT  
		Size: 9.3 MB (9282393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09be9213196e288bdcccf553107591d6fe4f04fccea4da55faea35dd79cfff15`  
		Last Modified: Tue, 25 Oct 2022 05:30:00 GMT  
		Size: 11.4 MB (11379737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7cf8ff2ca1128a94c435416195c01bd46e7b32191a4a225527692f374d4e31e`  
		Last Modified: Tue, 25 Oct 2022 05:30:21 GMT  
		Size: 59.5 MB (59473844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d348a2548fad4997feadc2b7be7e32cc9412c27e3208c57b624b3263c3c096c3`  
		Last Modified: Tue, 25 Oct 2022 05:30:57 GMT  
		Size: 212.1 MB (212125582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:2caaf8b43b29ccbbe6df934dfce764b42a555f9dfc7c3e1a3cc7bf2a9100d322
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.9 MB (326920922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a616d7e3db3ce0164a507b56b89952f874fd85d67230fa9a2a34798f0270ae98`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:11:00 GMT
ADD file:a7d6f7226093388fbc662c6e3fa1bc8dc263ab630fe03ea088486e6b016474ff in / 
# Wed, 05 Oct 2022 00:11:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:20:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:21:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:22:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:28:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3110bff10f823ecdaa06d8f7c65ce83d7c99521680207da9d264aaa8823d5209`  
		Last Modified: Wed, 05 Oct 2022 00:19:21 GMT  
		Size: 52.7 MB (52669988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6422d53934b53541883e4d8479c0384974a4f8c2ca335b2e86b900b4cf761d7d`  
		Last Modified: Wed, 05 Oct 2022 01:35:18 GMT  
		Size: 8.7 MB (8665467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2fd86c88bcf963ae10ae57261059a1b2bdbad2590061f63513acf0308dacf1`  
		Last Modified: Wed, 05 Oct 2022 01:35:18 GMT  
		Size: 11.1 MB (11130537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408a6f9d0ef9c4902e1584d5a5ac4ed8e9e71594c69a06143ca94a9b42bfc026`  
		Last Modified: Wed, 05 Oct 2022 01:36:07 GMT  
		Size: 56.9 MB (56887661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7896915ee9ec5c0e37b59cfbe6d7cb364dff641bd4c04f0160f59fab6e46f072`  
		Last Modified: Wed, 05 Oct 2022 01:38:22 GMT  
		Size: 197.6 MB (197567269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:4a3598d62e23e3003db6e423ae264e43db2ff5657ec189e6f6d00f5c69e85a4b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.0 MB (352964297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:992be19844bb6ce728b69d6af195e74bad155d8b12433dacfa7ba1c518fffaa8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:14:07 GMT
ADD file:6e9efd6bb77c835520332c88cb412f38f0d8573ec3347b090b77965e17131780 in / 
# Tue, 25 Oct 2022 03:14:10 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:17:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:17:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:17:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:19:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a3962f6ac5b86fa159789ea1e9241ecbb956b3223e8312f7d92d7fbb8bf5485`  
		Last Modified: Tue, 25 Oct 2022 03:20:03 GMT  
		Size: 54.7 MB (54704717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c5225e6c97e35e08afc065bed0fb4156a1727da9a3e12b4a611189682c919a`  
		Last Modified: Tue, 25 Oct 2022 06:50:49 GMT  
		Size: 9.7 MB (9684744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39fe7c3b495d9320ca99478bfddf7a3fa0412a37c56ca95a4cc891ceb738e62`  
		Last Modified: Tue, 25 Oct 2022 06:50:49 GMT  
		Size: 11.9 MB (11937807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9270b45cd7087efea37438ff9651d0078e51c8b476b199cfc26770079313e3`  
		Last Modified: Tue, 25 Oct 2022 06:51:17 GMT  
		Size: 62.7 MB (62679073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652adf8e207d919d0f1ddc84ad9fa208e1ec7d27d5573d5c3348e681a13f65b5`  
		Last Modified: Tue, 25 Oct 2022 06:52:18 GMT  
		Size: 214.0 MB (213957956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:3a887968fe43226ca614e3bdfba591197b3593e08bde65a9a38a179bf5715812
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.9 MB (359929860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0617997a465ac3f99d967a05d654c18e959edee32e325b2b1dc07db26768495`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:39:40 GMT
ADD file:cff1e1a432929527e9bb64bde53e2b614c941bd4631b7bd3634fdda8a7240455 in / 
# Wed, 05 Oct 2022 00:39:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:26:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:27:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 02:31:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:40:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9cc6da93595cf4d9d589de999765cc4f1efa5e0d8e23ca6dd8b73b18afdc8189`  
		Last Modified: Wed, 05 Oct 2022 00:57:59 GMT  
		Size: 48.9 MB (48857821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554ce58712f86101a4716baede25ee43c9c1fc550b39fb4b3e5fa1622fd3b00b`  
		Last Modified: Wed, 05 Oct 2022 03:30:22 GMT  
		Size: 8.4 MB (8388012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd132871253f925889ef836099addcf830644843a64a1529bddc510390846a9b`  
		Last Modified: Wed, 05 Oct 2022 03:30:22 GMT  
		Size: 10.8 MB (10750715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bfc76b3f6f1ba447e697e6e2190cf70e757458cce81446b79426ae4cccdb03`  
		Last Modified: Wed, 05 Oct 2022 03:33:00 GMT  
		Size: 54.0 MB (54018661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58e7099a4ad88bc20a780df4c500b9445dc2cb39e8ac84d70a11e8903e5b6448`  
		Last Modified: Wed, 05 Oct 2022 03:40:39 GMT  
		Size: 237.9 MB (237914651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:f3a95238e9fb25bdb30cf9bac9a31017e573719ecc1390cb196795031f399a69
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.9 MB (308907690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b76b4efc93df24f2f1e78a196a448ee70d9bf65a4f671e9a7d61ee0a29bad85`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:14:54 GMT
ADD file:7dba2ae439c9f5da3fe962e867cee94eafc0b12a74939e13fdf987965ef8191c in / 
# Tue, 25 Oct 2022 01:14:57 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:32:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:32:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 02:33:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:33:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1430653806baea9ab2928a0d226c10ba8e7bf4b9b93398f9082ba16edfb2d4b8`  
		Last Modified: Tue, 25 Oct 2022 01:19:17 GMT  
		Size: 49.0 MB (49012977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa67452e329e71787509a1583923b8e1e83b22a2fb76e48111393a03205d4c20`  
		Last Modified: Tue, 25 Oct 2022 02:50:30 GMT  
		Size: 8.7 MB (8738304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7be163526b121ed701b3595b33b6d8755aba04a12b0fd801f9c899cbd3ebd0`  
		Last Modified: Tue, 25 Oct 2022 02:50:30 GMT  
		Size: 11.0 MB (11041665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ea6534b4c7c78beb071314cf02af39dc48f27dffa56b6182c538fc47d868d4`  
		Last Modified: Tue, 25 Oct 2022 02:50:45 GMT  
		Size: 56.9 MB (56939890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e73095f949aa471b5db609eab93348cee45f8092aba617f080c27c32b8c06c`  
		Last Modified: Tue, 25 Oct 2022 02:51:14 GMT  
		Size: 183.2 MB (183174854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:unstable-curl`

```console
$ docker pull buildpack-deps@sha256:d73594bc7e05039d42fa3ad9c5b2daabadc46b38fafe9e9e545616f582643259
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
$ docker pull buildpack-deps@sha256:cc22c156446c9313c4680623e26c6e48bba2f98ec6ce87c8ed3a0d52e716c0a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.4 MB (73367169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87b8c38f75980c2def43a2d61e770ccc0b3c9955ae57c722bb79d7f977a21e31`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:27:32 GMT
ADD file:b2f29ff1f75077ccce680becaa7bffdc9dfb9c7938188e93673e1b42bf418630 in / 
# Tue, 04 Oct 2022 23:27:32 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:58:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:59:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a9fedee3000f9dcc2b77410cd53420ec321135a3f7a6c688b43f31e503042e1e`  
		Last Modified: Tue, 04 Oct 2022 23:32:34 GMT  
		Size: 52.7 MB (52684279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dda17d2d1d2961ba6c7083d3013dde5fb5af68bd80ee1e40adbf7886b64df3c`  
		Last Modified: Wed, 05 Oct 2022 01:21:27 GMT  
		Size: 9.3 MB (9300772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809d617f2e2db52d55fec066a28a409d69e1dc40dd9f91f7f03c19ec8d16c587`  
		Last Modified: Wed, 05 Oct 2022 01:21:27 GMT  
		Size: 11.4 MB (11382118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:003e17008ddaf3d07c54f0e22bf1740953332445e88af588740603583bd313ef
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (68957196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:735e2d1a8b82054ce8ae48afcdbd6e7bd00b34f6107e66adc81d2023c1a0c787`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:06:50 GMT
ADD file:829f8e96e527611e85aa710b19c01c75a4760a27c651fb439f8cdb5609db64aa in / 
# Tue, 25 Oct 2022 03:06:52 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:14:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:14:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:513ea4862e78a8cc07ed6d320f10e746ca770eb039dec1548c31a9de19d1f7ce`  
		Last Modified: Tue, 25 Oct 2022 03:12:19 GMT  
		Size: 49.6 MB (49578888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1ace4b71d48c3105e8f55674a41898f6b1df73d7ee8b05d5c3d3b3fea66077`  
		Last Modified: Tue, 25 Oct 2022 06:20:29 GMT  
		Size: 8.5 MB (8548544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:428ee02803cd3666baa3051b15b273e86d1d20710ddd79191fb1367a0dda5edc`  
		Last Modified: Tue, 25 Oct 2022 06:20:29 GMT  
		Size: 10.8 MB (10829764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:67e81d32e4a379ebc001840f12d827e5f67833629cc8d825dc7e62681fdec972
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68499979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ead5cdfb9f5e5c275759c55be9d11eb1dc155f3aa55dad5b5be0cb66efd70376`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:00:01 GMT
ADD file:41046e966f37a45410c2aa02920b78f877f5aacb6ee087b2c6c6642f4e7b474f in / 
# Wed, 05 Oct 2022 00:00:02 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:38:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:38:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1316bf5b10f256f27feadcb25edef6365e912773e60cc382610ef003daf37248`  
		Last Modified: Wed, 05 Oct 2022 00:07:10 GMT  
		Size: 49.4 MB (49436823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00270159c4caaec159e25e1eaca6209b11c838dd60b5e0f5194e2279c51cd70`  
		Last Modified: Wed, 05 Oct 2022 00:56:26 GMT  
		Size: 8.4 MB (8399366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8524fd9b0e923155334b98a655b41aa941eb210e3248b7cc375ee49257b2b929`  
		Last Modified: Wed, 05 Oct 2022 00:56:26 GMT  
		Size: 10.7 MB (10663790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a0fa7918450dd9fe388abd5681d138ceac42806881b9f01ab9773a5a6cfce977
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.7 MB (70715689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d50f6af0113bc54f7f717b62c4be946ce8984d31d0e202389ef84720e47a647`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:29 GMT
ADD file:6a2d69a5a731490271c915d99634a89755f7236ef56712924ea061730d8552c4 in / 
# Tue, 25 Oct 2022 05:46:30 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:01:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:01:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:63a396bb133ce57141398b6c6d776ce17e3e973085b5a1b746d76407240a376a`  
		Last Modified: Tue, 25 Oct 2022 05:50:38 GMT  
		Size: 50.6 MB (50643735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a89cf1bf3c8da06b08672e8551d2511df312e843fb3acab24e31d9ba0afa866`  
		Last Modified: Tue, 25 Oct 2022 08:32:19 GMT  
		Size: 8.9 MB (8932959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e653e6dd7e514d68792b5ac0d2812dbc50a0e1d5c4842fd356c767031c54aec`  
		Last Modified: Tue, 25 Oct 2022 08:32:19 GMT  
		Size: 11.1 MB (11138995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:7a92edc5d0d1d9b005fc402881b8f8eddac8e13c8f5adf57fb62e1a26d00983d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.3 MB (72287451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b1893a81cbf84a850be47ff4f28e1dd4035b9c2256bdedf86584fb4079c771d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:23:38 GMT
ADD file:80dabb60a37b1d88f3750adb85c9e159d00b55293f70ad93512f94bd3cfd99bc in / 
# Tue, 25 Oct 2022 02:23:39 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:18:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:18:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:367799113badd94b9683087d6086436649a1fb7127698c42b0d730f5bbedcf86`  
		Last Modified: Tue, 25 Oct 2022 02:30:22 GMT  
		Size: 51.6 MB (51625321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564d2fccc59969c0b37e3bb8384bc6545a4cce125daa11c7e8b599ec0acac788`  
		Last Modified: Tue, 25 Oct 2022 05:30:00 GMT  
		Size: 9.3 MB (9282393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09be9213196e288bdcccf553107591d6fe4f04fccea4da55faea35dd79cfff15`  
		Last Modified: Tue, 25 Oct 2022 05:30:00 GMT  
		Size: 11.4 MB (11379737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:177c731ad458bb98287f9b7f0ff300408fc1a53c32e1d406bb638c4c00719d21
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72465992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50d48d0070c45b656746927bfe7b8ec4a82c7b00acdd9cce150d2c20e17feb87`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:11:00 GMT
ADD file:a7d6f7226093388fbc662c6e3fa1bc8dc263ab630fe03ea088486e6b016474ff in / 
# Wed, 05 Oct 2022 00:11:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:20:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:21:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3110bff10f823ecdaa06d8f7c65ce83d7c99521680207da9d264aaa8823d5209`  
		Last Modified: Wed, 05 Oct 2022 00:19:21 GMT  
		Size: 52.7 MB (52669988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6422d53934b53541883e4d8479c0384974a4f8c2ca335b2e86b900b4cf761d7d`  
		Last Modified: Wed, 05 Oct 2022 01:35:18 GMT  
		Size: 8.7 MB (8665467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2fd86c88bcf963ae10ae57261059a1b2bdbad2590061f63513acf0308dacf1`  
		Last Modified: Wed, 05 Oct 2022 01:35:18 GMT  
		Size: 11.1 MB (11130537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:124e076bd786711b687044fd136c24af7bc4500c1e67e6e1f0f4086eedfced08
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.3 MB (76327268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce644126cccec0395c556b7c4763b65ccbe0344029fc1fc5a5a1c93e9d1c4787`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:14:07 GMT
ADD file:6e9efd6bb77c835520332c88cb412f38f0d8573ec3347b090b77965e17131780 in / 
# Tue, 25 Oct 2022 03:14:10 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:17:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:17:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:7a3962f6ac5b86fa159789ea1e9241ecbb956b3223e8312f7d92d7fbb8bf5485`  
		Last Modified: Tue, 25 Oct 2022 03:20:03 GMT  
		Size: 54.7 MB (54704717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c5225e6c97e35e08afc065bed0fb4156a1727da9a3e12b4a611189682c919a`  
		Last Modified: Tue, 25 Oct 2022 06:50:49 GMT  
		Size: 9.7 MB (9684744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39fe7c3b495d9320ca99478bfddf7a3fa0412a37c56ca95a4cc891ceb738e62`  
		Last Modified: Tue, 25 Oct 2022 06:50:49 GMT  
		Size: 11.9 MB (11937807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:91c41397454a62656ddc234f54c6ce9bc6eebb7463198b379aec9760ef9f5ce3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.0 MB (67996548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c82f669a88d6376397cb790855001ce2a2328184d9fc8f1fbf316b588cd40e4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:39:40 GMT
ADD file:cff1e1a432929527e9bb64bde53e2b614c941bd4631b7bd3634fdda8a7240455 in / 
# Wed, 05 Oct 2022 00:39:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:26:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:27:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9cc6da93595cf4d9d589de999765cc4f1efa5e0d8e23ca6dd8b73b18afdc8189`  
		Last Modified: Wed, 05 Oct 2022 00:57:59 GMT  
		Size: 48.9 MB (48857821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554ce58712f86101a4716baede25ee43c9c1fc550b39fb4b3e5fa1622fd3b00b`  
		Last Modified: Wed, 05 Oct 2022 03:30:22 GMT  
		Size: 8.4 MB (8388012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd132871253f925889ef836099addcf830644843a64a1529bddc510390846a9b`  
		Last Modified: Wed, 05 Oct 2022 03:30:22 GMT  
		Size: 10.8 MB (10750715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:459e259ac9d973e273d44f4977a901a7c57dce7f749c5caf0ade7837350bf940
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68792946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8919e63d46a3758bb8046627e26a7d852ed8e26e8b044f56948b519863d33fd4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:14:54 GMT
ADD file:7dba2ae439c9f5da3fe962e867cee94eafc0b12a74939e13fdf987965ef8191c in / 
# Tue, 25 Oct 2022 01:14:57 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:32:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:32:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1430653806baea9ab2928a0d226c10ba8e7bf4b9b93398f9082ba16edfb2d4b8`  
		Last Modified: Tue, 25 Oct 2022 01:19:17 GMT  
		Size: 49.0 MB (49012977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa67452e329e71787509a1583923b8e1e83b22a2fb76e48111393a03205d4c20`  
		Last Modified: Tue, 25 Oct 2022 02:50:30 GMT  
		Size: 8.7 MB (8738304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7be163526b121ed701b3595b33b6d8755aba04a12b0fd801f9c899cbd3ebd0`  
		Last Modified: Tue, 25 Oct 2022 02:50:30 GMT  
		Size: 11.0 MB (11041665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:unstable-scm`

```console
$ docker pull buildpack-deps@sha256:b50c4e396c237f001ad110bae4dc336d4385072144bbcc70545e1aac7afc164e
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
$ docker pull buildpack-deps@sha256:25c732971a707c1aa513e89ebe69d3167742941a1926860949186f4665a61e90
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131420075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f4ee86a7ab5c87f3ca76cf99bb43f859974dcabaee4095c54ee36e61f14f963`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:27:32 GMT
ADD file:b2f29ff1f75077ccce680becaa7bffdc9dfb9c7938188e93673e1b42bf418630 in / 
# Tue, 04 Oct 2022 23:27:32 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:58:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:59:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:59:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a9fedee3000f9dcc2b77410cd53420ec321135a3f7a6c688b43f31e503042e1e`  
		Last Modified: Tue, 04 Oct 2022 23:32:34 GMT  
		Size: 52.7 MB (52684279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dda17d2d1d2961ba6c7083d3013dde5fb5af68bd80ee1e40adbf7886b64df3c`  
		Last Modified: Wed, 05 Oct 2022 01:21:27 GMT  
		Size: 9.3 MB (9300772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809d617f2e2db52d55fec066a28a409d69e1dc40dd9f91f7f03c19ec8d16c587`  
		Last Modified: Wed, 05 Oct 2022 01:21:27 GMT  
		Size: 11.4 MB (11382118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15dd69568329cc8f49552e84cc7a6c0a0c112efb493830d52d7c1c6ed88af8f`  
		Last Modified: Wed, 05 Oct 2022 01:21:45 GMT  
		Size: 58.1 MB (58052906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:a8b12521cd98493a261a1f55e4e49770685b571e6386be3381e830a332b0fb77
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.5 MB (124504941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71f6828f20558d795c5704b92e9a7aa0d14089cfce9c332cbeddd096e880fb9e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:06:50 GMT
ADD file:829f8e96e527611e85aa710b19c01c75a4760a27c651fb439f8cdb5609db64aa in / 
# Tue, 25 Oct 2022 03:06:52 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:14:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:14:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:15:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:513ea4862e78a8cc07ed6d320f10e746ca770eb039dec1548c31a9de19d1f7ce`  
		Last Modified: Tue, 25 Oct 2022 03:12:19 GMT  
		Size: 49.6 MB (49578888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1ace4b71d48c3105e8f55674a41898f6b1df73d7ee8b05d5c3d3b3fea66077`  
		Last Modified: Tue, 25 Oct 2022 06:20:29 GMT  
		Size: 8.5 MB (8548544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:428ee02803cd3666baa3051b15b273e86d1d20710ddd79191fb1367a0dda5edc`  
		Last Modified: Tue, 25 Oct 2022 06:20:29 GMT  
		Size: 10.8 MB (10829764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecfb58f8aebfa286f964add0eb9b5f5bf243c4e6b5c934809df2c000acf0301c`  
		Last Modified: Tue, 25 Oct 2022 06:20:53 GMT  
		Size: 55.5 MB (55547745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:40c9e410a265ce99ab8112cf900f9fa0daef54cf9234ad867c88266563924307
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122227727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d951a42d8333c4774860fbaa9e0b184cb41f258db3b954eb1f6cbfae9610cf4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:00:01 GMT
ADD file:41046e966f37a45410c2aa02920b78f877f5aacb6ee087b2c6c6642f4e7b474f in / 
# Wed, 05 Oct 2022 00:00:02 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:38:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:38:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:38:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1316bf5b10f256f27feadcb25edef6365e912773e60cc382610ef003daf37248`  
		Last Modified: Wed, 05 Oct 2022 00:07:10 GMT  
		Size: 49.4 MB (49436823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00270159c4caaec159e25e1eaca6209b11c838dd60b5e0f5194e2279c51cd70`  
		Last Modified: Wed, 05 Oct 2022 00:56:26 GMT  
		Size: 8.4 MB (8399366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8524fd9b0e923155334b98a655b41aa941eb210e3248b7cc375ee49257b2b929`  
		Last Modified: Wed, 05 Oct 2022 00:56:26 GMT  
		Size: 10.7 MB (10663790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92867f6312a37ef5d4d5b38b1944bbe65123c5127a3ace08db615300dfc442c7`  
		Last Modified: Wed, 05 Oct 2022 00:56:52 GMT  
		Size: 53.7 MB (53727748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:009fc52c030c01267bd65a2028550fb986ff9a24369ae3d7ef56602a860c7962
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128431668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:401058bc5bd559766e08995d18ca3833502c6c103700576f37a012f933754edf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:29 GMT
ADD file:6a2d69a5a731490271c915d99634a89755f7236ef56712924ea061730d8552c4 in / 
# Tue, 25 Oct 2022 05:46:30 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:01:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:01:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:02:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:63a396bb133ce57141398b6c6d776ce17e3e973085b5a1b746d76407240a376a`  
		Last Modified: Tue, 25 Oct 2022 05:50:38 GMT  
		Size: 50.6 MB (50643735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a89cf1bf3c8da06b08672e8551d2511df312e843fb3acab24e31d9ba0afa866`  
		Last Modified: Tue, 25 Oct 2022 08:32:19 GMT  
		Size: 8.9 MB (8932959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e653e6dd7e514d68792b5ac0d2812dbc50a0e1d5c4842fd356c767031c54aec`  
		Last Modified: Tue, 25 Oct 2022 08:32:19 GMT  
		Size: 11.1 MB (11138995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c34d6a76d061ba3fc92256f8a3d68cb9c3d5840430072a886deb01b71229ceba`  
		Last Modified: Tue, 25 Oct 2022 08:32:40 GMT  
		Size: 57.7 MB (57715979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:727397e319709783655de941e122470c8e5580ec96e62fbc532fce0166e10ea4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131761295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbf8113ad39378aabee953d3468724d3c1eb3ab375b04cb1942f60a917ec3e0f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:23:38 GMT
ADD file:80dabb60a37b1d88f3750adb85c9e159d00b55293f70ad93512f94bd3cfd99bc in / 
# Tue, 25 Oct 2022 02:23:39 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:18:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:18:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 05:19:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:367799113badd94b9683087d6086436649a1fb7127698c42b0d730f5bbedcf86`  
		Last Modified: Tue, 25 Oct 2022 02:30:22 GMT  
		Size: 51.6 MB (51625321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564d2fccc59969c0b37e3bb8384bc6545a4cce125daa11c7e8b599ec0acac788`  
		Last Modified: Tue, 25 Oct 2022 05:30:00 GMT  
		Size: 9.3 MB (9282393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09be9213196e288bdcccf553107591d6fe4f04fccea4da55faea35dd79cfff15`  
		Last Modified: Tue, 25 Oct 2022 05:30:00 GMT  
		Size: 11.4 MB (11379737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7cf8ff2ca1128a94c435416195c01bd46e7b32191a4a225527692f374d4e31e`  
		Last Modified: Tue, 25 Oct 2022 05:30:21 GMT  
		Size: 59.5 MB (59473844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:c9c05846a233f3706bbd7659030113b2c11cb85bcbc85f0b7b52ceb249609d45
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.4 MB (129353653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33fe28a49a8569202e6d59224f55c96afa8a526b2d020c759bf8a9e89b40f50f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:11:00 GMT
ADD file:a7d6f7226093388fbc662c6e3fa1bc8dc263ab630fe03ea088486e6b016474ff in / 
# Wed, 05 Oct 2022 00:11:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:20:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:21:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:22:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3110bff10f823ecdaa06d8f7c65ce83d7c99521680207da9d264aaa8823d5209`  
		Last Modified: Wed, 05 Oct 2022 00:19:21 GMT  
		Size: 52.7 MB (52669988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6422d53934b53541883e4d8479c0384974a4f8c2ca335b2e86b900b4cf761d7d`  
		Last Modified: Wed, 05 Oct 2022 01:35:18 GMT  
		Size: 8.7 MB (8665467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2fd86c88bcf963ae10ae57261059a1b2bdbad2590061f63513acf0308dacf1`  
		Last Modified: Wed, 05 Oct 2022 01:35:18 GMT  
		Size: 11.1 MB (11130537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408a6f9d0ef9c4902e1584d5a5ac4ed8e9e71594c69a06143ca94a9b42bfc026`  
		Last Modified: Wed, 05 Oct 2022 01:36:07 GMT  
		Size: 56.9 MB (56887661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:b752fc221f409b6cdab8b2847838e201ce3d7c95856590870fa67391d109b85c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.0 MB (139006341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6da31aa88a012fc286c9e83bfe13f29518d53fa4afd44a2356ddc53ddc827f65`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:14:07 GMT
ADD file:6e9efd6bb77c835520332c88cb412f38f0d8573ec3347b090b77965e17131780 in / 
# Tue, 25 Oct 2022 03:14:10 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:17:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:17:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:17:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a3962f6ac5b86fa159789ea1e9241ecbb956b3223e8312f7d92d7fbb8bf5485`  
		Last Modified: Tue, 25 Oct 2022 03:20:03 GMT  
		Size: 54.7 MB (54704717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c5225e6c97e35e08afc065bed0fb4156a1727da9a3e12b4a611189682c919a`  
		Last Modified: Tue, 25 Oct 2022 06:50:49 GMT  
		Size: 9.7 MB (9684744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39fe7c3b495d9320ca99478bfddf7a3fa0412a37c56ca95a4cc891ceb738e62`  
		Last Modified: Tue, 25 Oct 2022 06:50:49 GMT  
		Size: 11.9 MB (11937807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9270b45cd7087efea37438ff9651d0078e51c8b476b199cfc26770079313e3`  
		Last Modified: Tue, 25 Oct 2022 06:51:17 GMT  
		Size: 62.7 MB (62679073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:80fe5d929462fbcb8fb502564ba1c94f3a1fb305aff0e201341b695be50f3fd5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.0 MB (122015209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3095c5914c0792da561d083de7026417fc5bec6e01a866d86b2f8f8d796eac27`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:39:40 GMT
ADD file:cff1e1a432929527e9bb64bde53e2b614c941bd4631b7bd3634fdda8a7240455 in / 
# Wed, 05 Oct 2022 00:39:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:26:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:27:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 02:31:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9cc6da93595cf4d9d589de999765cc4f1efa5e0d8e23ca6dd8b73b18afdc8189`  
		Last Modified: Wed, 05 Oct 2022 00:57:59 GMT  
		Size: 48.9 MB (48857821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554ce58712f86101a4716baede25ee43c9c1fc550b39fb4b3e5fa1622fd3b00b`  
		Last Modified: Wed, 05 Oct 2022 03:30:22 GMT  
		Size: 8.4 MB (8388012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd132871253f925889ef836099addcf830644843a64a1529bddc510390846a9b`  
		Last Modified: Wed, 05 Oct 2022 03:30:22 GMT  
		Size: 10.8 MB (10750715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bfc76b3f6f1ba447e697e6e2190cf70e757458cce81446b79426ae4cccdb03`  
		Last Modified: Wed, 05 Oct 2022 03:33:00 GMT  
		Size: 54.0 MB (54018661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:4030ace049550e7266628c08a838e0658e705dad4f0491dac2535698df26107b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125732836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78d8337e348ae8954f28173bf3c8248b38c98bf8c64e684b15d1dc50a21089c7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:14:54 GMT
ADD file:7dba2ae439c9f5da3fe962e867cee94eafc0b12a74939e13fdf987965ef8191c in / 
# Tue, 25 Oct 2022 01:14:57 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:32:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:32:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 02:33:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1430653806baea9ab2928a0d226c10ba8e7bf4b9b93398f9082ba16edfb2d4b8`  
		Last Modified: Tue, 25 Oct 2022 01:19:17 GMT  
		Size: 49.0 MB (49012977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa67452e329e71787509a1583923b8e1e83b22a2fb76e48111393a03205d4c20`  
		Last Modified: Tue, 25 Oct 2022 02:50:30 GMT  
		Size: 8.7 MB (8738304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7be163526b121ed701b3595b33b6d8755aba04a12b0fd801f9c899cbd3ebd0`  
		Last Modified: Tue, 25 Oct 2022 02:50:30 GMT  
		Size: 11.0 MB (11041665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ea6534b4c7c78beb071314cf02af39dc48f27dffa56b6182c538fc47d868d4`  
		Last Modified: Tue, 25 Oct 2022 02:50:45 GMT  
		Size: 56.9 MB (56939890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:xenial`

```console
$ docker pull buildpack-deps@sha256:9f3239283e1eb80449f823d8e18a8a94b2e766adaa92a29b9f2f48b964674dd5
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
$ docker pull buildpack-deps@sha256:a76fa2851a818bd9e17282587a14ab6a70f87bc50ad71aa4194dd68193d0c5e3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.1 MB (210145871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:150729efc1f801b3c41dad5c9402bedd2cc631f5f40eae14367bd776664701b4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:55:17 GMT
ADD file:3c6dc937cb7b4c81b42126f377d23320ec1d0a8ca34d38e7c45871f1d08dac43 in / 
# Tue, 25 Oct 2022 05:55:18 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 25 Oct 2022 05:55:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:55:19 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 25 Oct 2022 05:55:19 GMT
CMD ["/bin/bash"]
# Tue, 25 Oct 2022 08:24:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:24:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:24:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:28:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:828b35a09f0b2f3d1dead43aa2468ff5eba6c463423b3fff7ee6d150f6fd1b6b`  
		Last Modified: Thu, 05 Aug 2021 00:25:09 GMT  
		Size: 41.2 MB (41239253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66927c6d1d3d2e9321c4893f7f2105b7cd23dfb082853d97ec08f188e271e612`  
		Last Modified: Tue, 25 Oct 2022 05:57:02 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000560be91651dcbf476ebacb8bf1f1339694a3327f8e6da2519e0b29b33eb5d`  
		Last Modified: Tue, 25 Oct 2022 05:57:02 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6225a0253717abdc2ee23ea211c1c439c93b84231ec0a4f1c74762a205ba7234`  
		Last Modified: Tue, 25 Oct 2022 05:57:02 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e6d65f936039d0e2af7dd447344ff1a4f3d1987e1cf2628011285c9492be94`  
		Last Modified: Tue, 25 Oct 2022 08:36:56 GMT  
		Size: 6.8 MB (6838703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5c22d5e41e5c25f365fc9199c3648c8fe1b7819614ce763b3dbc00fa6e0242`  
		Last Modified: Tue, 25 Oct 2022 08:37:11 GMT  
		Size: 39.8 MB (39808282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0bcb2fc5c488536f3c7fb6acf7cfdf7815783a88e34de08f2e3ab3b05a7a9a`  
		Last Modified: Tue, 25 Oct 2022 08:37:34 GMT  
		Size: 122.3 MB (122258127 bytes)  
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
$ docker pull buildpack-deps@sha256:1f96d9808e87659130e067e8dd0f04514541dcf5ba5f26c01f361595bec5eb39
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
$ docker pull buildpack-deps@sha256:9729b711e909d53c0dcac87e152741034c35987034110ec2df03fef0c182419c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48079462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:950208a6f6157f0c26f5634bd58c369a0072c83b7f568b430e84c66224f18dbe`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:55:17 GMT
ADD file:3c6dc937cb7b4c81b42126f377d23320ec1d0a8ca34d38e7c45871f1d08dac43 in / 
# Tue, 25 Oct 2022 05:55:18 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 25 Oct 2022 05:55:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:55:19 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 25 Oct 2022 05:55:19 GMT
CMD ["/bin/bash"]
# Tue, 25 Oct 2022 08:24:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:24:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:828b35a09f0b2f3d1dead43aa2468ff5eba6c463423b3fff7ee6d150f6fd1b6b`  
		Last Modified: Thu, 05 Aug 2021 00:25:09 GMT  
		Size: 41.2 MB (41239253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66927c6d1d3d2e9321c4893f7f2105b7cd23dfb082853d97ec08f188e271e612`  
		Last Modified: Tue, 25 Oct 2022 05:57:02 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000560be91651dcbf476ebacb8bf1f1339694a3327f8e6da2519e0b29b33eb5d`  
		Last Modified: Tue, 25 Oct 2022 05:57:02 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6225a0253717abdc2ee23ea211c1c439c93b84231ec0a4f1c74762a205ba7234`  
		Last Modified: Tue, 25 Oct 2022 05:57:02 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e6d65f936039d0e2af7dd447344ff1a4f3d1987e1cf2628011285c9492be94`  
		Last Modified: Tue, 25 Oct 2022 08:36:56 GMT  
		Size: 6.8 MB (6838703 bytes)  
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
$ docker pull buildpack-deps@sha256:03039fe25cc2845bf8e249b2eca46ae5937e884ddabb6548d8f1cb296f2e5b17
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
$ docker pull buildpack-deps@sha256:d02144ab71a36dd5357661276ef23395a32022382a53294d6681cfd442327547
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.9 MB (87887744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:067fd097536acda8a5a5cc26b969443e4a156dc464664ce5692a72466ca48caa`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:55:17 GMT
ADD file:3c6dc937cb7b4c81b42126f377d23320ec1d0a8ca34d38e7c45871f1d08dac43 in / 
# Tue, 25 Oct 2022 05:55:18 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 25 Oct 2022 05:55:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:55:19 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 25 Oct 2022 05:55:19 GMT
CMD ["/bin/bash"]
# Tue, 25 Oct 2022 08:24:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:24:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:24:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:828b35a09f0b2f3d1dead43aa2468ff5eba6c463423b3fff7ee6d150f6fd1b6b`  
		Last Modified: Thu, 05 Aug 2021 00:25:09 GMT  
		Size: 41.2 MB (41239253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66927c6d1d3d2e9321c4893f7f2105b7cd23dfb082853d97ec08f188e271e612`  
		Last Modified: Tue, 25 Oct 2022 05:57:02 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000560be91651dcbf476ebacb8bf1f1339694a3327f8e6da2519e0b29b33eb5d`  
		Last Modified: Tue, 25 Oct 2022 05:57:02 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6225a0253717abdc2ee23ea211c1c439c93b84231ec0a4f1c74762a205ba7234`  
		Last Modified: Tue, 25 Oct 2022 05:57:02 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e6d65f936039d0e2af7dd447344ff1a4f3d1987e1cf2628011285c9492be94`  
		Last Modified: Tue, 25 Oct 2022 08:36:56 GMT  
		Size: 6.8 MB (6838703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5c22d5e41e5c25f365fc9199c3648c8fe1b7819614ce763b3dbc00fa6e0242`  
		Last Modified: Tue, 25 Oct 2022 08:37:11 GMT  
		Size: 39.8 MB (39808282 bytes)  
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
