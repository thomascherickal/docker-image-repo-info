## `buildpack-deps:eoan`

```console
$ docker pull buildpack-deps@sha256:ff11515cf2f38b218c1e48e381b504c7d70bc677a3b9d603ad7ca6f7305dea3e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:eoan` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:ce4ef9de44e2d8da1cc44c3344adddc9be89f0b1d08ab6331c41d11c8c0b314d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.3 MB (234334353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffa03af468a67e5e2abb685fb7df26fe482c23995fef5bf9896f279c5295a40b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 20 Mar 2020 19:20:34 GMT
ADD file:537f9883fb90d19383082b8ac20c17b581db9045a48fa28b83cab73fe317047d in / 
# Fri, 20 Mar 2020 19:20:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:20:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:20:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:20:36 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:48:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:48:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 20 Mar 2020 19:49:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 01:26:06 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:eeacba527962683a1b026af611fe162d35281159762b699172caa48c69480f79`  
		Last Modified: Mon, 16 Mar 2020 15:44:17 GMT  
		Size: 28.3 MB (28276050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25405ed4f245fc5627d0b03996d04c11d492c7a9ff937f4562a18e8757c39434`  
		Last Modified: Fri, 20 Mar 2020 19:21:27 GMT  
		Size: 30.6 KB (30632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22752cd61bd53e9ac71e22fef539c165b3e11b368c1e54ca947260e317c4870a`  
		Last Modified: Fri, 20 Mar 2020 19:21:27 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9460de83957c509dd234ede9ea96d4d03b7f9cd252ef1497844f8450dedb6570`  
		Last Modified: Fri, 20 Mar 2020 19:21:27 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c42eb88f91904b1b4337337103ab96430c87f3ad2e37d3f822b84a655bd0809e`  
		Last Modified: Fri, 20 Mar 2020 19:57:01 GMT  
		Size: 6.5 MB (6512597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ff84c2324c65af66e83971227b34dc08eb47fa329d526af15e72ee7c2243b8`  
		Last Modified: Fri, 20 Mar 2020 19:57:00 GMT  
		Size: 3.5 MB (3517022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e64540e87545fd02991a47180c59c4082383009f57dd967e9be025e7b35265`  
		Last Modified: Fri, 20 Mar 2020 19:57:15 GMT  
		Size: 47.4 MB (47369722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d39ccc51f0e89f50cc6728f95581d93701fc805deddd8b6d140cb546f0d28e`  
		Last Modified: Tue, 21 Apr 2020 01:38:37 GMT  
		Size: 148.6 MB (148627323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:eoan` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:2217aa1f7c88e9ff00d29dd68389a46b25d024621fd227498ccdcc4a1a3e778c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.0 MB (202037249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f82d0628377ad5b1451a1132ca65bd5de8208122fe08faa2c326bd2207747ab`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 20 Mar 2020 18:58:53 GMT
ADD file:d5ea94843f1a1e0976b02f8e02c5256c148157dd51f492da5181ad8753622ab4 in / 
# Fri, 20 Mar 2020 18:58:56 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 18:58:57 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 18:58:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 18:58:59 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:21:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:21:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 20 Mar 2020 19:22:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 01:08:34 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2ea86edd9db57be0bd75bed151c49e031bd6699fcbd94130c3a8a8ab459692de`  
		Last Modified: Mon, 16 Mar 2020 15:44:38 GMT  
		Size: 23.7 MB (23735633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a6c62210e628371fc8ed38017e5360a6a15489b56acd8dba096dc79768da4ca`  
		Last Modified: Fri, 20 Mar 2020 19:00:28 GMT  
		Size: 30.6 KB (30613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8325644a644873d31f1108862c1ed632f57c3fbc43ebe7603f57c2c0d39a3665`  
		Last Modified: Fri, 20 Mar 2020 19:00:28 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c4a05bf433715cda695415ab43dfdcae3e89606057e6ab273703fa768f4a6d`  
		Last Modified: Fri, 20 Mar 2020 19:00:28 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5329b380082dac433270a0b1ad42ffe176511a6b4a4a7f6081c725d8a9772858`  
		Last Modified: Fri, 20 Mar 2020 19:26:53 GMT  
		Size: 5.5 MB (5532315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b02e6dbd45902d44e8810a3b6e246f1b3b62a3b0345c64c711bba978777b0d6`  
		Last Modified: Fri, 20 Mar 2020 19:26:53 GMT  
		Size: 3.0 MB (2982641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c21255b32720cb530bc823f976c6c1a1ef706e100533c555d5867b5bea5c38e7`  
		Last Modified: Fri, 20 Mar 2020 19:27:15 GMT  
		Size: 43.1 MB (43085491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44461ec0eedfff2a9cec3373d513c96ea7cec818875c387dcd1d13aa17db69e3`  
		Last Modified: Tue, 21 Apr 2020 01:25:08 GMT  
		Size: 126.7 MB (126669520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:eoan` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:1fa236c247ca527b46226d9e156e3da077164c2409203f520d437a022cec8d7a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.7 MB (229746933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:440bd0e3a902474cf981f1c2d86ee600e77dc3eb529d6c8a615835477a7b8f6b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 20 Mar 2020 18:43:59 GMT
ADD file:908424aa468cb2a7000dd795511259c67a0f70d0bbafa4b05b405faf89be8a02 in / 
# Fri, 20 Mar 2020 18:44:01 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 18:44:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 18:44:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 18:44:06 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:14:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:14:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 20 Mar 2020 19:14:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 01:50:46 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:20fe7914fb520387e59fda29e21ea64541bf9e7e95c9eef77a6ac68c18d23349`  
		Last Modified: Mon, 16 Mar 2020 15:44:48 GMT  
		Size: 26.9 MB (26869532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c6aa3850fcf8c6207823b79f1560303443a33d4fe996bf809b4dc7d00f7d35`  
		Last Modified: Fri, 20 Mar 2020 18:45:14 GMT  
		Size: 30.5 KB (30452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c02ac1bb4168bfb44e13693f63bd600c9230216a2443e5fb4839aedbb31635a2`  
		Last Modified: Fri, 20 Mar 2020 18:45:14 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be1b98aacf49712db6881b4d4da724b4349964afa1b6e6b4e983b7465c028513`  
		Last Modified: Fri, 20 Mar 2020 18:45:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87bce95c870b3e429de8b2891d6e9fd55ff65194bb2c98b4dd1517d810be1ed`  
		Last Modified: Fri, 20 Mar 2020 19:23:03 GMT  
		Size: 6.4 MB (6370756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420f2437c57580d01b2aecf81116f84e3120a5062815f6ea05b18bac2f74e9f8`  
		Last Modified: Fri, 20 Mar 2020 19:23:02 GMT  
		Size: 3.5 MB (3511455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2336f533fdfa48f41cac342e90a7b3458b135212c49b35dfb83911081c067a2`  
		Last Modified: Fri, 20 Mar 2020 19:23:23 GMT  
		Size: 47.4 MB (47380124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8931e7439e1cf6fc13db55317a97afbca159b8f100eb63df2ce27be0ddd6ff7`  
		Last Modified: Tue, 21 Apr 2020 02:06:58 GMT  
		Size: 145.6 MB (145583582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:eoan` - linux; 386

```console
$ docker pull buildpack-deps@sha256:f14d628eda1cef79e1962a07c4afb7873180a692e01131b49c55e0fdc9bf0d07
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.8 MB (238837440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24259785292c5001e6a72d04fa1724e83c8c1a10d7a56c3edfbea23deed666e5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 20 Mar 2020 18:39:08 GMT
ADD file:0e9faec03747f7230dbb61530a500027d8a504b2aa7edc19353d9d113a28b775 in / 
# Fri, 20 Mar 2020 18:39:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 18:39:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 18:39:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 18:39:11 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 18:59:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:00:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 20 Mar 2020 19:00:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 01:46:33 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7ec2907f7e8e2aa58e6e8544a4c009b751bc4ffb0260097338c8af14584c359e`  
		Last Modified: Mon, 16 Mar 2020 15:45:02 GMT  
		Size: 29.0 MB (29044614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6611c39bb98f10485e66c9de26f541ea83047ec3a7c7c375b08960b001e976f7`  
		Last Modified: Fri, 20 Mar 2020 18:39:45 GMT  
		Size: 30.7 KB (30688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925c05ba7d1067bfcebc90f78d1d37877173cccaab5663827e1e19a564ae9064`  
		Last Modified: Fri, 20 Mar 2020 18:39:44 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de9c38a779a8dbacc0c634c58a8e8abbcb85229eac1910ff6d3fa00081dda86`  
		Last Modified: Fri, 20 Mar 2020 18:39:44 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f7f723694def9380e68a617edcb019578a85bcabb11c1c8314bfdf72d567c5`  
		Last Modified: Fri, 20 Mar 2020 19:05:20 GMT  
		Size: 6.8 MB (6841242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797bf372b91800946efda9e04e576b23d1a182a772d6dd22c10bc1b560de9e42`  
		Last Modified: Fri, 20 Mar 2020 19:05:20 GMT  
		Size: 3.8 MB (3810307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6fa2deeb59229eefed23389b0d0873c063ed57652297f0f207d4f7fb5be8db`  
		Last Modified: Fri, 20 Mar 2020 19:05:38 GMT  
		Size: 49.0 MB (48962266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fdfea8c685e304f9324c68068aba2543286c91ba448ed3102de6f3ca293fcd`  
		Last Modified: Tue, 21 Apr 2020 02:00:01 GMT  
		Size: 150.1 MB (150147315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:eoan` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:a7e84911774a91a0273787f782be11bbc08399b5c2d4544ad111ec47d96961c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.1 MB (261082538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca228943610f8faf1fc45ccee3e5940f57f9464e694c8a837eebc11857baf627`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 20 Mar 2020 19:23:08 GMT
ADD file:5f2d0c54e4b302f16104b557b94863ea583b0f5077cdba4a739077166e742286 in / 
# Fri, 20 Mar 2020 19:23:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:23:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:23:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:23:31 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 20:26:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:26:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 20 Mar 2020 20:28:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:37:43 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ed545fde3a421d26f2fe47bd4ffaa6f5e4d1922ee226f849b9030af8e0469cb6`  
		Last Modified: Mon, 16 Mar 2020 15:46:10 GMT  
		Size: 33.0 MB (32986715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0dc90382a97787ce60215cad11117e850fe8c74a63cb5b8ce024645ea62b7a8`  
		Last Modified: Fri, 20 Mar 2020 19:25:21 GMT  
		Size: 30.5 KB (30494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c59e83ff7085e57aab1e4c48a50af629cf66f6ae0c896c7ca190d951b38b1f1`  
		Last Modified: Fri, 20 Mar 2020 19:25:21 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6ff0efafd163296380421cd94ed46d501335204734c716873fde2954ae4d84`  
		Last Modified: Fri, 20 Mar 2020 19:25:21 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2b12250d905cd2b3af1ed612fbcd1792c072d94aa5bb27f5ad3a94aed436c3`  
		Last Modified: Fri, 20 Mar 2020 20:53:06 GMT  
		Size: 7.4 MB (7420572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866515692221b069b60e0e16398694fe3e3ab0a294b549f3c6b3b55f4ffe0835`  
		Last Modified: Fri, 20 Mar 2020 20:53:07 GMT  
		Size: 4.5 MB (4463169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a677b781757c944bffbdae3549d724d76daeb7696b43ff3f7a00c10494732221`  
		Last Modified: Fri, 20 Mar 2020 20:53:29 GMT  
		Size: 54.8 MB (54780967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e8379bd5508d34fe4c81699ff1eefd6f8710b159f14a1ece6f0754f04b50e8`  
		Last Modified: Fri, 20 Mar 2020 20:54:14 GMT  
		Size: 161.4 MB (161399588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:eoan` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:74785bcaa4e08f39e42d162e9a2715f76f1c06fa984517119546636fdf7d620c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.8 MB (218751767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:390dbf03c7d4785ea53604c551a0faa6bdfe963b1e763b7008614aa8b4f67879`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 20 Mar 2020 18:42:18 GMT
ADD file:67b3704d37c528c5ff6a197ca57162dc6c474867b382ad39db7904ab7e226fc5 in / 
# Fri, 20 Mar 2020 18:42:20 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 18:42:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 18:42:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 18:42:22 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:32:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:32:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 20 Mar 2020 19:32:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 01:46:39 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0517329801b2de345bcce817664cf86ae07c4024192a4284158da43c3122a418`  
		Last Modified: Mon, 16 Mar 2020 15:46:11 GMT  
		Size: 26.7 MB (26682375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:511ae87888dfc4543789268e73d6a6615b85f3cf537675ca82cd56ccee47b8fd`  
		Last Modified: Fri, 20 Mar 2020 18:43:01 GMT  
		Size: 31.1 KB (31112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2492fa1c3c34d5a0666ea3189b225fbf28caa4aa29c30534274be8313a299c6a`  
		Last Modified: Fri, 20 Mar 2020 18:43:02 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad57e1baaa7aef9e2412ea570ae32f8973c10febade619f78326cd18c22eb6a`  
		Last Modified: Fri, 20 Mar 2020 18:43:06 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201e9590b4324aab4dfbd09eeab54089a6c9d7feb382d3a800ba7b871d578e5b`  
		Last Modified: Fri, 20 Mar 2020 19:36:46 GMT  
		Size: 6.1 MB (6139579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58616e43320d89facaf8f9003ae1495c9caff28193ed6c78f884ef4f56bda91`  
		Last Modified: Fri, 20 Mar 2020 19:36:51 GMT  
		Size: 3.4 MB (3433638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fdf262297fdf488fdfe610648a3a9c40a0250db5b60eff6e5bbb5df4aad4241`  
		Last Modified: Fri, 20 Mar 2020 19:37:02 GMT  
		Size: 47.0 MB (46964229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642afb280657f85dd229fbfe789945fed64c1731550835317bd455da4f52fb80`  
		Last Modified: Tue, 21 Apr 2020 01:53:36 GMT  
		Size: 135.5 MB (135499800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
