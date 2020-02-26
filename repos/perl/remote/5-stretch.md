## `perl:5-stretch`

```console
$ docker pull perl@sha256:2e401ae829313c423c6f9ca6a5a79fc7940f6e0f23819677bf40e2d81a99d6d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `perl:5-stretch` - linux; amd64

```console
$ docker pull perl@sha256:bbcdc841f373dde17f1fe18cee88fce1cac383e9d40a2c5ecab964cd6a3e5c0e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.3 MB (339252092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e8416b355d3f1e21deb21a2c1829ac362d92df9c72ca5e6d9468f48f17676b8`
-	Default Command: `["perl5.30.1","-de0"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:41 GMT
ADD file:8a9218592e5d736a05a1821a6dd38b205cdd8197c26a5aa33f6fc22fbfaa1c4d in / 
# Sat, 01 Feb 2020 17:23:41 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 00:33:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 00:34:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 02 Feb 2020 00:34:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 00:35:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 01:00:50 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sun, 02 Feb 2020 01:00:51 GMT
COPY file:15650064fd29deac721f0aa084ddb3d41db77b78e2907775e257bd67e116ade4 in /usr/src/perl/ 
# Sun, 02 Feb 2020 01:00:51 GMT
WORKDIR /usr/src/perl
# Sun, 02 Feb 2020 01:10:40 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.30.1.tar.xz -o perl-5.30.1.tar.xz     && echo '7336cd3ed0535eb61b76a71350effcfa7c88b44faf37d64d70952ced5d38cd35 *perl-5.30.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.30.1.tar.xz -C /usr/src/perl     && rm perl-5.30.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Sun, 02 Feb 2020 01:10:40 GMT
WORKDIR /
# Sun, 02 Feb 2020 01:10:40 GMT
CMD ["perl5.30.1" "-de0"]
```

-	Layers:
	-	`sha256:3192219afd04f93d90f0af7f89cb527d1af2a16975ea391ea8517c602ad6ddb6`  
		Last Modified: Sat, 01 Feb 2020 17:28:49 GMT  
		Size: 45.4 MB (45380658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c160265e75550c2ed099aa7d3906b3fef0bf046a2aeead136f8e587a015159`  
		Last Modified: Sun, 02 Feb 2020 00:42:04 GMT  
		Size: 10.8 MB (10797219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4fe40d0e618e3319afb689c3570bb87e8e8cf51bca080364d1552317bc66c2`  
		Last Modified: Sun, 02 Feb 2020 00:42:02 GMT  
		Size: 4.3 MB (4340216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d647f502a07e6daaee43c23cfac9399501b1d7f55fb4c60d56307e23f0ed5a5`  
		Last Modified: Sun, 02 Feb 2020 00:42:26 GMT  
		Size: 50.1 MB (50073989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8bd59397b26db56ddd19f152a7095a91795cf4af7f144ebc4dae741df451039`  
		Last Modified: Sun, 02 Feb 2020 00:43:16 GMT  
		Size: 214.8 MB (214840255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05b5ac73caf1c34b00d19663a31108d56e8fc280ff7d215fa551ba7b8395d12`  
		Last Modified: Sun, 02 Feb 2020 05:19:20 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055dc8fce1d1e43ca16f7bc503a6b6b23bc2b7922d1a49ffbc6a9c8bdd939a9b`  
		Last Modified: Sun, 02 Feb 2020 05:19:26 GMT  
		Size: 13.8 MB (13819339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-stretch` - linux; arm variant v7

```console
$ docker pull perl@sha256:83de50e5dc210f107fc1d31ce408bebdf78a9cc717eb5ec90f02f6d183936595
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.4 MB (310445135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f550598aa19cf14e51ebb373d958d80a333fb20f4e7101df1dab24661389e4a7`
-	Default Command: `["perl5.30.1","-de0"]`

```dockerfile
# Wed, 26 Feb 2020 00:59:40 GMT
ADD file:6497e2f777f4487d9221931005a8b4b81c021442a769b581e223cf30c81ff553 in / 
# Wed, 26 Feb 2020 00:59:53 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 02:27:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 02:27:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Feb 2020 02:28:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 02:30:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 04:48:25 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 26 Feb 2020 04:48:25 GMT
COPY file:15650064fd29deac721f0aa084ddb3d41db77b78e2907775e257bd67e116ade4 in /usr/src/perl/ 
# Wed, 26 Feb 2020 04:48:27 GMT
WORKDIR /usr/src/perl
# Wed, 26 Feb 2020 04:58:30 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.30.1.tar.xz -o perl-5.30.1.tar.xz     && echo '7336cd3ed0535eb61b76a71350effcfa7c88b44faf37d64d70952ced5d38cd35 *perl-5.30.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.30.1.tar.xz -C /usr/src/perl     && rm perl-5.30.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Wed, 26 Feb 2020 04:58:31 GMT
WORKDIR /
# Wed, 26 Feb 2020 04:58:32 GMT
CMD ["perl5.30.1" "-de0"]
```

-	Layers:
	-	`sha256:2478a2ed882cb5fbb5e4e92c9f580da9ca52f5fc78b8bb439ecbf3ac18023caa`  
		Last Modified: Wed, 26 Feb 2020 01:11:29 GMT  
		Size: 42.1 MB (42100335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c541086e0dffa72464d4077dcc60504a1c08a73ecec554c159269786ba08fed`  
		Last Modified: Wed, 26 Feb 2020 02:37:24 GMT  
		Size: 9.5 MB (9498391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf0f97b070f73118badb36d21af3459f8317d4ac6d45aec680092cc962f1c47`  
		Last Modified: Wed, 26 Feb 2020 02:37:23 GMT  
		Size: 3.9 MB (3918781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d620eb05d9fd9184b8f200537b866a27af44aa6d7ef4dd6113bf1b51421d4795`  
		Last Modified: Wed, 26 Feb 2020 02:37:45 GMT  
		Size: 46.4 MB (46391794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f6d10893167716e03df782cfd3f378f099999787bc15655d27fd06cc601e46`  
		Last Modified: Wed, 26 Feb 2020 02:38:40 GMT  
		Size: 195.5 MB (195548773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d024d0bb5a1be6519b330045bb60909d86fd0dd19411ff90e1fd6f3b97b234ea`  
		Last Modified: Wed, 26 Feb 2020 08:27:03 GMT  
		Size: 444.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aa2ef16f70b3b7dc7398364d37ec505f2d3f6aa31815a9fc0cf506bffc7b0dd`  
		Last Modified: Wed, 26 Feb 2020 08:27:09 GMT  
		Size: 13.0 MB (12986617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-stretch` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:106ad76117f19c9e63967c5be52f7a3edc695b3decfd0f709199fce45d7d32f4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **320.9 MB (320915172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c7782de8a04f84722443b7a62ae1e3fd72ee82d70076e6e8f108dad211ff3c5`
-	Default Command: `["perl5.30.1","-de0"]`

```dockerfile
# Sat, 01 Feb 2020 16:43:01 GMT
ADD file:1618e6474dbe6462a610ce7eed99f0bfd087ea37ddfc287bbd69def5c24ede47 in / 
# Sat, 01 Feb 2020 16:43:02 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:29:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:29:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 17:30:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:32:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 21:51:16 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 01 Feb 2020 21:51:17 GMT
COPY file:15650064fd29deac721f0aa084ddb3d41db77b78e2907775e257bd67e116ade4 in /usr/src/perl/ 
# Sat, 01 Feb 2020 21:51:18 GMT
WORKDIR /usr/src/perl
# Sat, 01 Feb 2020 22:01:21 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.30.1.tar.xz -o perl-5.30.1.tar.xz     && echo '7336cd3ed0535eb61b76a71350effcfa7c88b44faf37d64d70952ced5d38cd35 *perl-5.30.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.30.1.tar.xz -C /usr/src/perl     && rm perl-5.30.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Sat, 01 Feb 2020 22:01:22 GMT
WORKDIR /
# Sat, 01 Feb 2020 22:01:23 GMT
CMD ["perl5.30.1" "-de0"]
```

-	Layers:
	-	`sha256:df3de44c7096ba135556a1e7044f9e1feee3ef713ab96f0416f71fe78422cbf6`  
		Last Modified: Sat, 01 Feb 2020 16:48:40 GMT  
		Size: 43.2 MB (43166749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf173a01baf7d45b479bb380ece219cbf0ea52178e9b8cdc5b87891759d1122`  
		Last Modified: Sat, 01 Feb 2020 17:39:19 GMT  
		Size: 9.7 MB (9748586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3392eac7bc27f3bd5fcb024413ca55ec4115c22da3e229567d5fc03cd4ff4e4`  
		Last Modified: Sat, 01 Feb 2020 17:39:18 GMT  
		Size: 4.1 MB (4094322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04a82fc9ca296b095585ba7f3f6d83566428dbefcbfd284e242039aba97840b2`  
		Last Modified: Sat, 01 Feb 2020 17:39:40 GMT  
		Size: 48.0 MB (48024205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9a981e1269e4bf23132efb6a90365b5d82020f20a2ae5252c2d7c3b9ad7f48`  
		Last Modified: Sat, 01 Feb 2020 17:40:34 GMT  
		Size: 202.2 MB (202233524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7003de42f324334e5da0dd9f6cea31223693a5e587720bc317c7b6af3a72e38d`  
		Last Modified: Sun, 02 Feb 2020 01:30:21 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ffb59acc97cf7f14f2704ce786f90dcf79049aaa8e9aa18243173f8d2c5967`  
		Last Modified: Sun, 02 Feb 2020 01:30:30 GMT  
		Size: 13.6 MB (13647341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-stretch` - linux; 386

```console
$ docker pull perl@sha256:10fa0c1550e98e21c94ae90a621f2242382e8bc3fb37c90abdf207a49f33f476
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.4 MB (346351180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef03057c6259ce085af9ac8d57f2e25cbddac553be23e8993cbf1dc6f33ce28`
-	Default Command: `["perl5.30.1","-de0"]`

```dockerfile
# Wed, 26 Feb 2020 00:35:22 GMT
ADD file:f57292acaae4c3d7e8b3217b28f9efb27faef1c4e08ca95f4a25d1302355fb51 in / 
# Wed, 26 Feb 2020 00:35:23 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 01:23:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 01:23:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Feb 2020 01:24:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 01:25:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 05:51:55 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 26 Feb 2020 05:51:55 GMT
COPY file:15650064fd29deac721f0aa084ddb3d41db77b78e2907775e257bd67e116ade4 in /usr/src/perl/ 
# Wed, 26 Feb 2020 05:51:55 GMT
WORKDIR /usr/src/perl
# Wed, 26 Feb 2020 06:02:45 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.30.1.tar.xz -o perl-5.30.1.tar.xz     && echo '7336cd3ed0535eb61b76a71350effcfa7c88b44faf37d64d70952ced5d38cd35 *perl-5.30.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.30.1.tar.xz -C /usr/src/perl     && rm perl-5.30.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Wed, 26 Feb 2020 06:02:45 GMT
WORKDIR /
# Wed, 26 Feb 2020 06:02:45 GMT
CMD ["perl5.30.1" "-de0"]
```

-	Layers:
	-	`sha256:ef83ea0a858b11598fe63ce7d80a401ebb47c746763b35564bd712f013cb961f`  
		Last Modified: Wed, 26 Feb 2020 00:41:45 GMT  
		Size: 46.1 MB (46095035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa60bcba0a57a2662cae84d0bd1cc3e9baa383c9a1589cecbb68b4e65d231ce2`  
		Last Modified: Wed, 26 Feb 2020 01:31:18 GMT  
		Size: 10.8 MB (10818060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a172f4142e9968e299cb42a03c7124d1456062e69197d3d50c972ca924d0d107`  
		Last Modified: Wed, 26 Feb 2020 01:31:15 GMT  
		Size: 4.6 MB (4561448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8d299990640c71bf2446b454c0391fe405a3390c363cf97eab4f8fe9cd57e6`  
		Last Modified: Wed, 26 Feb 2020 01:31:40 GMT  
		Size: 51.6 MB (51603478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e7d83f116087dbb03cd1e9e8196a8ccb100d15756be529f99a9e7779dff81e8`  
		Last Modified: Wed, 26 Feb 2020 01:32:40 GMT  
		Size: 220.0 MB (219969557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e60f3a4ddc44569a152455d5708f80f0b7454682f246cec08a1659c49d2c5c`  
		Last Modified: Wed, 26 Feb 2020 10:46:07 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2bf21c1009d88134c94b8ebbf3cea96c6f67d9aa6b07247520570a617405f5`  
		Last Modified: Wed, 26 Feb 2020 10:46:13 GMT  
		Size: 13.3 MB (13303187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-stretch` - linux; ppc64le

```console
$ docker pull perl@sha256:cdbd2453e3075a0bba6f3b99ed11eabdf750d8e39f6208fc35fe0265f241be3c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.2 MB (334189786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46a89554a3c0018a305fdb3cecc4658750baa929320777c2d7df7aa5dabda8a7`
-	Default Command: `["perl5.30.1","-de0"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:12 GMT
ADD file:ebcf4b112436fa7be8efa5ef204cc174c0d1af648c6ab4af968a71aa2ab2cf4a in / 
# Sat, 01 Feb 2020 17:20:16 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 19:04:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 19:05:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 19:06:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 19:13:32 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 23:07:40 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 01 Feb 2020 23:07:41 GMT
COPY file:15650064fd29deac721f0aa084ddb3d41db77b78e2907775e257bd67e116ade4 in /usr/src/perl/ 
# Sat, 01 Feb 2020 23:07:43 GMT
WORKDIR /usr/src/perl
# Sat, 01 Feb 2020 23:14:15 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.30.1.tar.xz -o perl-5.30.1.tar.xz     && echo '7336cd3ed0535eb61b76a71350effcfa7c88b44faf37d64d70952ced5d38cd35 *perl-5.30.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.30.1.tar.xz -C /usr/src/perl     && rm perl-5.30.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Sat, 01 Feb 2020 23:14:20 GMT
WORKDIR /
# Sat, 01 Feb 2020 23:14:23 GMT
CMD ["perl5.30.1" "-de0"]
```

-	Layers:
	-	`sha256:072f803f12e35b1a40604b6081cb448d46529e3eb1d453ebbf56850c211f5bdb`  
		Last Modified: Sat, 01 Feb 2020 17:30:44 GMT  
		Size: 45.7 MB (45652299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1738f3141f5288b7d088c111ef5c0250cf1779363648e4abd0a2fa786691279a`  
		Last Modified: Sat, 01 Feb 2020 19:25:20 GMT  
		Size: 10.0 MB (10002083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3a959eee44d8ac35abe99ef74efe938d0f14c75e8ba029451e3bb2f3c594206`  
		Last Modified: Sat, 01 Feb 2020 19:25:18 GMT  
		Size: 4.3 MB (4296690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c05296e9b4c4e064ac637742557d903aff58a97639760bb778595e90492a8f`  
		Last Modified: Sat, 01 Feb 2020 19:26:08 GMT  
		Size: 50.1 MB (50086371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0053e8ab1908886809e0b53ed05d1644123e096ed152bef227af4bdd63d04506`  
		Last Modified: Sat, 01 Feb 2020 19:28:13 GMT  
		Size: 210.5 MB (210480034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df50b9324f5f3dec29e0b0783efff8d323b602799d8b3916379a0a9107947b6d`  
		Last Modified: Sun, 02 Feb 2020 02:07:08 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df68877ff0aae2ab5d0aa1c9f32f4c54b3f3ed1d4673712e54d45ea091588942`  
		Last Modified: Sun, 02 Feb 2020 02:07:12 GMT  
		Size: 13.7 MB (13671864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-stretch` - linux; s390x

```console
$ docker pull perl@sha256:229b066e911493c31cb3d8e9c3162a7f4029c16699a6a60a504b72c95adcb252
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.6 MB (331634058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcfb279056d0073aa761d67065c65eebc24356f7d9f0087b9dffc264ccd4257f`
-	Default Command: `["perl5.30.1","-de0"]`

```dockerfile
# Wed, 26 Feb 2020 00:44:30 GMT
ADD file:bb76ab55808bcd0567a32c3d7328d5c1719147f0f723a4aa574872eb8f12b4d4 in / 
# Wed, 26 Feb 2020 00:44:38 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 04:42:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 04:42:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Feb 2020 04:42:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 04:44:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 05:09:37 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 26 Feb 2020 05:09:38 GMT
COPY file:15650064fd29deac721f0aa084ddb3d41db77b78e2907775e257bd67e116ade4 in /usr/src/perl/ 
# Wed, 26 Feb 2020 05:09:38 GMT
WORKDIR /usr/src/perl
# Wed, 26 Feb 2020 05:14:34 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.30.1.tar.xz -o perl-5.30.1.tar.xz     && echo '7336cd3ed0535eb61b76a71350effcfa7c88b44faf37d64d70952ced5d38cd35 *perl-5.30.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.30.1.tar.xz -C /usr/src/perl     && rm perl-5.30.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Wed, 26 Feb 2020 05:14:36 GMT
WORKDIR /
# Wed, 26 Feb 2020 05:14:36 GMT
CMD ["perl5.30.1" "-de0"]
```

-	Layers:
	-	`sha256:a2baf8ed1bce68a4f36469f3537f12b9e5bebc860ab4aac0954714901595c575`  
		Last Modified: Wed, 26 Feb 2020 00:49:08 GMT  
		Size: 45.2 MB (45232848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a58b9c529db9ec73f2bb8ba3f678b389c4df7bdb3ff1083ebf516aee839533b2`  
		Last Modified: Wed, 26 Feb 2020 04:49:17 GMT  
		Size: 10.3 MB (10325927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d9d2deeb51ba62efa7f9206911520eae29fdd6a401851f5f400f881ef0fbc8`  
		Last Modified: Wed, 26 Feb 2020 04:49:16 GMT  
		Size: 4.4 MB (4372671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:945d494eee6f349916e86f798c51b0ee9e6c3e769f797eb840c23ce5857bed41`  
		Last Modified: Wed, 26 Feb 2020 04:49:30 GMT  
		Size: 50.5 MB (50500268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32172ae2ff63a2a428c16879a62e110ef908cf42a10b9fc15275a5bc9bb8707c`  
		Last Modified: Wed, 26 Feb 2020 04:50:00 GMT  
		Size: 206.9 MB (206915719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3426256adde5ad69b61a00f2d57140b49b0669f9cb3d4f78a3dae6e2b3d08fe1`  
		Last Modified: Wed, 26 Feb 2020 07:29:51 GMT  
		Size: 439.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bdcc78f46e861f9eacb1cccc30c33078fec45bed0adde648df6c6d1de6e9d9a`  
		Last Modified: Wed, 26 Feb 2020 07:30:00 GMT  
		Size: 14.3 MB (14286186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
