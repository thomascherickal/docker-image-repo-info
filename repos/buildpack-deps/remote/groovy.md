## `buildpack-deps:groovy`

```console
$ docker pull buildpack-deps@sha256:d7220e1ed842c854a708324ff142c69148cc9bacbeb2f9749fa06e5f3744b304
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:groovy` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:1b26a4b429ef514a90d3f1810deadd20034357ba8608370f6fb07e5b90bb78c5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.3 MB (239327735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9398fef452e91393be5a98b4b7daaa70cc39ce6a4c56f95421a04902d975e572`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:45 GMT
ADD file:8cda7bfcf6c3010f9498acf5db465d8affd86bacb786338974486e23ea62b05d in / 
# Fri, 24 Jul 2020 14:38:46 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:46 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:47 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:47 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:02:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:02:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 24 Jul 2020 15:02:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:04:33 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5f55bfaf77a136f7c6b5063e591480c2e7690ed1c29b0ee354caf8f6c62741e0`  
		Last Modified: Fri, 24 Jul 2020 14:39:44 GMT  
		Size: 28.4 MB (28357957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef373180da2631c7a56d9629e37de8010fe57414453617dde3a2c1e9861f1eb`  
		Last Modified: Fri, 24 Jul 2020 14:39:39 GMT  
		Size: 31.8 KB (31838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:675d10b513df5337d26a6e2ccaf4875267999084d7f0d2f3102c54d7430cfa35`  
		Last Modified: Fri, 24 Jul 2020 14:39:39 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552f92805e8c6585c466083ac60f40092ae127e794d498c599a31bd67df21c09`  
		Last Modified: Fri, 24 Jul 2020 14:39:39 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c003fe1ffd7eb86efa0bcd0d127f5dca3b2f9dcaa3ad54bdeaaf16602fff1a`  
		Last Modified: Fri, 24 Jul 2020 15:10:39 GMT  
		Size: 6.9 MB (6859149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3935824be9d9e08e1fe2b607c81e88e8128e36b84b36bdb20dfbc6a90fd43d96`  
		Last Modified: Fri, 24 Jul 2020 15:10:38 GMT  
		Size: 3.6 MB (3586137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:049526d25885d6dfb6c25aecefc91a85fc8ba6307755f335b42a72db89ea08bb`  
		Last Modified: Fri, 24 Jul 2020 15:10:58 GMT  
		Size: 62.2 MB (62168097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a2d9641745bd584145cd18a85952594b41ebad99d34eca0626597f491930f37`  
		Last Modified: Fri, 24 Jul 2020 15:11:29 GMT  
		Size: 138.3 MB (138323553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:bfd41ce761287f0d9dd8e6b0b346fc7c5ff5a8207c54172c96ba18a3403ba5a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **209.5 MB (209476479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7d5e35aec35acc77d28cce5e69f7984f68f88a50f9cb87d9c6aaa514ecaf5d2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 06 Jul 2020 20:08:43 GMT
ADD file:021612df98a3252c0018261734979dffe9cdc59bdd68707ae03cea58d0c65498 in / 
# Mon, 06 Jul 2020 20:08:48 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 23 Jul 2020 08:04:50 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 23 Jul 2020 08:04:54 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 23 Jul 2020 08:04:55 GMT
CMD ["/bin/bash"]
# Thu, 23 Jul 2020 08:12:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jul 2020 08:12:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jul 2020 08:13:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jul 2020 08:15:54 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:008c40b75c61a21ea627c86505f910d9a47056dc120ce6996c3d080b08658308`  
		Last Modified: Mon, 06 Jul 2020 15:50:47 GMT  
		Size: 23.8 MB (23846810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669074342c885ac270b199e748002596d0f32df7f77c659f5413f77f274cc91e`  
		Last Modified: Thu, 23 Jul 2020 08:05:45 GMT  
		Size: 31.9 KB (31856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca6860323f7121ae3ef42c0e5a729d9019a7d73fb9243d8a51943a2aa107c6b7`  
		Last Modified: Thu, 23 Jul 2020 08:05:45 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2afad5102492ecbe7ecd632b6fe604a800b86c249d9d2b3479b2da9647a22495`  
		Last Modified: Thu, 23 Jul 2020 08:05:44 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:468e38fb132bdeddfd36c0a893c4fb4814ed93c6e0c83eab5faeabf7deb892f6`  
		Last Modified: Thu, 23 Jul 2020 08:18:31 GMT  
		Size: 6.2 MB (6191330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242b21b142e64cc1983d3d7e88a1255886de1d1c5c746eafc0b392be36a3aec8`  
		Last Modified: Thu, 23 Jul 2020 08:18:30 GMT  
		Size: 3.1 MB (3059236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63baa8602234f81fc6fe662b71785f7dcb8823c03010b994bd64875e1cc981ae`  
		Last Modified: Thu, 23 Jul 2020 08:18:56 GMT  
		Size: 56.7 MB (56657419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7042925ae5bab285f2f4eb101ef739018771dc6ffca1b7f096b34528836fea19`  
		Last Modified: Thu, 23 Jul 2020 08:19:40 GMT  
		Size: 119.7 MB (119688792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:47d4e783d535f4c39f9322a2d01a81eb0ef6eac067f432962478797d8ca4b980
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.1 MB (229134703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eda713f7df55533f632a231a691136625e8c9ab35aeeeb90330ec918bd951776`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 06 Jul 2020 22:05:50 GMT
ADD file:35b0d977e8fc4305b3f988e3af2c52419e39aae68287af590636dfdb7487dbed in / 
# Mon, 06 Jul 2020 22:05:53 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 22:05:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 22:05:57 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 22:05:58 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 22:58:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 22:58:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 06 Jul 2020 22:59:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 23:01:34 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bca3f99199d9260076c548f38af71788f901900c99316e357c1dfb0e06fafbd6`  
		Last Modified: Mon, 06 Jul 2020 15:50:50 GMT  
		Size: 27.0 MB (26969246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf01b6284862c6caa2ce0e716ddb00705d21bb4f7cc4501c1fdf1130c17ffa7`  
		Last Modified: Mon, 06 Jul 2020 22:07:25 GMT  
		Size: 31.8 KB (31830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e991f38a848885cf9ff0e35cb51871c37ee33387f3159b4dbd1fa25146a3ecb`  
		Last Modified: Mon, 06 Jul 2020 22:07:26 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b128a6106c13f4424dcc44fef4eaa219acaf5f3c8510660e77bd90c81e6227`  
		Last Modified: Mon, 06 Jul 2020 22:07:25 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac980152f16f03da3b03b8a6b0804bce8a1c28151d843524b791230e868b1b14`  
		Last Modified: Mon, 06 Jul 2020 23:08:19 GMT  
		Size: 6.7 MB (6722628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d85f32459c314182a20d3c5effc3b5a3e1d981ed5cc5a38d6d9d1a22a68642`  
		Last Modified: Mon, 06 Jul 2020 23:08:19 GMT  
		Size: 3.6 MB (3570275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6337ecac2f2b8ff3b2253c1e677ba4d09ec9d9f8abf72bcff4ef2fffba92c328`  
		Last Modified: Mon, 06 Jul 2020 23:08:43 GMT  
		Size: 62.1 MB (62061790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c202624c81de0d6fe70667520207a76e7da104817e914e513ff38d07984448`  
		Last Modified: Mon, 06 Jul 2020 23:09:24 GMT  
		Size: 129.8 MB (129777899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:7f657a1d34ecf2911f50f075fbec77f968ec55d651013fdc867ba3306048974a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.1 MB (263102808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:090c92f9714b8d2eea447fd0e44972206410cda8a5b731c1d9f6b946020754d2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 06 Jul 2020 22:14:37 GMT
ADD file:4ce6882e512c279031700803ff45277278a6abe7c6418f436c85e0d066943302 in / 
# Mon, 06 Jul 2020 22:14:50 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 22:15:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 22:15:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 22:15:38 GMT
CMD ["/bin/bash"]
# Tue, 07 Jul 2020 01:36:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jul 2020 01:37:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 07 Jul 2020 01:43:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jul 2020 01:57:19 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:de300362f1d644150544eb1523eefb5eb9d2d3fdf58be3aec349a0d3b02f33f9`  
		Last Modified: Mon, 06 Jul 2020 15:51:24 GMT  
		Size: 33.0 MB (32959640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9c67b569feeae3f4167718dcc98be6f8ea149d7547a436363b4ddb15570933`  
		Last Modified: Mon, 06 Jul 2020 22:18:47 GMT  
		Size: 31.6 KB (31635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f7a367e520abe796341a0391780c5d1d14df2dea9ac76d1b4c0cdc833062895`  
		Last Modified: Mon, 06 Jul 2020 22:18:47 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb6403ad0c2a89150f64679cb5bfe40a7f419582465b2b0cb91bbf6ca57844e`  
		Last Modified: Mon, 06 Jul 2020 22:18:47 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c11aa7997c34fac81ac44f0c030234ad75bac101bcdecb109b91e6171573ffe9`  
		Last Modified: Tue, 07 Jul 2020 02:23:51 GMT  
		Size: 7.8 MB (7812080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b56ea8d11e73fdab9482db3280b468c6014292335626ff160428d238325761d2`  
		Last Modified: Tue, 07 Jul 2020 02:23:51 GMT  
		Size: 4.4 MB (4447733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0349f72d4b39705bdd866d28287fc7104b9f5a6f51ff87ed935dc7fb378f7b`  
		Last Modified: Tue, 07 Jul 2020 02:24:23 GMT  
		Size: 71.2 MB (71249849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a85db8280aa5afb730265a8c9c74c067117f6eb0e96f782e65975e2c1c2307`  
		Last Modified: Tue, 07 Jul 2020 02:25:09 GMT  
		Size: 146.6 MB (146600836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:70c80f979bea0c42a5a395fd0666a5591dfd363b270daa582320e9609cbf64c0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.9 MB (224899867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7131b98daf8dfa9f1ffec4b85356f0002ef6490f769bef8856c1fb14a66864cb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 06 Jul 2020 20:20:33 GMT
ADD file:7c5297f390515aab00f66f663182cadbb3c5dbf52fb015526b80806df21de69d in / 
# Mon, 06 Jul 2020 20:20:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 20:20:36 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 20:20:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 20:20:37 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 20:46:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 20:46:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 06 Jul 2020 20:46:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 20:47:22 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3c5e60e47f65a4306c7d2ad46d35b9ea6d4aaf9cb77add2bff5be52a742d23e4`  
		Last Modified: Mon, 06 Jul 2020 15:52:10 GMT  
		Size: 27.2 MB (27174117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6ddf166e3f11601f2466edd2cfbfe9942c0f85314ffb2ea31f66bb6d0cf123`  
		Last Modified: Mon, 06 Jul 2020 20:21:35 GMT  
		Size: 32.5 KB (32456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076f8572b34a88b603a66fc9eba9b5237c09e64670ac0d8a02e024d6e3ade52f`  
		Last Modified: Mon, 06 Jul 2020 20:21:35 GMT  
		Size: 840.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f928d1948ab604aafd2985aaa9196351c03043dee8e4bbbd73f4cbf190abb675`  
		Last Modified: Mon, 06 Jul 2020 20:21:41 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11eec02dfd95f6d6df751544a08b98b891c24c0ad561386ffd22b32592094376`  
		Last Modified: Mon, 06 Jul 2020 20:51:12 GMT  
		Size: 6.5 MB (6545554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a9f1cd556b3c6d476e9540bdaec30b426c7e295beb757e67cbbb2a3bcfc3ca`  
		Last Modified: Mon, 06 Jul 2020 20:51:17 GMT  
		Size: 3.6 MB (3579909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4fdf7b85c7ed6238d1f8fd569fe19a41f284dcbd0bafb9e99a4684406a54758`  
		Last Modified: Mon, 06 Jul 2020 20:51:31 GMT  
		Size: 61.7 MB (61698287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:861bea8a31a801c4e52eba162f62e1189bb4b78c659c58845376ac47ab4d7811`  
		Last Modified: Mon, 06 Jul 2020 20:51:53 GMT  
		Size: 125.9 MB (125868516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
