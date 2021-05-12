## `perl:5-stretch`

```console
$ docker pull perl@sha256:fba0698d5b0caf827e7f6a633b3cbe667821256db9fca1a01f3b9f794c558eaa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `perl:5-stretch` - linux; amd64

```console
$ docker pull perl@sha256:8e5c5043a97f09a79abf495abb52b66ce2a6cd8d60ba86f020d9853533c6974a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.2 MB (339227102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76461ad1184224d58c29a2159d4c9dd8a79f3e1be57daff3bfb50a29f543a965`
-	Default Command: `["perl5.32.1","-de0"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:41 GMT
ADD file:e3d37689e896a83d39040f2c95091ff88f3899b5b410dbf76908dd6c938b8cb5 in / 
# Sat, 10 Apr 2021 01:21:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:57:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:57:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 01:57:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:58:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 08:09:03 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 10 Apr 2021 08:09:03 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Sat, 10 Apr 2021 08:09:03 GMT
WORKDIR /usr/src/perl
# Sat, 10 Apr 2021 08:16:04 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.1.tar.xz -o perl-5.32.1.tar.xz     && echo '57cc47c735c8300a8ce2fa0643507b44c4ae59012bfdad0121313db639e02309 *perl-5.32.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.1.tar.xz -C /usr/src/perl     && rm perl-5.32.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Sat, 10 Apr 2021 08:16:04 GMT
WORKDIR /
# Sat, 10 Apr 2021 08:16:04 GMT
CMD ["perl5.32.1" "-de0"]
```

-	Layers:
	-	`sha256:76b8ef87096fa726adbe8f073ef69bb5664bac19474c5cce4dd69e08a234903b`  
		Last Modified: Sat, 10 Apr 2021 01:27:52 GMT  
		Size: 45.4 MB (45380037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2bafe8a0f40509cc10249087268e66a662e437f10e9598a09abb5687038a57`  
		Last Modified: Sat, 10 Apr 2021 02:04:34 GMT  
		Size: 11.3 MB (11286411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53ce1fd2746e8d2037f1b0b91ddea0cc7411eb3e5949fe10c0320aca8f7392b`  
		Last Modified: Sat, 10 Apr 2021 02:04:33 GMT  
		Size: 4.3 MB (4342420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a8c1bd5887cc4a89e1f286fed9ee31ce12dba9f6813cf14082ada3e9ab6f63`  
		Last Modified: Sat, 10 Apr 2021 02:04:55 GMT  
		Size: 49.8 MB (49786874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a803dc0b40fcd10faee3fb3ebb2d7aaa88500520e6295295f5163c4bb48548b`  
		Last Modified: Sat, 10 Apr 2021 02:05:48 GMT  
		Size: 214.3 MB (214347112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfc21924b866ffad91e6cd2d83026e7bb06cc0289cf14af35d84a5353db4bac`  
		Last Modified: Sat, 10 Apr 2021 12:19:14 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8148f3410bb2c8294ffd24f3755faea3f1fcad3299fc26fe54bd633b11bafbe7`  
		Last Modified: Sat, 10 Apr 2021 12:19:17 GMT  
		Size: 14.1 MB (14084045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-stretch` - linux; arm variant v7

```console
$ docker pull perl@sha256:8b8a5c11d97fd78a8fb527cbc3dbe572e800e737e0776e81a48dfb0841cb8a80
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.3 MB (310348565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdad9cbc2e89b205f9d2b73e263d02315cd25cd4be19c8918870a373a36e2986`
-	Default Command: `["perl5.32.1","-de0"]`

```dockerfile
# Wed, 12 May 2021 01:11:51 GMT
ADD file:81cfd4e746bdfcc19847240b77012487652be22dbd5741ccb2485a4207f2b73f in / 
# Wed, 12 May 2021 01:11:56 GMT
CMD ["bash"]
# Wed, 12 May 2021 03:53:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 03:53:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 03:54:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 03:56:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:28:00 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 12 May 2021 06:28:11 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Wed, 12 May 2021 06:28:16 GMT
WORKDIR /usr/src/perl
# Wed, 12 May 2021 06:49:39 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.1.tar.xz -o perl-5.32.1.tar.xz     && echo '57cc47c735c8300a8ce2fa0643507b44c4ae59012bfdad0121313db639e02309 *perl-5.32.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.1.tar.xz -C /usr/src/perl     && rm perl-5.32.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Wed, 12 May 2021 06:49:52 GMT
WORKDIR /
# Wed, 12 May 2021 06:49:57 GMT
CMD ["perl5.32.1" "-de0"]
```

-	Layers:
	-	`sha256:55b9a6b6b2552c5b2eac0a316e75a7bc18092819ee25c4f1d4d54700bcc1d3dc`  
		Last Modified: Wed, 12 May 2021 01:21:23 GMT  
		Size: 42.1 MB (42120307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9949293f349d0c9019996e174c80df7a8a710fba2d4f1155451c228e33bc1f9e`  
		Last Modified: Wed, 12 May 2021 04:04:11 GMT  
		Size: 9.9 MB (9939912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2260f0f7d4174518bdec698aad994bd3fdc95ebc5b34c60ed84955b118cccebb`  
		Last Modified: Wed, 12 May 2021 04:04:10 GMT  
		Size: 3.9 MB (3921255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b560815c9657e548da0f3b44c74b3669291c71ef08e2dcaded2c5dfa6c07393b`  
		Last Modified: Wed, 12 May 2021 04:04:34 GMT  
		Size: 46.1 MB (46125864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3095a92b94fd2b88dc3f432f959d1825c17cad0a11bd87f295d24959177c71`  
		Last Modified: Wed, 12 May 2021 04:05:35 GMT  
		Size: 195.0 MB (194995404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4a9e22ba3bfcd840df56e48f9d9684a35c6bcaede9f9c28ea4fbba02b848f2`  
		Last Modified: Wed, 12 May 2021 10:48:20 GMT  
		Size: 206.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e56809d56936a8090e1d4e75dc198651c0c2c6ca7426d338354e66af21357b3`  
		Last Modified: Wed, 12 May 2021 10:48:27 GMT  
		Size: 13.2 MB (13245617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-stretch` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:92bc10259cba2438707a3f9a1e9a676d42cc8f58e52d07d8afc498baa55db3e3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **320.8 MB (320835705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e71972d86cf2e33ac7c093f3869a72ae8d5e4c955cea7ea15e14328e5a5381fa`
-	Default Command: `["perl5.32.1","-de0"]`

```dockerfile
# Wed, 12 May 2021 00:56:12 GMT
ADD file:9582243afc9973a3708fda530270ae8f23796b20a532a9f07e4faaf245e2cdc0 in / 
# Wed, 12 May 2021 00:56:18 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:41:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:41:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 01:42:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:44:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 08:08:28 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 12 May 2021 08:08:29 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Wed, 12 May 2021 08:08:30 GMT
WORKDIR /usr/src/perl
# Wed, 12 May 2021 08:18:21 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.1.tar.xz -o perl-5.32.1.tar.xz     && echo '57cc47c735c8300a8ce2fa0643507b44c4ae59012bfdad0121313db639e02309 *perl-5.32.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.1.tar.xz -C /usr/src/perl     && rm perl-5.32.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Wed, 12 May 2021 08:18:23 GMT
WORKDIR /
# Wed, 12 May 2021 08:18:23 GMT
CMD ["perl5.32.1" "-de0"]
```

-	Layers:
	-	`sha256:41f38ce3010a5142300d74e5e19db4dea7694f4771471c330fff27c633f8ba32`  
		Last Modified: Wed, 12 May 2021 01:04:15 GMT  
		Size: 43.2 MB (43177820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ac4bedb842678b3f7ca4713dead8d22045096d5176f53f8d191785b69f236f`  
		Last Modified: Wed, 12 May 2021 01:51:20 GMT  
		Size: 10.2 MB (10201144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea6e1b91eb654daaf672ce148b8e9bc5ba6326c274d202bab26c504f0451e73f`  
		Last Modified: Wed, 12 May 2021 01:51:18 GMT  
		Size: 4.1 MB (4096687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d312b156251ad6bb876bd760bf0fd069f10c10554c397edcf563553da2c1914b`  
		Last Modified: Wed, 12 May 2021 01:51:40 GMT  
		Size: 47.7 MB (47736486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd81579302617d9c4d8c8779ed768a00da2c73452745f51a0f4214a0d9c408a5`  
		Last Modified: Wed, 12 May 2021 01:52:35 GMT  
		Size: 201.7 MB (201720830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c206ecd0d2b55f7ac91c87f20029f4b0d38985eb866f4d487a4ba9d18c7fff4`  
		Last Modified: Wed, 12 May 2021 12:08:45 GMT  
		Size: 205.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e993349cc2728d63da8721da6c9c60ef9beb27704e95eaa07aeaf799ab442b`  
		Last Modified: Wed, 12 May 2021 12:08:51 GMT  
		Size: 13.9 MB (13902533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-stretch` - linux; 386

```console
$ docker pull perl@sha256:5147d13319e6fd62787155dcd3e4f9ab920d2c12c7a0735055c4f06f55cbd894
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.3 MB (346258111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6a8023231451779a9cb6d968f42fb408d595680edd51e16c019ed2ce25544ed`
-	Default Command: `["perl5.32.1","-de0"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:14 GMT
ADD file:cebeeb1ed904e9433778c60c09ed31939334fd4f1c9550cce191b3bff4df0272 in / 
# Sat, 10 Apr 2021 00:41:14 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 03:22:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 03:22:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 03:23:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 03:24:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 04:14:43 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 10 Apr 2021 04:14:44 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Sat, 10 Apr 2021 04:14:44 GMT
WORKDIR /usr/src/perl
# Sat, 10 Apr 2021 04:27:50 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.1.tar.xz -o perl-5.32.1.tar.xz     && echo '57cc47c735c8300a8ce2fa0643507b44c4ae59012bfdad0121313db639e02309 *perl-5.32.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.1.tar.xz -C /usr/src/perl     && rm perl-5.32.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Sat, 10 Apr 2021 04:27:50 GMT
WORKDIR /
# Sat, 10 Apr 2021 04:27:50 GMT
CMD ["perl5.32.1" "-de0"]
```

-	Layers:
	-	`sha256:f8270215e0f4bee2960e85333265840385530ee75e6f553f8cfc3e5b0534bf0e`  
		Last Modified: Sat, 10 Apr 2021 00:48:47 GMT  
		Size: 46.1 MB (46098724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e882cae824a5753e90da159075517ecd98fd4d38f11d907927f6664b6913c74`  
		Last Modified: Sat, 10 Apr 2021 03:34:01 GMT  
		Size: 11.3 MB (11336698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95a143794ab784f7db99b9f4ced22f07b03e17145a1b2b5ce5b731f4a3bad3f8`  
		Last Modified: Sat, 10 Apr 2021 03:33:59 GMT  
		Size: 4.6 MB (4565009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1929129fdd2546c216795ea9a1841aac230e86cc565cb6476fd2bbb168e6ebbe`  
		Last Modified: Sat, 10 Apr 2021 03:34:26 GMT  
		Size: 51.3 MB (51264698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15801b27fa97d290ae18cf943529c3a36e1ca45ee01de3c84913551e78e89281`  
		Last Modified: Sat, 10 Apr 2021 03:35:27 GMT  
		Size: 219.4 MB (219421873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d19b63a7b6b917412632973c36cd741d298d7a3e51075f3ec16df443b5b5a9d6`  
		Last Modified: Sat, 10 Apr 2021 08:08:24 GMT  
		Size: 206.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8587152b12334c7083d461d87453ef92719ba0b964e28fd0054e4b6c12d29dd`  
		Last Modified: Sat, 10 Apr 2021 08:08:31 GMT  
		Size: 13.6 MB (13570903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
