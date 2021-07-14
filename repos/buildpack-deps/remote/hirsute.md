## `buildpack-deps:hirsute`

```console
$ docker pull buildpack-deps@sha256:09e533aa9c95bb4200168f7feb27d2617ec143418039e7a7660c9f43b72044e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:hirsute` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:e7448dbfc2b43f4b3ede1a56972a62d056fcf1573f0cf196c23c2501b8aa908a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.0 MB (248951992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bbef891892574ce6dae5882c03d6d8bfc338e8da195e57b46e40805eb5cacfa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:57 GMT
ADD file:af305d3eb867f312743f97d1cbed14ee2a155fdfed4621c72a8e8cf25355660c in / 
# Tue, 13 Jul 2021 22:29:57 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:35:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:36:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Jul 2021 23:36:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:39:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:966b3c5c8637e41360eed39a59e6c16ee1e986f7f2b92244e4d39f7ca6669618`  
		Last Modified: Tue, 13 Jul 2021 22:31:57 GMT  
		Size: 31.8 MB (31836858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a04a01c24f99b40c331ead5fe266437c7e8f9792a150da4220010982073489`  
		Last Modified: Tue, 13 Jul 2021 23:47:46 GMT  
		Size: 5.4 MB (5431774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daefe3fcd90dbd594dc34d343456aba2e06f2154410b341785c870c71e553a7b`  
		Last Modified: Tue, 13 Jul 2021 23:47:46 GMT  
		Size: 3.7 MB (3662500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329d33d59d172b4978b80b2e8d6f049588732133e6a0516009f864a5b89154fc`  
		Last Modified: Tue, 13 Jul 2021 23:48:05 GMT  
		Size: 43.5 MB (43540964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b012841d013b92fa76d156145963cc1d0f6c15e7dccb69673cfbf683d602b5`  
		Last Modified: Tue, 13 Jul 2021 23:48:39 GMT  
		Size: 164.5 MB (164479896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:c7b154aab3b9bbf6a4bfe375185e07dbe1225ccd15e1588150d71a80167bd50d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.9 MB (208948831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:762fa2f5c87c13b469b5d49942f746d519dc818a2c71cc8b26154874a6fda5e7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:21:58 GMT
ADD file:5175798ab209bbc3941a05787751ecf9e7ba0b4e9cda31b044bd6d75e25976c8 in / 
# Tue, 13 Jul 2021 23:21:59 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:58:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:59:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 14 Jul 2021 01:59:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:01:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fb746c2c12b45d26860f880a6e953018e4e9b83f9de17d11528fa484e1eb0f9f`  
		Last Modified: Tue, 13 Jul 2021 23:27:31 GMT  
		Size: 26.9 MB (26853751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eece18331508c76042ad235a876e23b49181f5ec1a12bc249810a5c1054ecc4`  
		Last Modified: Wed, 14 Jul 2021 02:21:44 GMT  
		Size: 4.9 MB (4858455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ceee6719a049da986bf7137392215103a2329991689f89b7c21e4d6c154ea0`  
		Last Modified: Wed, 14 Jul 2021 02:21:42 GMT  
		Size: 3.1 MB (3138473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b42a764a798d56ca11ab0dd698ae53b182225ec31f170dcb1be9839ec6479ff6`  
		Last Modified: Wed, 14 Jul 2021 02:22:26 GMT  
		Size: 40.0 MB (39955901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:110ce402e9cdbf22f2355750f225f7c91542618660d1e70338803d0088a1dfb4`  
		Last Modified: Wed, 14 Jul 2021 02:24:01 GMT  
		Size: 134.1 MB (134142251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:23a59c7336d6052de69e1c26fa86e67dd2d33815f9a101e35e832817e9272170
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.7 MB (239733346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33b0518928ced6dc7a9310bcce968f04de467630956d418d904c8c8719d8d415`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:46 GMT
ADD file:9e964afafcec670390a354fe9412da078ea83c247037612ce2b4c00c025cb4f1 in / 
# Tue, 13 Jul 2021 23:01:46 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:54:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:54:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Jul 2021 23:55:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:56:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cfe8b2632f122e3d77487867f2d08211ff277e78f8cb07a44832e91dd7c09ad7`  
		Last Modified: Tue, 13 Jul 2021 23:04:18 GMT  
		Size: 30.3 MB (30297903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e729df8790411dd4b5d51402271f41ae54c66f21fab7d27a85128c28afbc1c86`  
		Last Modified: Wed, 14 Jul 2021 00:04:10 GMT  
		Size: 5.4 MB (5403289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4509723cca5717dcc263c340e8d2352f8f9c3473762a6f85c71a50891715ea65`  
		Last Modified: Wed, 14 Jul 2021 00:04:09 GMT  
		Size: 3.6 MB (3637990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aea3a51ab770ef91044f986297f719fa1640f81f67d75bc637f994f91464c96`  
		Last Modified: Wed, 14 Jul 2021 00:04:30 GMT  
		Size: 43.5 MB (43531440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57eefc69cafa2a93ba45703dfdc306286bdee7e694e668a6f1ec3ce4748f617a`  
		Last Modified: Wed, 14 Jul 2021 00:05:06 GMT  
		Size: 156.9 MB (156862724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:7a385bfb6ba57a89d52bed519ff574bbdf71c296c555c90ddb809169bf957353
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.9 MB (259859458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25fd543ec8d37dce9714fded2b19560f49144e701dc100b1d0d067d6f525bdb5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 21 Jan 2021 03:52:02 GMT
ADD file:3d7449eef944b930488986ed089606017a4392e5e8231031c80e680e31b4da77 in / 
# Thu, 21 Jan 2021 03:52:14 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:52:29 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:52:41 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:52:47 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 07:34:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 07:35:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 21 Jan 2021 07:37:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 07:46:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:55aebc4be35f4811f0c02de6f92178fd8f7b65e395e8cb03da193bac6fafea1d`  
		Last Modified: Thu, 21 Jan 2021 03:55:55 GMT  
		Size: 37.1 MB (37120027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf4a190c1c2a83741c3769bb3ad14038be64a619a04aa712f80ce3a1f5218e5`  
		Last Modified: Thu, 21 Jan 2021 03:55:47 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009631d025b1b2b9e034f9fd76ed1e632a0dc6f0aeec51263339007901b56748`  
		Last Modified: Thu, 21 Jan 2021 03:55:47 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c02946107bd138c77db9eab66487871adfba9c8b7b078d2990a469890389ec91`  
		Last Modified: Thu, 21 Jan 2021 08:10:57 GMT  
		Size: 6.1 MB (6054214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8cd4a6aa56af3abb812e969114f97e4dc21f400bccfa57cd61e6a36d310c99d`  
		Last Modified: Thu, 21 Jan 2021 08:10:56 GMT  
		Size: 4.8 MB (4827138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be0c8d3e6c904e1ab054ea36644f54cd5145a5631456649af11bbbaba489e5f`  
		Last Modified: Thu, 21 Jan 2021 08:11:24 GMT  
		Size: 50.0 MB (50044971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60d114b9d2196fed368ed8d5efaf038777f5a06e7d2e57f42e11576c91bd770`  
		Last Modified: Thu, 21 Jan 2021 08:12:13 GMT  
		Size: 161.8 MB (161812070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:c041431af7f4815bfe8b558604b08098918c96d53f6a06fb5512bcf45f9fd681
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.0 MB (238975398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d51b1646c8b1b700b9a46239a75ea97fd7a8c58ff017be117d628e48b49f2da`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 21 Jan 2021 04:02:00 GMT
ADD file:8ec30abb851d24263f13b8ab93a9889626368053d325848b2f951e43ccac9a0c in / 
# Thu, 21 Jan 2021 04:02:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 04:02:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 04:02:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 04:02:12 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:24:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:25:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 21 Jan 2021 05:25:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:27:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:35d604bd00566c6cbc331e49db9228af41b973581b365975622efcddfda24580`  
		Last Modified: Thu, 21 Jan 2021 04:04:14 GMT  
		Size: 32.5 MB (32534356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8645fe124321a0a9ceca773d8bd654c8edfb63087f69654dc33b005cd936031`  
		Last Modified: Thu, 21 Jan 2021 04:04:09 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:811acaaa59ef2c29c645ec90173a876498cec8129d2051e6826881ba068508fb`  
		Last Modified: Thu, 21 Jan 2021 04:04:09 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c0a035e1b4479247e30498cb38c95743838097221a8aafc70ede4da8e1b6bf`  
		Last Modified: Thu, 21 Jan 2021 05:34:30 GMT  
		Size: 5.7 MB (5691508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476bdd8305678676c465817a601000b79a702ef2feb7d9fc199dd171304f9712`  
		Last Modified: Thu, 21 Jan 2021 05:34:29 GMT  
		Size: 4.5 MB (4458912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9928f3c621a6ce2274dfc19b3cdbaa1fb5d4b0bb2c1e5b4e0a4bcd581247ff79`  
		Last Modified: Thu, 21 Jan 2021 05:34:47 GMT  
		Size: 48.1 MB (48063304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b179abe761eab874adc03f48045f5c3c79df3d6dc064b208512374bf29789a`  
		Last Modified: Thu, 21 Jan 2021 05:35:18 GMT  
		Size: 148.2 MB (148226281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
