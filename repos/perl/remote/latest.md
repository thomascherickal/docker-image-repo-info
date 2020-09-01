## `perl:latest`

```console
$ docker pull perl@sha256:ec1235dcabc36763b96252cf6481f2a52de3f1acdc754999c9bb2ff3e901c794
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `perl:latest` - linux; amd64

```console
$ docker pull perl@sha256:f02808513ee24765e854bb329fa978c12757c5bad7bd5c5196e13ef172d9c1df
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.3 MB (326346978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fad56a1e87146bb1f03756047047c1b26762ff0a3ac738f82135d90ba61f9036`
-	Default Command: `["perl5.32.0","-de0"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:33 GMT
ADD file:4b03b5f551e3fbdf47ec609712007327828f7530cc3455c43bbcdcaf449a75a9 in / 
# Tue, 04 Aug 2020 15:42:34 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:26:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:26:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 23:26:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:27:46 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 00:53:39 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 05 Aug 2020 00:53:39 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Wed, 05 Aug 2020 00:53:39 GMT
WORKDIR /usr/src/perl
# Wed, 05 Aug 2020 01:01:40 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.0.tar.xz -o perl-5.32.0.tar.xz     && echo '6f436b447cf56d22464f980fac1916e707a040e96d52172984c5d184c09b859b *perl-5.32.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.0.tar.xz -C /usr/src/perl     && rm perl-5.32.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Wed, 05 Aug 2020 01:01:40 GMT
WORKDIR /
# Wed, 05 Aug 2020 01:01:41 GMT
CMD ["perl5.32.0" "-de0"]
```

-	Layers:
	-	`sha256:d6ff36c9ec4822c9ff8953560f7ba41653b348a9c1136755e653575f58fbded7`  
		Last Modified: Tue, 04 Aug 2020 15:48:55 GMT  
		Size: 50.4 MB (50396000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c958d65b3090aefea91284d018b2a86530a3c8174b72616c4e76993c696a5797`  
		Last Modified: Tue, 04 Aug 2020 23:39:28 GMT  
		Size: 7.8 MB (7811570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edaf0a6b092f5673ec05b40edb606ce58881b2f40494251117d31805225ef064`  
		Last Modified: Tue, 04 Aug 2020 23:39:27 GMT  
		Size: 10.0 MB (9996337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80931cf6881673fd161a3fd73e8971fe4a569fd7fbb44e956d261ca58d97dfab`  
		Last Modified: Tue, 04 Aug 2020 23:39:45 GMT  
		Size: 51.8 MB (51829826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1b8aca3825e6c3b57e28c8075180f97879161dd58333de13f6b6da0f842af3`  
		Last Modified: Tue, 04 Aug 2020 23:40:24 GMT  
		Size: 192.2 MB (192243499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:812432e5d45b78c9b0872cef89601f06a4a735b8ce727523ae7be8cbb5e75824`  
		Last Modified: Wed, 05 Aug 2020 04:11:41 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7326901a09044f5af9105b3a6a5a3afaad51daae32651219189d2f52e5a73955`  
		Last Modified: Wed, 05 Aug 2020 04:11:44 GMT  
		Size: 14.1 MB (14069569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:latest` - linux; arm variant v7

```console
$ docker pull perl@sha256:7ee825cf83b13d60e27eb872ddb26e121301a62f676474d69d3d5c66916bbb00
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.4 MB (291359614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a8b3e0bb323cb41f0602bfe24f1aa2c479ced1422f809042877c7249d912ab1`
-	Default Command: `["perl5.32.0","-de0"]`

```dockerfile
# Tue, 04 Aug 2020 04:56:26 GMT
ADD file:aaf5c6340b3d662631775fa4536c2e48e9f68b6cc8d53e18fb8fd76ae41b305e in / 
# Tue, 04 Aug 2020 04:56:28 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 07:52:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 07:53:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 07:54:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 07:57:51 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 12:06:13 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 04 Aug 2020 12:06:14 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 04 Aug 2020 12:06:15 GMT
WORKDIR /usr/src/perl
# Tue, 04 Aug 2020 12:15:55 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.0.tar.xz -o perl-5.32.0.tar.xz     && echo '6f436b447cf56d22464f980fac1916e707a040e96d52172984c5d184c09b859b *perl-5.32.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.0.tar.xz -C /usr/src/perl     && rm perl-5.32.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 04 Aug 2020 12:15:57 GMT
WORKDIR /
# Tue, 04 Aug 2020 12:15:57 GMT
CMD ["perl5.32.0" "-de0"]
```

-	Layers:
	-	`sha256:e7cf402ee4b1ba67e92813d50297a082bbdbdd4d47f6aeb62f2316b81d5dc843`  
		Last Modified: Tue, 04 Aug 2020 05:04:56 GMT  
		Size: 45.9 MB (45869261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff6bd4a89fc21d80ca6924320f86708f35ddea71c7aa34a408a5b64257c764e`  
		Last Modified: Tue, 04 Aug 2020 08:25:56 GMT  
		Size: 7.1 MB (7097820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48f5852a753b7731e5d374567ae9b64e309805758f336c76d5f13bb67c94e20`  
		Last Modified: Tue, 04 Aug 2020 08:25:56 GMT  
		Size: 9.3 MB (9343353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58a93b33dd4d533cc1e04eab8045940d69cb287134aa90c982e3d248739044e`  
		Last Modified: Tue, 04 Aug 2020 08:26:25 GMT  
		Size: 47.4 MB (47355829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c3db37cc57c3bd3b819e95bf9e93e019c7170b1f799bb494232c26e8d10bc4`  
		Last Modified: Tue, 04 Aug 2020 08:27:21 GMT  
		Size: 168.5 MB (168478199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56850f92e9f7dc51421504fee58ddc077dda2b1f3d764f676e89af5ad1a6b3b8`  
		Last Modified: Tue, 04 Aug 2020 16:15:09 GMT  
		Size: 207.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08e3fda5d90e99918b7c868afc6cb80f69f09b2ccfa6106b1206e1eef768e99`  
		Last Modified: Tue, 04 Aug 2020 16:15:16 GMT  
		Size: 13.2 MB (13214945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:latest` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:cfe13a7a6e1580e5b1ccb6adf646ab2666e353fce92189a971c2c73dde7ec183
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.8 MB (316809263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74ba301d6f7778aa3f60cbffc380f6d03ee2140cb5153e2360e0bd79f102a485`
-	Default Command: `["perl5.32.0","-de0"]`

```dockerfile
# Tue, 04 Aug 2020 06:57:06 GMT
ADD file:ce999027b153d392f8a0f85e2e7a17b9279f3cf7ad0e45192378d527275f99c6 in / 
# Tue, 04 Aug 2020 06:57:08 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 11:10:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 11:10:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 11:10:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 11:12:33 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 17:52:48 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 04 Aug 2020 17:52:57 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 04 Aug 2020 17:53:01 GMT
WORKDIR /usr/src/perl
# Tue, 04 Aug 2020 18:03:19 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.0.tar.xz -o perl-5.32.0.tar.xz     && echo '6f436b447cf56d22464f980fac1916e707a040e96d52172984c5d184c09b859b *perl-5.32.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.0.tar.xz -C /usr/src/perl     && rm perl-5.32.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 04 Aug 2020 18:03:25 GMT
WORKDIR /
# Tue, 04 Aug 2020 18:03:26 GMT
CMD ["perl5.32.0" "-de0"]
```

-	Layers:
	-	`sha256:d5517ee72007172d5b814636405254dea459120ce08f85777bb287d106a6a240`  
		Last Modified: Tue, 04 Aug 2020 07:03:41 GMT  
		Size: 49.2 MB (49175491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0283897ad4463628bd259e1cbb5eb788e7df554b42ae17fc6f5d02c4a56035c2`  
		Last Modified: Tue, 04 Aug 2020 11:23:01 GMT  
		Size: 7.7 MB (7681458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3feb40d9f5fecfa098b8f7ece6c287c6fd61b114043c8b4647359120a7d943a3`  
		Last Modified: Tue, 04 Aug 2020 11:23:02 GMT  
		Size: 10.0 MB (9983917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86b5fabb62f79acd92186da3c02d23bd8c15d79603a700959b582bd9e62854c`  
		Last Modified: Tue, 04 Aug 2020 11:23:28 GMT  
		Size: 52.2 MB (52163657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:096dd1bf4833a31fe4195d0bed170525a91c3b2d0fcbb6e3af05376c91ae06fb`  
		Last Modified: Tue, 04 Aug 2020 11:24:27 GMT  
		Size: 183.8 MB (183788664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b02361e629bcaff58b8749751d4e1944cc5538fd249085dd1e59ba779cb1bf2`  
		Last Modified: Tue, 04 Aug 2020 22:35:16 GMT  
		Size: 205.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9bb039e6d39cca8f4bb5d12ee9552ecf42dbb5d1ccf726b5726422534688593`  
		Last Modified: Tue, 04 Aug 2020 22:35:27 GMT  
		Size: 14.0 MB (14015871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:latest` - linux; 386

```console
$ docker pull perl@sha256:c566d5f1269a5c2a5b8d8aab8a36706e126eaf0a5737460b58a701cf96a1e863
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.3 MB (335284759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6dad86423b14ff587733e703c330c345d400f13d876b0f8fcc7df4ed6e519da6`
-	Default Command: `["perl5.32.0","-de0"]`

```dockerfile
# Tue, 04 Aug 2020 03:37:21 GMT
ADD file:e8aac36755acd0915e9f9bae82fc8fcd0bbc3911ca4a5a40e104b2a4ebce44da in / 
# Tue, 04 Aug 2020 03:37:21 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 08:06:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 08:06:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 08:07:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Aug 2020 23:41:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 05:21:44 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 01 Sep 2020 05:21:44 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 01 Sep 2020 05:21:45 GMT
WORKDIR /usr/src/perl
# Tue, 01 Sep 2020 05:35:55 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.0.tar.xz -o perl-5.32.0.tar.xz     && echo '6f436b447cf56d22464f980fac1916e707a040e96d52172984c5d184c09b859b *perl-5.32.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.0.tar.xz -C /usr/src/perl     && rm perl-5.32.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 01 Sep 2020 05:35:56 GMT
WORKDIR /
# Tue, 01 Sep 2020 05:35:56 GMT
CMD ["perl5.32.0" "-de0"]
```

-	Layers:
	-	`sha256:b19305c328889ec69ec0d76e403c2cbc4603e5f27213a0e4d5f6597feefcf6e1`  
		Last Modified: Tue, 04 Aug 2020 03:42:18 GMT  
		Size: 51.2 MB (51158828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d9322a54f80129fd5cd69b7be3ac6ba44b9a0268afcbd10876508eb0f9264c`  
		Last Modified: Tue, 04 Aug 2020 08:25:50 GMT  
		Size: 8.0 MB (7981119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:571a7f32100867eafa619a9265416538a2a374b88219902c6270b6f023d19061`  
		Last Modified: Tue, 04 Aug 2020 08:25:51 GMT  
		Size: 10.3 MB (10338494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3ea04987808c324433cf4b1b813ccf6528f9bf603422fbee2725c1e4018eb8`  
		Last Modified: Tue, 04 Aug 2020 08:26:25 GMT  
		Size: 53.4 MB (53433408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f5bab8ea37e9aaec5e57e6ad1fec0818250ec45b7449995899fd030ba8e2b7`  
		Last Modified: Mon, 31 Aug 2020 23:50:11 GMT  
		Size: 198.8 MB (198807590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3122fbaea539879bcb07402eb92e722022d56044e045bd1d481db06cabadba`  
		Last Modified: Tue, 01 Sep 2020 08:08:13 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a08401973ec2d16e106cc61f7c58e60017d6f381dd9a6e9d012f670bd95678`  
		Last Modified: Tue, 01 Sep 2020 08:08:22 GMT  
		Size: 13.6 MB (13565142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:latest` - linux; ppc64le

```console
$ docker pull perl@sha256:ac0c0ed8adf695218cf53214474fda275fc2c88e2eaa21a086d9863c815114d3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **347.8 MB (347758295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb6eb3a596abd77f6cb6fae23680dce6a4b1cc36b599400de86240b1c91c4b28`
-	Default Command: `["perl5.32.0","-de0"]`

```dockerfile
# Tue, 04 Aug 2020 04:44:59 GMT
ADD file:7cc5195cf323fbee8e0c74a76984198dca35599ab18b1ecc5639fa719326bd35 in / 
# Tue, 04 Aug 2020 04:45:05 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 07:12:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 07:13:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 07:15:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 07:24:41 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 13:52:11 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 04 Aug 2020 13:52:14 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 04 Aug 2020 13:52:18 GMT
WORKDIR /usr/src/perl
# Tue, 04 Aug 2020 13:58:49 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.0.tar.xz -o perl-5.32.0.tar.xz     && echo '6f436b447cf56d22464f980fac1916e707a040e96d52172984c5d184c09b859b *perl-5.32.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.0.tar.xz -C /usr/src/perl     && rm perl-5.32.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 04 Aug 2020 13:58:52 GMT
WORKDIR /
# Tue, 04 Aug 2020 13:58:56 GMT
CMD ["perl5.32.0" "-de0"]
```

-	Layers:
	-	`sha256:db4e2d8d5901311f959f0a2271be587f91ea2826238f2a17347ffab142413f53`  
		Last Modified: Tue, 04 Aug 2020 04:52:50 GMT  
		Size: 54.1 MB (54142497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe2d012519ce68bcd2414835909fb4784fd4eb5bea2c88916fdea0c661c872e`  
		Last Modified: Tue, 04 Aug 2020 07:45:05 GMT  
		Size: 8.3 MB (8254809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d8f1d1f9197bf1817cda35a89da9bd2544ceb7bf0c7b92fba5977ab2b2ab9e6`  
		Last Modified: Tue, 04 Aug 2020 07:45:07 GMT  
		Size: 10.7 MB (10727103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1301750ffb48db80c63d6d21adae9f88f4f4aaf4f561ab3512287683a04c04c0`  
		Last Modified: Tue, 04 Aug 2020 07:45:33 GMT  
		Size: 57.5 MB (57455994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc2bbaa0b6108d40a45e95e74b910c3c7ac2fbfc0622823fac1c0c472800ebdc`  
		Last Modified: Tue, 04 Aug 2020 07:46:22 GMT  
		Size: 203.1 MB (203075211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d0856e290ffe800008184da015b5e9a6182345f10658e4a956e3a56cb549fe`  
		Last Modified: Tue, 04 Aug 2020 15:33:32 GMT  
		Size: 204.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc36ea97f74dadaabfeb60086ecaf33266d34bd95277846ddb62c0470dbb6579`  
		Last Modified: Tue, 04 Aug 2020 15:33:38 GMT  
		Size: 14.1 MB (14102477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:latest` - linux; s390x

```console
$ docker pull perl@sha256:8277d5b94c6ae903e18ebd12d428579c18d2762e420a5803485643546a027149
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.8 MB (308834467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:736fa6d5857afcdcace3a6cf6f9e0be557d7d13d47c595d78ab795137b64b933`
-	Default Command: `["perl5.32.0","-de0"]`

```dockerfile
# Tue, 04 Aug 2020 01:17:02 GMT
ADD file:07519836baf21317676c799c0905c76bf767fe8caa1fa718c0dfe0a152577ee8 in / 
# Tue, 04 Aug 2020 01:17:04 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 02:22:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 02:22:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 02:22:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Aug 2020 23:46:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 07:01:10 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 01 Sep 2020 07:01:11 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 01 Sep 2020 07:01:12 GMT
WORKDIR /usr/src/perl
# Tue, 01 Sep 2020 07:06:12 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.0.tar.xz -o perl-5.32.0.tar.xz     && echo '6f436b447cf56d22464f980fac1916e707a040e96d52172984c5d184c09b859b *perl-5.32.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.0.tar.xz -C /usr/src/perl     && rm perl-5.32.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 01 Sep 2020 07:06:13 GMT
WORKDIR /
# Tue, 01 Sep 2020 07:06:13 GMT
CMD ["perl5.32.0" "-de0"]
```

-	Layers:
	-	`sha256:f2b199a6d9adcfa5f879ec8042306ab2f919623f8018d0d7a6f4e9dade5e1a71`  
		Last Modified: Tue, 04 Aug 2020 01:19:47 GMT  
		Size: 49.0 MB (48966275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5615f13ce6c82698ac5df02b39113e3a8949db1a7a7f7f5d07c9265ee15b79d0`  
		Last Modified: Tue, 04 Aug 2020 02:28:11 GMT  
		Size: 7.4 MB (7385167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ffecb808bd421be3db88ff08f67b19f28c1ffe0d4c157be3fcff3360f527bc`  
		Last Modified: Tue, 04 Aug 2020 02:28:11 GMT  
		Size: 9.9 MB (9882139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e2ce491a55134d5e4118405670fcc19b140898dc8ac62156e47a49f52e9f2d`  
		Last Modified: Tue, 04 Aug 2020 02:28:29 GMT  
		Size: 51.4 MB (51379924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd4c01fb5114b8979db673af5df15b834739b58c5a9486010011d3da89780a8`  
		Last Modified: Mon, 31 Aug 2020 23:51:50 GMT  
		Size: 176.8 MB (176814752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:789ebe801ef75183d79e8da868f6d0fc421fd54147ed905e4ee701758627367d`  
		Last Modified: Tue, 01 Sep 2020 07:35:42 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b5d1a6b38dc1260a3646bb3b96ea196b2a443e926c3275e3460a8ecda7aad9`  
		Last Modified: Tue, 01 Sep 2020 07:35:45 GMT  
		Size: 14.4 MB (14406007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
