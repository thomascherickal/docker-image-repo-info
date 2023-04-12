## `perl:stable`

```console
$ docker pull perl@sha256:37ea7db4398365a45cec5917a73de8c7df68d859be3d865a49c7f552f771ac26
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

### `perl:stable` - linux; amd64

```console
$ docker pull perl@sha256:0859f242d4a63c53e0238ad1d14172ca0d83a06e0c721df07a1b8708da75ea23
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.7 MB (337716345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ced9209e0e62a48cfc7b335e91c034edfb2ad076cf34408ceac82be39147a21`
-	Default Command: `["perl5.36.0","-de0"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:15 GMT
ADD file:459d1e92eb8c24ff4758f974d289ca8a2abe04cf50b6fe2bd760aa4589478289 in / 
# Thu, 23 Mar 2023 01:30:15 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:01:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:01:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 06:01:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:02:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 11:10:48 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 23 Mar 2023 11:10:48 GMT
WORKDIR /usr/src/perl
# Thu, 23 Mar 2023 11:16:00 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.0.tar.xz -o perl-5.36.0.tar.xz     && echo '0f386dccbee8e26286404b2cca144e1005be65477979beb9b1ba272d4819bcf0 *perl-5.36.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.0.tar.xz -C /usr/src/perl     && rm perl-5.36.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Thu, 23 Mar 2023 11:16:01 GMT
WORKDIR /
# Thu, 23 Mar 2023 11:16:01 GMT
CMD ["perl5.36.0" "-de0"]
```

-	Layers:
	-	`sha256:3e440a7045683e27f8e2fa04000e0e078d8dfac0c971358ae0f8c65c13321c8e`  
		Last Modified: Thu, 23 Mar 2023 01:34:00 GMT  
		Size: 55.0 MB (55045608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a71c865a2c34678c6dea55e4b0928f751ee3c0ca91cace6e4e0578c534d6cf`  
		Last Modified: Thu, 23 Mar 2023 06:08:01 GMT  
		Size: 5.2 MB (5166592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670730c27c2eacf07897a6e94fe55423ea50b884d9c28161a283bbbf064d1124`  
		Last Modified: Thu, 23 Mar 2023 06:08:02 GMT  
		Size: 10.9 MB (10876735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a7a2c95f0f8b221d776ccf35911b68eec2cf9414a44d216205a6f03e381d3d7`  
		Last Modified: Thu, 23 Mar 2023 06:08:19 GMT  
		Size: 54.6 MB (54583510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d627e120214bb28a729d4b54a0ecba4c4aeaf0295ca2d1f129480145fad2af6`  
		Last Modified: Thu, 23 Mar 2023 06:08:51 GMT  
		Size: 196.8 MB (196812279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79532c5c4ba5bf13cc967ad4b177c3d2f61cbe373b688851c51303d85784faf`  
		Last Modified: Thu, 23 Mar 2023 14:13:24 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eff4027c695dc6ead19144af4dbf8851b896649e6b4dfe5eaa5a18e46316e98`  
		Last Modified: Thu, 23 Mar 2023 14:13:27 GMT  
		Size: 15.2 MB (15231455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:stable` - linux; arm variant v5

```console
$ docker pull perl@sha256:3763ceeadae4b472166b2beddc9286630fbf142ff79a2d4796301996c9d3ddbb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.1 MB (310072507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ab21a2e46de1badd21d489fe557229843bb89d305e1271f63d4d1c3756bc47d`
-	Default Command: `["perl5.36.0","-de0"]`

```dockerfile
# Wed, 12 Apr 2023 00:48:34 GMT
ADD file:ae13a4cbeb20b92ec29dd7409de47a964fe373bdde2a4e8880b5a4d9dc64171e in / 
# Wed, 12 Apr 2023 00:48:35 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:15:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:15:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:16:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:17:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 02:30:30 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 12 Apr 2023 02:30:30 GMT
WORKDIR /usr/src/perl
# Wed, 12 Apr 2023 02:35:42 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.0.tar.xz -o perl-5.36.0.tar.xz     && echo '0f386dccbee8e26286404b2cca144e1005be65477979beb9b1ba272d4819bcf0 *perl-5.36.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.0.tar.xz -C /usr/src/perl     && rm perl-5.36.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Wed, 12 Apr 2023 02:35:42 GMT
WORKDIR /
# Wed, 12 Apr 2023 02:35:43 GMT
CMD ["perl5.36.0" "-de0"]
```

-	Layers:
	-	`sha256:86cb8d774eca43d428d6a35506c172ba62358d2d5ec90c886e3b38b297f93b20`  
		Last Modified: Wed, 12 Apr 2023 00:50:46 GMT  
		Size: 52.6 MB (52555175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49db155cdf8645f599affcbbbc75eb928b0a9d010c4ac54afcfa9d7e4fa85e0`  
		Last Modified: Wed, 12 Apr 2023 01:21:15 GMT  
		Size: 5.1 MB (5072827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8936087cbd048148575fda58348506149db80a2699e99ae2042086628c0e5a38`  
		Last Modified: Wed, 12 Apr 2023 01:21:16 GMT  
		Size: 10.6 MB (10573853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0bf11569c39ee4f3d8515112046a55f14f39e54c6f0ea26271033c090f77d2`  
		Last Modified: Wed, 12 Apr 2023 01:21:35 GMT  
		Size: 52.3 MB (52340617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622390f39404d88752f248bc2136a55baca97d5324d43689204df0157d284282`  
		Last Modified: Wed, 12 Apr 2023 01:22:13 GMT  
		Size: 175.0 MB (175009432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d6cbfa5ffa45390a5dfe039951ee6ee63fd08e11bcda62ae1c151c2195b1784`  
		Last Modified: Wed, 12 Apr 2023 04:08:26 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b69360ff49161ea1b356b9161a1ced31812be5f764e7d467d1f9def8728544`  
		Last Modified: Wed, 12 Apr 2023 04:08:30 GMT  
		Size: 14.5 MB (14520436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:stable` - linux; arm variant v7

```console
$ docker pull perl@sha256:0af1513e0dd49b2ae4550cf1f14ca0fa60429731271d3d9dbb42759a45e56c6a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.3 MB (297334457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdcbe3d79b52e7d473b98f808ce53404fc59451ebd74ed1fc0b773ff84cb25c1`
-	Default Command: `["perl5.36.0","-de0"]`

```dockerfile
# Thu, 23 Mar 2023 01:13:21 GMT
ADD file:fa1cbfdd44274e571cabd5ca7fafa08b17c6f497ecfca6368a9eec4d2527a364 in / 
# Thu, 23 Mar 2023 01:13:22 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:40:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:40:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 12:40:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:41:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 21:29:01 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 23 Mar 2023 21:29:01 GMT
WORKDIR /usr/src/perl
# Thu, 23 Mar 2023 21:34:08 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.0.tar.xz -o perl-5.36.0.tar.xz     && echo '0f386dccbee8e26286404b2cca144e1005be65477979beb9b1ba272d4819bcf0 *perl-5.36.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.0.tar.xz -C /usr/src/perl     && rm perl-5.36.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Thu, 23 Mar 2023 21:34:08 GMT
WORKDIR /
# Thu, 23 Mar 2023 21:34:08 GMT
CMD ["perl5.36.0" "-de0"]
```

-	Layers:
	-	`sha256:d50e868f9a626a3c456c0c52c3b013e87619bbac7798ac0c2acf2a2407303125`  
		Last Modified: Thu, 23 Mar 2023 01:33:00 GMT  
		Size: 50.2 MB (50211788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eca667140ff247fc759283fc9ff4cafbe304d1777ffc70e1bd593b63151c31a`  
		Last Modified: Thu, 23 Mar 2023 12:45:01 GMT  
		Size: 4.9 MB (4934357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1879c254431e9965afb23e55a148faffd29450a9218269f769be95d6e9673a93`  
		Last Modified: Thu, 23 Mar 2023 12:45:01 GMT  
		Size: 10.2 MB (10217859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64c4a1b9916f6da6f286835522f27f11a812694e5f878e87468d4c6b90b343e`  
		Last Modified: Thu, 23 Mar 2023 12:45:20 GMT  
		Size: 50.4 MB (50355514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5862d41b96b9b8c37267f9bb50226c9d63fc5a8df2310f511837355e187e090a`  
		Last Modified: Thu, 23 Mar 2023 12:45:51 GMT  
		Size: 167.3 MB (167288602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69da07bb16566472a948a7db5070305f87e3170382d59b566e62f9cce7365ca7`  
		Last Modified: Thu, 23 Mar 2023 22:13:34 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e2c998c3c1ae1ddad4c142caa45f68cc22d67d4c5681d555e203b5ab629b77`  
		Last Modified: Thu, 23 Mar 2023 22:13:38 GMT  
		Size: 14.3 MB (14326170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:stable` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:feb3484a5774e0f60e0a3fdd37d9504f362c4ed663891fd66ee493744f370b27
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.3 MB (329316068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96b0c699e40dec93c558d4dfbe8f421a134563b6044c00af37c0ff8f24931e4d`
-	Default Command: `["perl5.36.0","-de0"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:42 GMT
ADD file:dd3d4e5fe819950e7d01b44a29dbd790438cd722ba76198910e2597448ab0c6f in / 
# Wed, 12 Apr 2023 00:39:43 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:06:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:06:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:07:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:08:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 05:14:36 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 12 Apr 2023 05:14:36 GMT
WORKDIR /usr/src/perl
# Wed, 12 Apr 2023 05:22:16 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.0.tar.xz -o perl-5.36.0.tar.xz     && echo '0f386dccbee8e26286404b2cca144e1005be65477979beb9b1ba272d4819bcf0 *perl-5.36.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.0.tar.xz -C /usr/src/perl     && rm perl-5.36.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Wed, 12 Apr 2023 05:22:16 GMT
WORKDIR /
# Wed, 12 Apr 2023 05:22:16 GMT
CMD ["perl5.36.0" "-de0"]
```

-	Layers:
	-	`sha256:dc80b8cdbfd36cb20231d807a50d704945d1df4da8f6e23197ccfcb629970491`  
		Last Modified: Wed, 12 Apr 2023 00:42:14 GMT  
		Size: 53.7 MB (53705529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5884e7f2c8c61aa845de4902fc29639b58861ae6c2d80bafe82082c0456c0740`  
		Last Modified: Wed, 12 Apr 2023 01:13:17 GMT  
		Size: 5.2 MB (5152752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b792b01ed3c8dc1488cd8aac41ab7d49bb17f3fa22b2e6c846078cec81a1c00`  
		Last Modified: Wed, 12 Apr 2023 01:13:17 GMT  
		Size: 10.9 MB (10873655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f993d5b17f32f4b8a535c25e182e5d8412625beee450e513ca57036e8fdd6dc`  
		Last Modified: Wed, 12 Apr 2023 01:13:34 GMT  
		Size: 54.7 MB (54676038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26edf98ece5babdb6b65e76738cef2c2d05e7075161753d3ba95cd84480d211`  
		Last Modified: Wed, 12 Apr 2023 01:14:02 GMT  
		Size: 189.7 MB (189727693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112b1da5f49847f2fc66af6d7b4c5b27d56e496caf785da7a6276943053c8d01`  
		Last Modified: Wed, 12 Apr 2023 07:49:37 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c56770255055ecb35178862c4c37c8554b611645c3997da817fcc4e682ec7c9`  
		Last Modified: Wed, 12 Apr 2023 07:49:40 GMT  
		Size: 15.2 MB (15180234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:stable` - linux; 386

```console
$ docker pull perl@sha256:ea3bd9c0a9c56e46bfd375430ef96ecdbe7b16e0bfbdcc592c3392662f3b2e77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **342.9 MB (342949421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c36a99a2554543bce7b4c5daf4bd06a678879c1d3b2fff0af471f812446006e4`
-	Default Command: `["perl5.36.0","-de0"]`

```dockerfile
# Wed, 12 Apr 2023 00:38:51 GMT
ADD file:4da7e6af0782b21849e5f6385de3589ac5b8d81d173721f9990d32da754df2cb in / 
# Wed, 12 Apr 2023 00:38:51 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:05:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:05:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:06:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:07:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 10:25:24 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 12 Apr 2023 10:25:24 GMT
WORKDIR /usr/src/perl
# Wed, 12 Apr 2023 10:34:30 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.0.tar.xz -o perl-5.36.0.tar.xz     && echo '0f386dccbee8e26286404b2cca144e1005be65477979beb9b1ba272d4819bcf0 *perl-5.36.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.0.tar.xz -C /usr/src/perl     && rm perl-5.36.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Wed, 12 Apr 2023 10:34:30 GMT
WORKDIR /
# Wed, 12 Apr 2023 10:34:30 GMT
CMD ["perl5.36.0" "-de0"]
```

-	Layers:
	-	`sha256:b2bef40925391866903279768b0ae1e8233ef6a1aae64509a922f4aa96fe42a6`  
		Last Modified: Wed, 12 Apr 2023 00:42:19 GMT  
		Size: 56.0 MB (56032818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a37ccf9a5e34ba2345ce265a9a11c93ee254e1f3616dfd1c1deda6e2f7d614c8`  
		Last Modified: Wed, 12 Apr 2023 01:14:53 GMT  
		Size: 5.3 MB (5293626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4988d5e4328f031f6884a7351766aa8a2806c9cdca38d354477fc537eaa4911f`  
		Last Modified: Wed, 12 Apr 2023 01:14:54 GMT  
		Size: 11.2 MB (11249875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660a2befd486d43a308dd1561f57efeafe1f13defd6439d34aeb5efec783ee3d`  
		Last Modified: Wed, 12 Apr 2023 01:15:17 GMT  
		Size: 55.9 MB (55922746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f09985282f12d05c5724bcbb0481a94f66820112bafc34a1d990dfdf74a52fc`  
		Last Modified: Wed, 12 Apr 2023 01:16:02 GMT  
		Size: 199.7 MB (199724315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:521ea4b0c8f723a20ae5ca57d35ba4d20f0b53e343054101b0c2e6d97c0fd138`  
		Last Modified: Wed, 12 Apr 2023 15:33:32 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dea5528f6af43d0745c13a6c880d422bde12a79d07cd092720c806e68865cd9`  
		Last Modified: Wed, 12 Apr 2023 15:33:37 GMT  
		Size: 14.7 MB (14725874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:stable` - linux; mips64le

```console
$ docker pull perl@sha256:c9a4a9dca3142a79f3fa6e26d4096e9c28f745264fa55fcca0ed5c7f39916dc1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **315.5 MB (315532163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce2fd07e5f28ee9ce7f5995cd5afd6a75b298ada3d3c4e42bb64d8ba517a8f2d`
-	Default Command: `["perl5.36.0","-de0"]`

```dockerfile
# Thu, 23 Mar 2023 05:17:18 GMT
ADD file:2337efa705c8772705fa8519e513f4299e72c9eb63e3a68069778ca95a1511e6 in / 
# Thu, 23 Mar 2023 05:17:24 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:13:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:14:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 07:15:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:21:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:40:34 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 23 Mar 2023 07:40:39 GMT
WORKDIR /usr/src/perl
# Thu, 23 Mar 2023 08:03:18 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.0.tar.xz -o perl-5.36.0.tar.xz     && echo '0f386dccbee8e26286404b2cca144e1005be65477979beb9b1ba272d4819bcf0 *perl-5.36.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.0.tar.xz -C /usr/src/perl     && rm perl-5.36.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Thu, 23 Mar 2023 08:03:24 GMT
WORKDIR /
# Thu, 23 Mar 2023 08:03:30 GMT
CMD ["perl5.36.0" "-de0"]
```

-	Layers:
	-	`sha256:f3951ee58695b4d906b37f2d9a07e6158f66a7328d0c70445d9607cd8367ede0`  
		Last Modified: Thu, 23 Mar 2023 05:25:08 GMT  
		Size: 53.3 MB (53264720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f79f6951926609a68e21aee7e612375637f7c12703c62b028fd60a22e2d9bfd`  
		Last Modified: Thu, 23 Mar 2023 07:34:02 GMT  
		Size: 4.9 MB (4922133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119b6297024241cbdae60b7afa1bce7cc669d998e17b209e8b133df9e13da064`  
		Last Modified: Thu, 23 Mar 2023 07:34:04 GMT  
		Size: 10.7 MB (10662010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9437ab03a3b730ed3d31f18a79500c8ce379f2a971ed27695d60f38e887121b2`  
		Last Modified: Thu, 23 Mar 2023 07:34:50 GMT  
		Size: 53.3 MB (53306810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173435a2410e4cdc681e9bd4a44f44da5e7905b9826d94efbc91429ed38126f1`  
		Last Modified: Thu, 23 Mar 2023 07:36:46 GMT  
		Size: 178.9 MB (178928274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b697a4587d95ab5efc8a0a412192a98a5bbfdf6c01fa964f5595faf79671febf`  
		Last Modified: Thu, 23 Mar 2023 13:59:57 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57375cc6d4f2c7322f20eb8ddbeb94b616675f9ae5e29d3f1014180d52ff4ac8`  
		Last Modified: Thu, 23 Mar 2023 14:00:09 GMT  
		Size: 14.4 MB (14448082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:stable` - linux; ppc64le

```console
$ docker pull perl@sha256:aef3296256670c5d349d03d7d4156bb2984707b8003ec9160786bb5fb2ea0b2d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.2 MB (346239596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7eac1e079ebf285ee82829895a78ccce818239136880d072c217101acd0dc39e`
-	Default Command: `["perl5.36.0","-de0"]`

```dockerfile
# Wed, 12 Apr 2023 00:07:58 GMT
ADD file:c3c2a10473ddaa3d8a30ca99b19ad3599d0e60d826c4e0315bdb7463352ebc09 in / 
# Wed, 12 Apr 2023 00:08:02 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 09:31:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 09:32:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 09:33:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 09:36:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 15:37:31 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 12 Apr 2023 15:37:31 GMT
WORKDIR /usr/src/perl
# Wed, 12 Apr 2023 15:45:56 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.0.tar.xz -o perl-5.36.0.tar.xz     && echo '0f386dccbee8e26286404b2cca144e1005be65477979beb9b1ba272d4819bcf0 *perl-5.36.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.0.tar.xz -C /usr/src/perl     && rm perl-5.36.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Wed, 12 Apr 2023 15:45:58 GMT
WORKDIR /
# Wed, 12 Apr 2023 15:45:59 GMT
CMD ["perl5.36.0" "-de0"]
```

-	Layers:
	-	`sha256:2d3ffdd4610a019889b845cc82b3d956ad85cca78ad4bff2d5e5522bd02c17e7`  
		Last Modified: Wed, 12 Apr 2023 00:12:37 GMT  
		Size: 58.9 MB (58926600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00772c18aacd8e2ae167f5f94b2e86c7b77fd3f7790dc5e6754e48fcce1ff484`  
		Last Modified: Wed, 12 Apr 2023 09:45:12 GMT  
		Size: 5.4 MB (5415380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1877fd565f7c580ab3b8fd343d19de69c9c3334787d6a3c93c9c21fe08ea32a`  
		Last Modified: Wed, 12 Apr 2023 09:45:13 GMT  
		Size: 11.6 MB (11629984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a24a9774fce2d157b32633fbd68d6d4777632ca49b0a35d2e9be9a2455d88b`  
		Last Modified: Wed, 12 Apr 2023 09:45:40 GMT  
		Size: 58.9 MB (58865366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d134f385b05ace42f019d92548a9dd6708f9ae2ee3269131645b4ff67b2463`  
		Last Modified: Wed, 12 Apr 2023 09:46:38 GMT  
		Size: 196.2 MB (196160009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6892a6618630101e81d196a0d238cc146dc8ba2673577d4754bf363ccef9e46e`  
		Last Modified: Wed, 12 Apr 2023 16:47:19 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec322373e2d37137cf49db4ad414a2e97aed43bbca2d5e1741d0cf6d314b510`  
		Last Modified: Wed, 12 Apr 2023 16:47:25 GMT  
		Size: 15.2 MB (15242090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:stable` - linux; s390x

```console
$ docker pull perl@sha256:20dfa0018e285d37fd2c68a1b615eec106c7747ff9904f11d9cc9afbf7712f92
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.7 MB (311672505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46b5803d1379514c0b4f11928f398438fb1835aa911a3e141e259f2cc55cc261`
-	Default Command: `["perl5.36.0","-de0"]`

```dockerfile
# Wed, 12 Apr 2023 00:00:25 GMT
ADD file:ab4e28724d04724a57e0f5bbe299d3361103f05ad1978dc3bfef243c1f9d6476 in / 
# Wed, 12 Apr 2023 00:00:38 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:26:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:26:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 00:27:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:28:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:43:11 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 12 Apr 2023 01:43:12 GMT
WORKDIR /usr/src/perl
# Wed, 12 Apr 2023 01:49:06 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.0.tar.xz -o perl-5.36.0.tar.xz     && echo '0f386dccbee8e26286404b2cca144e1005be65477979beb9b1ba272d4819bcf0 *perl-5.36.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.0.tar.xz -C /usr/src/perl     && rm perl-5.36.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Wed, 12 Apr 2023 01:49:11 GMT
WORKDIR /
# Wed, 12 Apr 2023 01:49:11 GMT
CMD ["perl5.36.0" "-de0"]
```

-	Layers:
	-	`sha256:042263756d7dc47bf98a243871107aa3a2b41acda91d104d8b4e148749a43dda`  
		Last Modified: Wed, 12 Apr 2023 00:05:03 GMT  
		Size: 53.3 MB (53286682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2973b8c98f9da7833ab9cd69185dd958a8939a30136cdcfedb66ce775db358ee`  
		Last Modified: Wed, 12 Apr 2023 00:32:48 GMT  
		Size: 5.1 MB (5149313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f740d13ac612bf8b6489559a7945ec1439fee2d5eba455ab0db047cd3f30a9a`  
		Last Modified: Wed, 12 Apr 2023 00:32:49 GMT  
		Size: 10.8 MB (10766104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c0067783f401b099adca196dce9e464e66236e49faba106e2f04ac73a90df7`  
		Last Modified: Wed, 12 Apr 2023 00:33:02 GMT  
		Size: 54.1 MB (54061843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1b5accdd9fd68a290692e1a0a3d853312f236ae0463540b5fdd97d598cc7a6`  
		Last Modified: Wed, 12 Apr 2023 00:33:28 GMT  
		Size: 172.8 MB (172815473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fcf796542ca12f880ea32e3d918cf25d5bfc57c541d0fab5364e8ffd59636b6`  
		Last Modified: Wed, 12 Apr 2023 03:32:55 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3afea4c47d4364d9c60ab0dc155931a0e729e79aba7fabdff05bb4d97e30cf87`  
		Last Modified: Wed, 12 Apr 2023 03:32:58 GMT  
		Size: 15.6 MB (15592923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
