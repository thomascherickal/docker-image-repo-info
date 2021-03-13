## `perl:threaded`

```console
$ docker pull perl@sha256:0f90ff6d5625775d3c6f643d7e39c21f72d5238280b191d93912dedf6edf71b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `perl:threaded` - linux; amd64

```console
$ docker pull perl@sha256:563206ca408fd2cc30a9430c85edb165cc08bbb519cdb47f4b73e8b3acce04cf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.5 MB (326526203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22d14f34c2be9330c1859c95dd6d993c49f08e46a1501191a9a5f680cc2bfa3b`
-	Default Command: `["perl5.32.1","-de0"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:27 GMT
ADD file:575bf0d00d72810609a4118728923f11625b43de536352fe69a341086e4ebfd1 in / 
# Fri, 12 Mar 2021 02:20:28 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:49:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:49:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 12 Mar 2021 02:49:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:50:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 22:45:08 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Fri, 12 Mar 2021 22:45:08 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Fri, 12 Mar 2021 22:45:09 GMT
WORKDIR /usr/src/perl
# Fri, 12 Mar 2021 23:31:22 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.1.tar.xz -o perl-5.32.1.tar.xz     && echo '57cc47c735c8300a8ce2fa0643507b44c4ae59012bfdad0121313db639e02309 *perl-5.32.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.1.tar.xz -C /usr/src/perl     && rm perl-5.32.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Fri, 12 Mar 2021 23:31:22 GMT
WORKDIR /
# Fri, 12 Mar 2021 23:31:22 GMT
CMD ["perl5.32.1" "-de0"]
```

-	Layers:
	-	`sha256:e22122b926a1a853d61887fa35c3fe53e05ee7dc0f2f488936dc9838bd0e230d`  
		Last Modified: Fri, 12 Mar 2021 02:25:38 GMT  
		Size: 50.4 MB (50400353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29e09ae83733d697508e34827538cc0129b8719b85db943041c5d37287bcb81`  
		Last Modified: Fri, 12 Mar 2021 03:19:09 GMT  
		Size: 7.8 MB (7832474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e319e3daef68c36099bf3b534377a78d373f67bde3d156119c2463f5fe133ac5`  
		Last Modified: Fri, 12 Mar 2021 03:19:09 GMT  
		Size: 10.0 MB (9997147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e499244fe254b6f980c82ea555f38e7a6527e5105545922005e88a6b81b01cac`  
		Last Modified: Fri, 12 Mar 2021 03:19:36 GMT  
		Size: 51.8 MB (51839506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6ebed20e89bafb5798e66484bd3f1bb41f6e8f6443d231f85b9b6eb2fec334`  
		Last Modified: Fri, 12 Mar 2021 03:20:20 GMT  
		Size: 192.3 MB (192341639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a4f0234046527bd35a4e7c8ccd54fb659b3e9db883e833b0c417004f9648a8`  
		Last Modified: Sat, 13 Mar 2021 02:07:51 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5aa92e1fdf3311f2b5778aa8f64df6163bde19fe5d84f320cda3a5b59703bde`  
		Last Modified: Sat, 13 Mar 2021 02:09:29 GMT  
		Size: 14.1 MB (14114881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded` - linux; arm variant v7

```console
$ docker pull perl@sha256:89ba6a912e0722d11feeb49a0bafc7c122b5b2160fb66416fd4f469def4a96fb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.5 MB (291471180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d0de961daedb2271e19153a6a2d23b37d4bf294e53d205e125454dbffd877a6`
-	Default Command: `["perl5.32.1","-de0"]`

```dockerfile
# Fri, 12 Mar 2021 01:59:39 GMT
ADD file:7a272c0a2bf029fde32186ff5d55a8ef335d159da9770327eedf010bd6e6c42d in / 
# Fri, 12 Mar 2021 01:59:44 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 03:32:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 03:32:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 12 Mar 2021 03:33:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 03:35:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 04:59:21 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Fri, 12 Mar 2021 04:59:21 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Fri, 12 Mar 2021 04:59:22 GMT
WORKDIR /usr/src/perl
# Fri, 12 Mar 2021 05:50:03 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.1.tar.xz -o perl-5.32.1.tar.xz     && echo '57cc47c735c8300a8ce2fa0643507b44c4ae59012bfdad0121313db639e02309 *perl-5.32.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.1.tar.xz -C /usr/src/perl     && rm perl-5.32.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Fri, 12 Mar 2021 05:50:06 GMT
WORKDIR /
# Fri, 12 Mar 2021 05:50:07 GMT
CMD ["perl5.32.1" "-de0"]
```

-	Layers:
	-	`sha256:199f83f6a2f5a375b8f94d3025f9bbdaca75f4ca46ad0aab2061c331588fa662`  
		Last Modified: Fri, 12 Mar 2021 02:10:00 GMT  
		Size: 45.9 MB (45868120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d535c087e97eba956c56d41b509048f3f9283744c2b2ef7fabbb6a75fe7d3c`  
		Last Modified: Fri, 12 Mar 2021 03:47:04 GMT  
		Size: 7.1 MB (7123778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7cfc4c570eb98f73a8ab1d871e36ff43492038fa4c0279c70ccff1797447d2b`  
		Last Modified: Fri, 12 Mar 2021 03:47:04 GMT  
		Size: 9.3 MB (9343577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2cb364b2d38bcbf9b4e594b01bbf2a4d3509357468c391ebc39660a58df706`  
		Last Modified: Fri, 12 Mar 2021 03:47:29 GMT  
		Size: 47.4 MB (47356842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6a4c96290dae9783769803c208fc6157611ef232af26cb0f1405f42559491b`  
		Last Modified: Fri, 12 Mar 2021 03:48:27 GMT  
		Size: 168.5 MB (168548294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0919c19ae956c79bf54caade389a7bd70d52129ce189cc9b0b429f40eb7a2d9d`  
		Last Modified: Fri, 12 Mar 2021 08:51:26 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe744a9d7997049362d941d3239d561fd91ec8f25d95aaa94073d4e622a16b7`  
		Last Modified: Fri, 12 Mar 2021 08:52:45 GMT  
		Size: 13.2 MB (13230368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:14f721f179a8a8d7b1f58f262b6b93cdd0792a101a7921235446d69559ae16fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.0 MB (316974205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83e71a0b7f19132068f1b658eefcf2730a0324782e8d0b43ce9cb9978b96900e`
-	Default Command: `["perl5.32.1","-de0"]`

```dockerfile
# Fri, 12 Mar 2021 01:53:16 GMT
ADD file:b2e2cca51e131b97e6a7e02af893c7f9b1f7a491b3d5fdaafa80409ed248a706 in / 
# Fri, 12 Mar 2021 01:53:20 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:29:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:29:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 12 Mar 2021 02:30:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:32:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 06:52:30 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Fri, 12 Mar 2021 06:52:31 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Fri, 12 Mar 2021 06:52:33 GMT
WORKDIR /usr/src/perl
# Fri, 12 Mar 2021 07:44:57 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.1.tar.xz -o perl-5.32.1.tar.xz     && echo '57cc47c735c8300a8ce2fa0643507b44c4ae59012bfdad0121313db639e02309 *perl-5.32.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.1.tar.xz -C /usr/src/perl     && rm perl-5.32.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Fri, 12 Mar 2021 07:44:58 GMT
WORKDIR /
# Fri, 12 Mar 2021 07:44:59 GMT
CMD ["perl5.32.1" "-de0"]
```

-	Layers:
	-	`sha256:e9742a63e95a88f8685c4f23a73f7dd15e4039ac1862ce5753c53406a5f7c04a`  
		Last Modified: Fri, 12 Mar 2021 02:01:14 GMT  
		Size: 49.2 MB (49195763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90273c85fdda8648cee9282aa7b01faf0ec1f45451931985b3504c37cf1ac3e6`  
		Last Modified: Fri, 12 Mar 2021 02:43:30 GMT  
		Size: 7.7 MB (7694407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:685f873e984153af9a44cf556c7679b430b9c557d901c7d476725134f28754e7`  
		Last Modified: Fri, 12 Mar 2021 02:43:30 GMT  
		Size: 10.0 MB (9984339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34041dfaf60ca49c213d83e89205fc2b7e222817c9728a4aa4f7d3f09d579c9`  
		Last Modified: Fri, 12 Mar 2021 02:43:54 GMT  
		Size: 52.2 MB (52165212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9688107c15585cc88b559730b6668481b4b5d142a662c94868eb4d7fa262a80`  
		Last Modified: Fri, 12 Mar 2021 02:44:48 GMT  
		Size: 183.9 MB (183888582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0ff1c643236ffa428bbcdf9a953dd288ac3d2d15501de7dd0447de037448d6`  
		Last Modified: Fri, 12 Mar 2021 11:01:49 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0076f3b2418f14dc3a5cc568ecbdece94afd79195a7c503e62967b148fe8a72b`  
		Last Modified: Fri, 12 Mar 2021 11:03:09 GMT  
		Size: 14.0 MB (14045699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded` - linux; 386

```console
$ docker pull perl@sha256:9512ffaffc8406cfd3aede6b24bd9ab9b6f0c5e0ed4412a1860d8758c0149708
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.5 MB (335467317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:158541b28f219acb9299169d0eedad58d0ace10fa58bd47d150d839d58f43a40`
-	Default Command: `["perl5.32.1","-de0"]`

```dockerfile
# Fri, 12 Mar 2021 01:44:10 GMT
ADD file:7fc865376477d0a3207f0488aa53a01be49cf76d0f075eb2d8dfb866f67472c2 in / 
# Fri, 12 Mar 2021 01:44:11 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:16:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:16:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 12 Mar 2021 02:17:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:18:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 15:39:58 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Fri, 12 Mar 2021 15:39:58 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Fri, 12 Mar 2021 15:39:59 GMT
WORKDIR /usr/src/perl
# Fri, 12 Mar 2021 16:39:21 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.1.tar.xz -o perl-5.32.1.tar.xz     && echo '57cc47c735c8300a8ce2fa0643507b44c4ae59012bfdad0121313db639e02309 *perl-5.32.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.1.tar.xz -C /usr/src/perl     && rm perl-5.32.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Fri, 12 Mar 2021 16:39:22 GMT
WORKDIR /
# Fri, 12 Mar 2021 16:39:22 GMT
CMD ["perl5.32.1" "-de0"]
```

-	Layers:
	-	`sha256:a0450ef8e4ab4239c43726ef6f13a160860a6ab25f82c8f011ca37ee436324a2`  
		Last Modified: Fri, 12 Mar 2021 01:51:32 GMT  
		Size: 51.2 MB (51160386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f62290e3e304b8095d37508b9b2051cb2b2d26d61984ec27eb7560a808f020`  
		Last Modified: Fri, 12 Mar 2021 02:36:17 GMT  
		Size: 8.0 MB (7997281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e78fb5d9226b64f0de7250162ff06d8a9871bcc020e50b44675068767d820a5f`  
		Last Modified: Fri, 12 Mar 2021 02:36:17 GMT  
		Size: 10.3 MB (10340057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6f80e285dc0ec638e021f54cc99edebfeba111ee99288f0674a32914c3c063`  
		Last Modified: Fri, 12 Mar 2021 02:36:44 GMT  
		Size: 53.4 MB (53437850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc622bc51edb15bef25984a84dc283b3692df13947304b538321f767144ad4c`  
		Last Modified: Fri, 12 Mar 2021 02:37:39 GMT  
		Size: 198.9 MB (198885897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:871af466bd2dd84de1ab8321b2cb54173faf4187aa210f6545a9226fb6904762`  
		Last Modified: Fri, 12 Mar 2021 20:10:27 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c513cecdeef02f92ead5dbaa5e9ac5c35050006b0ae96aba8bb407271721b4dd`  
		Last Modified: Fri, 12 Mar 2021 20:12:43 GMT  
		Size: 13.6 MB (13645645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded` - linux; ppc64le

```console
$ docker pull perl@sha256:2ab95fec950715f3bd1b71bf5b6e2831cc50b6ea6834d17c6cdae425d4ed7f2d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.0 MB (347956620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71ddae941dd2850ee27c3118e568d9068bd6d75d2bd53c3f9d43b23c4c188bfd`
-	Default Command: `["perl5.32.1","-de0"]`

```dockerfile
# Fri, 12 Mar 2021 02:31:55 GMT
ADD file:75cbd246f27dc871f6d43b196814d29950e19fbcf60ba31740b0f3b69d1eb5cf in / 
# Fri, 12 Mar 2021 02:32:10 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 11:02:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 11:03:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 12 Mar 2021 11:06:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 11:24:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 13 Mar 2021 02:33:47 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 13 Mar 2021 02:33:48 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Sat, 13 Mar 2021 02:33:54 GMT
WORKDIR /usr/src/perl
# Sat, 13 Mar 2021 02:47:44 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.1.tar.xz -o perl-5.32.1.tar.xz     && echo '57cc47c735c8300a8ce2fa0643507b44c4ae59012bfdad0121313db639e02309 *perl-5.32.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.1.tar.xz -C /usr/src/perl     && rm perl-5.32.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Sat, 13 Mar 2021 02:47:52 GMT
WORKDIR /
# Sat, 13 Mar 2021 02:47:55 GMT
CMD ["perl5.32.1" "-de0"]
```

-	Layers:
	-	`sha256:e82e55acc97d8fc958b57715031c249868ac5d8978e8d9f94ca4c15d553fe3cf`  
		Last Modified: Fri, 12 Mar 2021 02:44:17 GMT  
		Size: 54.1 MB (54136226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d7821ad6b4fb4c264f87306146cca85ae319c012535ca5ba869f297681f528`  
		Last Modified: Fri, 12 Mar 2021 12:00:12 GMT  
		Size: 8.3 MB (8271375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efadb27dbbd9968d195399537fc5c6be6627d842ed384ff4e9510632b9f24720`  
		Last Modified: Fri, 12 Mar 2021 12:00:09 GMT  
		Size: 10.7 MB (10727647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65fb57ad94f43eee037ef854e05c8d78064d228650a412c8cbf509359c99228`  
		Last Modified: Fri, 12 Mar 2021 12:02:19 GMT  
		Size: 57.5 MB (57456654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39177f6c9e22c9bf455b910e45774661c45b56f07426974183f48ea7e664943d`  
		Last Modified: Fri, 12 Mar 2021 12:06:24 GMT  
		Size: 203.2 MB (203180145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:696367325c505a8852ddd835539af08c739ae2a4dc1fe72361887b2da5525bd5`  
		Last Modified: Sat, 13 Mar 2021 03:14:44 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b57534db074babaf9ad7cdf037b94c4545b25ab587476c08aba8a7cf4bfc55`  
		Last Modified: Sat, 13 Mar 2021 03:15:19 GMT  
		Size: 14.2 MB (14184370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded` - linux; s390x

```console
$ docker pull perl@sha256:22c40bf6bf768bef56479ce31d0af7cbebe28acb734b815e99581fe064fca9b9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.9 MB (308934580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0840f4e2336a7ebeb44775c5221ff83a63c2f659b87122eefaaa1bacd2a92a63`
-	Default Command: `["perl5.32.1","-de0"]`

```dockerfile
# Fri, 12 Mar 2021 01:45:42 GMT
ADD file:c1bc4d97e132d650b9f7848521ea163735e8d93b365da94640ff25e0e01bc891 in / 
# Fri, 12 Mar 2021 01:45:47 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:31:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:31:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 12 Mar 2021 02:32:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:33:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 03:30:28 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Fri, 12 Mar 2021 03:30:28 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Fri, 12 Mar 2021 03:30:29 GMT
WORKDIR /usr/src/perl
# Fri, 12 Mar 2021 03:48:14 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.1.tar.xz -o perl-5.32.1.tar.xz     && echo '57cc47c735c8300a8ce2fa0643507b44c4ae59012bfdad0121313db639e02309 *perl-5.32.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.1.tar.xz -C /usr/src/perl     && rm perl-5.32.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Fri, 12 Mar 2021 03:48:16 GMT
WORKDIR /
# Fri, 12 Mar 2021 03:48:17 GMT
CMD ["perl5.32.1" "-de0"]
```

-	Layers:
	-	`sha256:2fc1f9e428b932a8750b1c7f11f48b4c9a41328e9107b957451d8b8efbfd3fce`  
		Last Modified: Fri, 12 Mar 2021 01:50:13 GMT  
		Size: 49.0 MB (48969030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:befe52bd5ee0309720b929d18591173abb18f1edb53333e9dd9bd9f183ccfb43`  
		Last Modified: Fri, 12 Mar 2021 02:39:33 GMT  
		Size: 7.4 MB (7399848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c50286b18ab639a9609fab3ff02da0b0c7f4463147aa750868999fd2cb3c670`  
		Last Modified: Fri, 12 Mar 2021 02:39:33 GMT  
		Size: 9.9 MB (9883075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957e17b0db43215705ba4f0a95f8a4a58939895c2b6675d2c09f3243643ef861`  
		Last Modified: Fri, 12 Mar 2021 02:39:48 GMT  
		Size: 51.4 MB (51380029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e2251fd1ff0353af9654069600392e9d11eb924b7f3e0c52d5681eb12cab5e8`  
		Last Modified: Fri, 12 Mar 2021 02:40:17 GMT  
		Size: 176.8 MB (176848101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc3794e03df2af0067c0556b69189abab1fb3cde5ad21a96cc642614c703732`  
		Last Modified: Fri, 12 Mar 2021 04:48:59 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe2d50df67da2409fb46d66adaa01876fb57f1de574a276476166c591829b42e`  
		Last Modified: Fri, 12 Mar 2021 04:49:39 GMT  
		Size: 14.5 MB (14454295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
