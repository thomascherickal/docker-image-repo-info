## `perl:threaded`

```console
$ docker pull perl@sha256:9196c4166909c9f63ad66aec5ac46700aa28b34ce401d193c2b6d5b85dfdc267
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
$ docker pull perl@sha256:76e9c6835656ae6a7d4f79f9d71ecd6877603ffff68905ccb6ca51e4825bddae
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.0 MB (325995739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce5e74e2bd9f15c9f0e0080c5c29341696111e76c2a592b9bfe3fc937bcbdc39`
-	Default Command: `["perl5.30.1","-de0"]`

```dockerfile
# Wed, 26 Feb 2020 00:37:07 GMT
ADD file:e05e45c33042db4ec7f71a5952d65ee8cb3786dcd76fa7a990f48a2def1344e2 in / 
# Wed, 26 Feb 2020 00:37:07 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 01:06:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 01:06:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Feb 2020 01:06:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 01:07:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 07:05:10 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 26 Feb 2020 07:05:10 GMT
COPY file:15650064fd29deac721f0aa084ddb3d41db77b78e2907775e257bd67e116ade4 in /usr/src/perl/ 
# Wed, 26 Feb 2020 07:05:11 GMT
WORKDIR /usr/src/perl
# Wed, 26 Feb 2020 08:11:08 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.30.1.tar.xz -o perl-5.30.1.tar.xz     && echo '7336cd3ed0535eb61b76a71350effcfa7c88b44faf37d64d70952ced5d38cd35 *perl-5.30.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.30.1.tar.xz -C /usr/src/perl     && rm perl-5.30.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Wed, 26 Feb 2020 08:11:09 GMT
WORKDIR /
# Wed, 26 Feb 2020 08:11:09 GMT
CMD ["perl5.30.1" "-de0"]
```

-	Layers:
	-	`sha256:50e431f790939a2f924af65084cc9d39c3d3fb9ad2d57d183b7eadf86ea46992`  
		Last Modified: Wed, 26 Feb 2020 00:44:04 GMT  
		Size: 50.4 MB (50381971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8c6d374ea51e3dd671f71b28d025a7794ebea181b00838987d0b4d8a51372f`  
		Last Modified: Wed, 26 Feb 2020 01:20:25 GMT  
		Size: 7.8 MB (7812140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85513200d847a64a6e8f2cb714e2169f559b24b7736c586ff7b9aaedf71f410`  
		Last Modified: Wed, 26 Feb 2020 01:20:25 GMT  
		Size: 10.0 MB (9996282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55769680e8277a4ff083d05f0993d1483b3d26b93a8814cf3c6f04fe5975ffa0`  
		Last Modified: Wed, 26 Feb 2020 01:20:44 GMT  
		Size: 51.8 MB (51790538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5e195d50b880fcf8dc81f38d743c8b087777b3bfe0f27cd4ecdda513f5d20b9`  
		Last Modified: Wed, 26 Feb 2020 01:21:25 GMT  
		Size: 192.2 MB (192161449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbdc17ec6b115dd8a98124a8fdb260e2121a0a9c8fc27a25a2716b4099f61f66`  
		Last Modified: Wed, 26 Feb 2020 11:42:44 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54862660b722eba6b03a28e1f949c7ef83a81d0dea0112edf6ef8702b79caad`  
		Last Modified: Wed, 26 Feb 2020 11:43:30 GMT  
		Size: 13.9 MB (13852947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded` - linux; arm variant v7

```console
$ docker pull perl@sha256:f41f89d7ad897b3e5e7461690c9008f6edec48bfcfd98f6f109d4150604f7e49
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.0 MB (290980054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:002263cdcacc70bed7f8c99860c64b641cdfc3f8c5ed8cce66a6091d7ca52fe7`
-	Default Command: `["perl5.30.2","-de0"]`

```dockerfile
# Wed, 26 Feb 2020 00:50:58 GMT
ADD file:38fdfcc3155e437ce162aa0ed9dcdc5893b8145e2f3ede2858ed2187d79bf718 in / 
# Wed, 26 Feb 2020 00:51:08 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 02:11:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 02:11:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Feb 2020 02:12:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 02:14:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 04:38:43 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 26 Feb 2020 04:38:44 GMT
COPY file:15650064fd29deac721f0aa084ddb3d41db77b78e2907775e257bd67e116ade4 in /usr/src/perl/ 
# Wed, 26 Feb 2020 04:38:45 GMT
WORKDIR /usr/src/perl
# Tue, 17 Mar 2020 17:45:32 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.30.2.tar.xz -o perl-5.30.2.tar.xz     && echo 'a1aa88bd6fbbdc2e82938afbb76c408b0ea847317737b712dc196cc7907a5259 *perl-5.30.2.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.30.2.tar.xz -C /usr/src/perl     && rm perl-5.30.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 17 Mar 2020 17:45:33 GMT
WORKDIR /
# Tue, 17 Mar 2020 17:45:33 GMT
CMD ["perl5.30.2" "-de0"]
```

-	Layers:
	-	`sha256:3182cf45068cd9734abd8e38dedbb9930ede35ee8c11376ca2684e86f9a1aa85`  
		Last Modified: Wed, 26 Feb 2020 01:07:03 GMT  
		Size: 45.9 MB (45862691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b727ab99a6a790544e023dbba8625605266dd84b3a69acaa541144ad632f4ba`  
		Last Modified: Wed, 26 Feb 2020 02:33:37 GMT  
		Size: 7.1 MB (7096560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab9435f7cf0c46bc6621020fd229e7de8baa61f71059cb9a34b9f681caed9aa`  
		Last Modified: Wed, 26 Feb 2020 02:33:38 GMT  
		Size: 9.3 MB (9343152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2ad791c8431e9b6624239d0b1fee2523df27584a263ec1d8d525201bb44087`  
		Last Modified: Wed, 26 Feb 2020 02:34:01 GMT  
		Size: 47.3 MB (47315030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1406a1731086e1f62b02230770f70586935a96a1573aa2875186b1ad4c4fb91`  
		Last Modified: Wed, 26 Feb 2020 02:34:50 GMT  
		Size: 168.4 MB (168384180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f7f7220a5f91b75f9df3f3b2fe39099d4ea005dbe2cfb4f44a5365a0e9463d`  
		Last Modified: Wed, 26 Feb 2020 08:26:43 GMT  
		Size: 442.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604a1312381b1a06fe8c2be1748a2039293b4b66733acd706fed29c78aae959a`  
		Last Modified: Tue, 17 Mar 2020 20:32:25 GMT  
		Size: 13.0 MB (12977999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:408eacc2d8278d5e1c6a81a1143602f4646b3cc203ce4ff80cacaef768f5ed00
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.4 MB (316442223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:866fd4c8aab4a519fad73ad34ff93028554a77c7215d931dcfcdabf81049ae9c`
-	Default Command: `["perl5.30.2","-de0"]`

```dockerfile
# Wed, 26 Feb 2020 00:46:17 GMT
ADD file:e3320653f0d517a6181aa46fb47407790018e2d8dee590005ffdbee3d04f72d4 in / 
# Wed, 26 Feb 2020 00:46:19 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 03:50:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 03:50:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Feb 2020 03:51:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 03:53:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 08:03:42 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 26 Feb 2020 08:03:43 GMT
COPY file:15650064fd29deac721f0aa084ddb3d41db77b78e2907775e257bd67e116ade4 in /usr/src/perl/ 
# Wed, 26 Feb 2020 08:03:46 GMT
WORKDIR /usr/src/perl
# Tue, 17 Mar 2020 17:27:44 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.30.2.tar.xz -o perl-5.30.2.tar.xz     && echo 'a1aa88bd6fbbdc2e82938afbb76c408b0ea847317737b712dc196cc7907a5259 *perl-5.30.2.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.30.2.tar.xz -C /usr/src/perl     && rm perl-5.30.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 17 Mar 2020 17:27:45 GMT
WORKDIR /
# Tue, 17 Mar 2020 17:27:46 GMT
CMD ["perl5.30.2" "-de0"]
```

-	Layers:
	-	`sha256:77b067f4ec14d48dbc8cd83b7a46fbb5f21fe01ea8911db256cc0168a30c1f5b`  
		Last Modified: Wed, 26 Feb 2020 00:55:50 GMT  
		Size: 49.2 MB (49169974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:194f1ca8932d9ee1727375561698745fa548546f609956c4aca9fed0b48d41a1`  
		Last Modified: Wed, 26 Feb 2020 04:05:25 GMT  
		Size: 7.7 MB (7681467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88425686f799f708ae776f78a6d01c179a52f55fc5b32de874db3c4ace2dd156`  
		Last Modified: Wed, 26 Feb 2020 04:05:25 GMT  
		Size: 10.0 MB (9983767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c349f2c39d405d81a454ff62bdd8753ad71aeb8e8c1e300f3d7d19cd78eaced`  
		Last Modified: Wed, 26 Feb 2020 04:05:53 GMT  
		Size: 52.1 MB (52102940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8882fd3db1fac7e11ca7ef46b66e332293d45b8454f531202a424b88c61b57`  
		Last Modified: Wed, 26 Feb 2020 04:06:48 GMT  
		Size: 183.7 MB (183711106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35de08a405c029931e062bcdc8ea88731665f61f8c4ad6545a0a7fc6b90149a8`  
		Last Modified: Wed, 26 Feb 2020 11:49:14 GMT  
		Size: 442.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90d9e50023f736fad2f715e89315b37427a20a8549d46d4eef78593482624773`  
		Last Modified: Tue, 17 Mar 2020 20:18:37 GMT  
		Size: 13.8 MB (13792527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded` - linux; 386

```console
$ docker pull perl@sha256:91e3d1b3f479629837ec6bc6d4212eb67639929deeecfec75f8dfe39bb84cded
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.9 MB (334949634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4b8d70d98514a1e10f13c030964c07d6831274b396489c9e0004f4e9a11fb23`
-	Default Command: `["perl5.30.2","-de0"]`

```dockerfile
# Wed, 26 Feb 2020 00:31:58 GMT
ADD file:1deff975480520310bf2c8d3708554d98c696f82689f0b67f9a834217c861803 in / 
# Wed, 26 Feb 2020 00:31:59 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 01:07:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 01:07:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Feb 2020 01:08:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 01:09:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 05:40:48 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 26 Feb 2020 05:40:49 GMT
COPY file:15650064fd29deac721f0aa084ddb3d41db77b78e2907775e257bd67e116ade4 in /usr/src/perl/ 
# Wed, 26 Feb 2020 05:40:49 GMT
WORKDIR /usr/src/perl
# Tue, 17 Mar 2020 17:26:02 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.30.2.tar.xz -o perl-5.30.2.tar.xz     && echo 'a1aa88bd6fbbdc2e82938afbb76c408b0ea847317737b712dc196cc7907a5259 *perl-5.30.2.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.30.2.tar.xz -C /usr/src/perl     && rm perl-5.30.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 17 Mar 2020 17:26:03 GMT
WORKDIR /
# Tue, 17 Mar 2020 17:26:03 GMT
CMD ["perl5.30.2" "-de0"]
```

-	Layers:
	-	`sha256:9450e7c48681b3ba36935d4e7d891b4b180d4d223a6c938faacb41402857ebd3`  
		Last Modified: Wed, 26 Feb 2020 00:38:12 GMT  
		Size: 51.1 MB (51146129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3b9049fe76610ee534524c2087947a0c92f9d674f7395a2031161e4e448a57`  
		Last Modified: Wed, 26 Feb 2020 01:27:14 GMT  
		Size: 8.0 MB (7981680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e618476b0d787bc3028ca73062991dd8c2c5c71d93e2932eb7f14257541bc005`  
		Last Modified: Wed, 26 Feb 2020 01:27:15 GMT  
		Size: 10.3 MB (10338439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd3ac0f3869d874323567fd1fdb72f8976b62d2dd8d3c9761ab065b2426a6d9`  
		Last Modified: Wed, 26 Feb 2020 01:27:39 GMT  
		Size: 53.4 MB (53382038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63dbefcf2d3603f7c2cb004f59a7355633f1ea341bcdab4852ed9de22ae649f8`  
		Last Modified: Wed, 26 Feb 2020 01:28:36 GMT  
		Size: 198.7 MB (198715134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f3898c41dd25532f1d0269fd086524a5a00478c479484a2e20051beb9d48a1`  
		Last Modified: Wed, 26 Feb 2020 10:45:55 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a77363f19a4d0f5c9c75a10c00ff69e60b3e3b6a405b697b02ddb82a765ff8`  
		Last Modified: Tue, 17 Mar 2020 21:43:58 GMT  
		Size: 13.4 MB (13385802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded` - linux; ppc64le

```console
$ docker pull perl@sha256:9c3d3428cd843a991ba5971e74a8529cdf9de8df25438ae18d1193013c822393
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **347.4 MB (347432204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f517de6cb9867230d67b3edf2547b053c9347f83a40ea70c095951c1b9f16cd`
-	Default Command: `["perl5.30.2","-de0"]`

```dockerfile
# Wed, 26 Feb 2020 01:30:27 GMT
ADD file:b58865b3fd36d440998ef82e567179a9cd6b9ce0343d5e5a15a0b4f856f211c7 in / 
# Wed, 26 Feb 2020 01:30:35 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 08:02:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 08:03:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Feb 2020 08:05:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 08:15:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 09:30:45 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 26 Feb 2020 09:30:47 GMT
COPY file:15650064fd29deac721f0aa084ddb3d41db77b78e2907775e257bd67e116ade4 in /usr/src/perl/ 
# Wed, 26 Feb 2020 09:30:53 GMT
WORKDIR /usr/src/perl
# Tue, 17 Mar 2020 18:00:06 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.30.2.tar.xz -o perl-5.30.2.tar.xz     && echo 'a1aa88bd6fbbdc2e82938afbb76c408b0ea847317737b712dc196cc7907a5259 *perl-5.30.2.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.30.2.tar.xz -C /usr/src/perl     && rm perl-5.30.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 17 Mar 2020 18:00:17 GMT
WORKDIR /
# Tue, 17 Mar 2020 18:00:24 GMT
CMD ["perl5.30.2" "-de0"]
```

-	Layers:
	-	`sha256:928614537d6dedbdf79cc24c5c56bf98c3ed88f9d91a9ec1105d2a133611b0fd`  
		Last Modified: Wed, 26 Feb 2020 01:49:54 GMT  
		Size: 54.1 MB (54138444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f499895181a6ad2e0a4c9fdaf499ffa2704adc3eb69595e994d38b563c6000e8`  
		Last Modified: Wed, 26 Feb 2020 08:48:45 GMT  
		Size: 8.3 MB (8252620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:887a1613f8e8808f8cdb481db1614b9d79f0dc57f17235b478bd4c6c95849e29`  
		Last Modified: Wed, 26 Feb 2020 08:48:45 GMT  
		Size: 10.7 MB (10727256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6753b4bd70abfe94b10e69e3b643900c4f2e72961c4db6310963cd4c21303d5c`  
		Last Modified: Wed, 26 Feb 2020 08:49:40 GMT  
		Size: 57.4 MB (57392075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87e860c31973cd8a76230d957022cb21f08103d2bca9009d41efc403d6f34fb3`  
		Last Modified: Wed, 26 Feb 2020 08:51:34 GMT  
		Size: 203.0 MB (202975746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fda2af534972ad175cd3ebe37568b97b6f8c15153eb0de7b160fcf246a23301`  
		Last Modified: Wed, 26 Feb 2020 12:37:52 GMT  
		Size: 442.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f30a709aa092ce97625b2190d9734dde91c86631c6bea7f0dfe02ae333acca7`  
		Last Modified: Tue, 17 Mar 2020 20:45:23 GMT  
		Size: 13.9 MB (13945621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded` - linux; s390x

```console
$ docker pull perl@sha256:bf9c9ef8706baabfc0ad898f2c5e7c9227a2ecec1ac5e5298955c2cc720de5c4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.5 MB (308481404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0da85b7f6bd9e4397a76366c627e782c713154305722076e71f08e4ec8243bd`
-	Default Command: `["perl5.30.2","-de0"]`

```dockerfile
# Wed, 26 Feb 2020 00:42:32 GMT
ADD file:80536bfff518f6b425ad359b86a124f79ccdc82deb3e648f1746a7c87a1fcad0 in / 
# Wed, 26 Feb 2020 00:42:35 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 04:33:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 04:33:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Feb 2020 04:34:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 04:36:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 05:04:33 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 26 Feb 2020 05:04:33 GMT
COPY file:15650064fd29deac721f0aa084ddb3d41db77b78e2907775e257bd67e116ade4 in /usr/src/perl/ 
# Wed, 26 Feb 2020 05:04:34 GMT
WORKDIR /usr/src/perl
# Tue, 17 Mar 2020 17:04:49 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.30.2.tar.xz -o perl-5.30.2.tar.xz     && echo 'a1aa88bd6fbbdc2e82938afbb76c408b0ea847317737b712dc196cc7907a5259 *perl-5.30.2.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.30.2.tar.xz -C /usr/src/perl     && rm perl-5.30.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 17 Mar 2020 17:04:51 GMT
WORKDIR /
# Tue, 17 Mar 2020 17:04:51 GMT
CMD ["perl5.30.2" "-de0"]
```

-	Layers:
	-	`sha256:0a3603da42bb9e22573006a7f894b198954caeab529e2e041660e12c4fe62462`  
		Last Modified: Wed, 26 Feb 2020 00:47:26 GMT  
		Size: 49.0 MB (48958029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a7b142236e4c473f4fd19a0485f74364510f658dc999627e6c41f4684a50d5`  
		Last Modified: Wed, 26 Feb 2020 04:47:32 GMT  
		Size: 7.4 MB (7382213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f2c5965845a6f2fd1bfaa3a4814a17655d46330b5f60ed861daaa390d5b82a2`  
		Last Modified: Wed, 26 Feb 2020 04:47:37 GMT  
		Size: 9.9 MB (9882220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:942858cf91c54d2d1efa88f24491ba2b93cd15ed968d4f5e193c5e26ca4236e1`  
		Last Modified: Wed, 26 Feb 2020 04:47:51 GMT  
		Size: 51.3 MB (51327256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c253e6eac0df273f38b2ed2fb694f11e1a9538ec03a3d1456a34bec00f8f528d`  
		Last Modified: Wed, 26 Feb 2020 04:48:17 GMT  
		Size: 176.7 MB (176729778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4da9380745e2853f4b486e3c5f26cc06e48b9b5d4ab0a141e0f28ec2ea438f8e`  
		Last Modified: Wed, 26 Feb 2020 07:29:30 GMT  
		Size: 440.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd37931d1f2c41aef1314b2d91ee15e457b48bcfdafe5a2a632fee8ffda31405`  
		Last Modified: Tue, 17 Mar 2020 18:33:42 GMT  
		Size: 14.2 MB (14201468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
