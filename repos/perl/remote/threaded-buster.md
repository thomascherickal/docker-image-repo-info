## `perl:threaded-buster`

```console
$ docker pull perl@sha256:82aa6b143f2f996abce14c957f546755b3890d5b095ab3c710b3432d4b7c2f08
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

### `perl:threaded-buster` - linux; amd64

```console
$ docker pull perl@sha256:c515e84fe7075f9d9dfd5484c8a589122d518a5cd852a5d98cb41e9d367b8c23
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.0 MB (326994134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e486b8da18f35fb7fc61697b036f150771acdeff5bd0c66cd7cd5ccdfec66cac`
-	Default Command: `["perl5.34.1","-de0"]`

```dockerfile
# Sat, 28 May 2022 01:20:32 GMT
ADD file:5c5cde050dbdbd5c7c0d9c723f436d37ab4a8b1a498647a719771eccce99d9cb in / 
# Sat, 28 May 2022 01:20:33 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:42:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:42:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 May 2022 02:42:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:43:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 06:15:44 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 28 May 2022 06:15:45 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Sat, 28 May 2022 06:15:45 GMT
WORKDIR /usr/src/perl
# Sat, 28 May 2022 06:38:23 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.1.tar.xz -o perl-5.34.1.tar.xz     && echo '6d52cf833ff1af27bb5e986870a2c30cec73c044b41e3458cd991f94374039f7 *perl-5.34.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.1.tar.xz -C /usr/src/perl     && rm perl-5.34.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Sat, 28 May 2022 06:38:23 GMT
WORKDIR /
# Sat, 28 May 2022 06:38:23 GMT
CMD ["perl5.34.1" "-de0"]
```

-	Layers:
	-	`sha256:982cba7e471c6d3ce96014cf58b2e4e115a525e60da2e1e08716818f2c057a6b`  
		Last Modified: Sat, 28 May 2022 01:25:39 GMT  
		Size: 50.4 MB (50440422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02d86f59850f3e13d394072350625a8526b912af24b3bfc0e50e9a8862a79d0`  
		Last Modified: Sat, 28 May 2022 02:50:21 GMT  
		Size: 7.9 MB (7856653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b047e8f2e47bdf998a952572ae5e9d64edf8e29b716be0ee50a15e6d21cb2ce`  
		Last Modified: Sat, 28 May 2022 02:50:21 GMT  
		Size: 10.0 MB (9997224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478cfe935c2fb922eb2a95131ad8a2f1e6ff472bbdecdf94709edc3a85f74dfd`  
		Last Modified: Sat, 28 May 2022 02:50:38 GMT  
		Size: 51.8 MB (51843777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9044b155d8ec2ce83fdaefff4a4514dda53e8012b3d5aea2d0f182aeddc08dd`  
		Last Modified: Sat, 28 May 2022 02:51:18 GMT  
		Size: 192.5 MB (192488821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638a3053fb1e1362205caeba0c1f654add2314c316214c67121652aa4b4f6696`  
		Last Modified: Sat, 28 May 2022 08:01:46 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef41fba0dc92141cabe8afd83f27f74cf514248bf13a3b99f4bd8325deece5aa`  
		Last Modified: Sat, 28 May 2022 08:03:19 GMT  
		Size: 14.4 MB (14367038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded-buster` - linux; arm variant v5

```console
$ docker pull perl@sha256:e27df0d45678f399e44cb6c20771304dd3e180c02bc9b56c79405fe97634b68f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.9 MB (299918996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e601c97c0bbce2fb0095ff0203b3c8d7d7095e7a48e3de4fca2a156bf404b06c`
-	Default Command: `["perl5.34.1","-de0"]`

```dockerfile
# Sat, 28 May 2022 02:03:32 GMT
ADD file:ad4ce97f6ea5c59c2f067ac3448d897881ae301cb606e52556637f74cac09774 in / 
# Sat, 28 May 2022 02:03:33 GMT
CMD ["bash"]
# Sat, 28 May 2022 03:10:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 03:11:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 May 2022 03:12:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 03:14:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 04:31:29 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 28 May 2022 04:31:29 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Sat, 28 May 2022 04:31:30 GMT
WORKDIR /usr/src/perl
# Sat, 28 May 2022 05:34:39 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.1.tar.xz -o perl-5.34.1.tar.xz     && echo '6d52cf833ff1af27bb5e986870a2c30cec73c044b41e3458cd991f94374039f7 *perl-5.34.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.1.tar.xz -C /usr/src/perl     && rm perl-5.34.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Sat, 28 May 2022 05:34:40 GMT
WORKDIR /
# Sat, 28 May 2022 05:34:40 GMT
CMD ["perl5.34.1" "-de0"]
```

-	Layers:
	-	`sha256:ec27c4ead5d8a5ae35fd4bad58cadacd3d006bed1911fd9b07b5e4f74921f7c9`  
		Last Modified: Sat, 28 May 2022 02:19:24 GMT  
		Size: 48.2 MB (48160631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a992114821be2e9710384caf39f14081084f800a2696a444f4ccbb0b1871735b`  
		Last Modified: Sat, 28 May 2022 03:33:34 GMT  
		Size: 7.4 MB (7400831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07ea5e22b64ba119dfad12a9075a671c03b7ef047af4ba61bc5fd78cd2a0982`  
		Last Modified: Sat, 28 May 2022 03:33:35 GMT  
		Size: 9.7 MB (9687617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c1044d72ac1d1a1dae001eae9012d7d0f660f5a0ce319794ab546237ac3803`  
		Last Modified: Sat, 28 May 2022 03:34:20 GMT  
		Size: 49.6 MB (49583647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff189f2617675f66495c8020d53c024610dd37b6738c0c2cf601d6a9f95c187`  
		Last Modified: Sat, 28 May 2022 03:36:12 GMT  
		Size: 171.4 MB (171424836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcaf76f8af80d87613e81578706b128205da6f7bce6a9d32cf8aea08467a9e6d`  
		Last Modified: Sat, 28 May 2022 09:26:53 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3078eb30c2fdec8356a58c7c7e1436e9dd6811fb615e694290762a91ae03036f`  
		Last Modified: Sat, 28 May 2022 09:29:43 GMT  
		Size: 13.7 MB (13661232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded-buster` - linux; arm variant v7

```console
$ docker pull perl@sha256:eab9d44e88a8a8f92a99790b138f38c3602ca6f0891626833cdc5b9683b9cf23
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291920388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4008df562fbd149e52fc244e5dba4468ff2a7c01fa79d72a3a5a2fbced1b63ca`
-	Default Command: `["perl5.34.1","-de0"]`

```dockerfile
# Sat, 28 May 2022 01:00:18 GMT
ADD file:3c8ac0c219015f8fbf065e01216d362016d6068cb4e73ea6f0a56893c235a2a7 in / 
# Sat, 28 May 2022 01:00:20 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:46:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:46:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 May 2022 02:47:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:49:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 12:56:28 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 28 May 2022 12:56:28 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Sat, 28 May 2022 12:56:29 GMT
WORKDIR /usr/src/perl
# Sat, 28 May 2022 13:55:01 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.1.tar.xz -o perl-5.34.1.tar.xz     && echo '6d52cf833ff1af27bb5e986870a2c30cec73c044b41e3458cd991f94374039f7 *perl-5.34.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.1.tar.xz -C /usr/src/perl     && rm perl-5.34.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Sat, 28 May 2022 13:55:02 GMT
WORKDIR /
# Sat, 28 May 2022 13:55:02 GMT
CMD ["perl5.34.1" "-de0"]
```

-	Layers:
	-	`sha256:59fe0b97900eb1b641ad94d8d8f3bd9dbff0472e481c4c4c38f2372ef790900a`  
		Last Modified: Sat, 28 May 2022 01:16:20 GMT  
		Size: 45.9 MB (45915564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49649b4a05bcb1345df6dfa9a17fe8f7e713c3a3ff8df5a44f32e7bd74df8bfe`  
		Last Modified: Sat, 28 May 2022 03:11:59 GMT  
		Size: 7.1 MB (7145382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03cd2dac771a38a2c51428234f8ad25ae6aa1f7b60d2497c96d251b5fafc88d4`  
		Last Modified: Sat, 28 May 2022 03:11:59 GMT  
		Size: 9.3 MB (9343880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a6a17283b05e5d4fc6748f4fc5c19db1f90640b2e3e18d2b792a6eb338fe11`  
		Last Modified: Sat, 28 May 2022 03:12:43 GMT  
		Size: 47.4 MB (47359471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fded1003413dc57e16c2429aabba936ea5c63d4813c77598954c01d2832992fe`  
		Last Modified: Sat, 28 May 2022 03:14:30 GMT  
		Size: 168.7 MB (168685748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9704e7b200610d9dbd677d01ac63393d1e355a34caf74604e14c72039cc1bb8c`  
		Last Modified: Sat, 28 May 2022 17:32:57 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d44970614ddaa3fe6fd5540b0b1c5a2bd9dbc1998d11201c000ff5b7b1fb301`  
		Last Modified: Sat, 28 May 2022 17:35:47 GMT  
		Size: 13.5 MB (13470142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded-buster` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:dd364744a82d8491af5f2a9f2c184849b8b0339b293fc781151caa7a666e170e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.4 MB (317443732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfd7b4dfd8e0daabcc5b7c6987b1452acdcca484be4d4a4dfa7f59a67230ab6a`
-	Default Command: `["perl5.36.0","-de0"]`

```dockerfile
# Sat, 28 May 2022 00:40:49 GMT
ADD file:af879be34a7eccc177a3000eb8c45d5207bfbec108caf9be9d11c1a6620c376c in / 
# Sat, 28 May 2022 00:40:51 GMT
CMD ["bash"]
# Sat, 28 May 2022 11:07:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 11:07:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 May 2022 11:07:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 11:08:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 02:37:27 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sun, 29 May 2022 02:37:28 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Sun, 29 May 2022 02:37:29 GMT
WORKDIR /usr/src/perl
# Mon, 30 May 2022 18:14:15 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.36.0.tar.xz -o perl-5.36.0.tar.xz     && echo '0f386dccbee8e26286404b2cca144e1005be65477979beb9b1ba272d4819bcf0 *perl-5.36.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.36.0.tar.xz -C /usr/src/perl     && rm perl-5.36.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Mon, 30 May 2022 18:14:16 GMT
WORKDIR /
# Mon, 30 May 2022 18:14:17 GMT
CMD ["perl5.36.0" "-de0"]
```

-	Layers:
	-	`sha256:fadbed17b01e84815ca3018d3dc42670c3add65c67e7cc74d6bc477ae8425934`  
		Last Modified: Sat, 28 May 2022 00:47:58 GMT  
		Size: 49.2 MB (49229054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5795076bf6e9bf96da71f2e31cbe91d3c49a17f211c5b0d33e032e095c5564a5`  
		Last Modified: Sat, 28 May 2022 11:18:22 GMT  
		Size: 7.7 MB (7719823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1eda3e266fa432ba8ae8ba25a5ad2fa4c5349ef2aa244612c89f990704c5b25`  
		Last Modified: Sat, 28 May 2022 11:18:22 GMT  
		Size: 9.8 MB (9767307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64dfac45ba23f255c176d3688a882854cfc56b2e822c56e0eb0d91ecc8bad25f`  
		Last Modified: Sat, 28 May 2022 11:18:40 GMT  
		Size: 52.2 MB (52174936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbbaa341afd100d046a7984d13026b6c267e48782ed899301d8fe8702e7f721`  
		Last Modified: Sat, 28 May 2022 11:19:14 GMT  
		Size: 184.1 MB (184065328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be1c4e5981f4059152cad8e357bf84cda1eb8ba9dcfd82451ce63d4631fd7083`  
		Last Modified: Sun, 29 May 2022 03:26:52 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd4b28f7856f4a4bf214a42b2995bf4f10fd974100afd5cda8e4ed9a162df1f9`  
		Last Modified: Mon, 30 May 2022 18:33:21 GMT  
		Size: 14.5 MB (14487106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded-buster` - linux; 386

```console
$ docker pull perl@sha256:f9c884def09637d8d8d51a5c34f25243f91cffe3eefce3aadd5ecf7863dcdf8c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.9 MB (335901132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a2846d03a6d2ca08f40da98c6857dcdcd3c0d1efe83bd54e47d6ff86dbe6da7`
-	Default Command: `["perl5.36.0","-de0"]`

```dockerfile
# Sat, 28 May 2022 00:39:45 GMT
ADD file:3995ccc1e3f12a1e3f28dd818223bdc5454a7651248bfb98fae7c14961c49bba in / 
# Sat, 28 May 2022 00:39:45 GMT
CMD ["bash"]
# Sat, 28 May 2022 01:12:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 01:12:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 May 2022 01:12:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 01:14:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 04:08:33 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 28 May 2022 04:08:35 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Sat, 28 May 2022 04:08:35 GMT
WORKDIR /usr/src/perl
# Mon, 30 May 2022 18:10:56 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.36.0.tar.xz -o perl-5.36.0.tar.xz     && echo '0f386dccbee8e26286404b2cca144e1005be65477979beb9b1ba272d4819bcf0 *perl-5.36.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.36.0.tar.xz -C /usr/src/perl     && rm perl-5.36.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Mon, 30 May 2022 18:10:57 GMT
WORKDIR /
# Mon, 30 May 2022 18:10:58 GMT
CMD ["perl5.36.0" "-de0"]
```

-	Layers:
	-	`sha256:045913a916496008850e7e3b499b9acc93c72b4018eda833a11c562a6d8413b5`  
		Last Modified: Sat, 28 May 2022 00:47:08 GMT  
		Size: 51.2 MB (51204248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8b88cac678bf7c61d66ca5c565ceb244ff4764b8651c88bf3e1ae159872dd0`  
		Last Modified: Sat, 28 May 2022 01:22:38 GMT  
		Size: 8.0 MB (8022586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbc00efc59e7dbf25d25c6c5d412bc1115e1d5d65c61cb6e2c9d65b1f39faf8`  
		Last Modified: Sat, 28 May 2022 01:22:39 GMT  
		Size: 10.1 MB (10121911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7916ade5bb54b5ab127448e4b330bab4425569af949deb035ba142298784c147`  
		Last Modified: Sat, 28 May 2022 01:23:00 GMT  
		Size: 53.4 MB (53443985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde1cf8841a6c64f6fb1dce7d6d058db53618d3d3a123f80b2c158b5dfad4e7a`  
		Last Modified: Sat, 28 May 2022 01:23:35 GMT  
		Size: 199.0 MB (199012105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e369916f1808a873b114e6123309cad8d5a6ba6be97bd5ecc41337dac397e7`  
		Last Modified: Sat, 28 May 2022 06:12:02 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04261ea159f2f23483d7d843f1cd55f0613275461772749fb6b4c92e23f09ab3`  
		Last Modified: Mon, 30 May 2022 18:29:02 GMT  
		Size: 14.1 MB (14096119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded-buster` - linux; mips64le

```console
$ docker pull perl@sha256:c7991ea6c3f26d491b0668e02306fa76b896688df413411c6d81fc03b0d479f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.6 MB (310642932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11252f26619a30acd8455cb3c10c1a5f7893884dee470128de81fe8780008792`
-	Default Command: `["perl5.34.1","-de0"]`

```dockerfile
# Sat, 28 May 2022 01:11:47 GMT
ADD file:e86c610403bdbc84066b42627ffdf92eb051badd2f3d1fcc964fba096215c297 in / 
# Sat, 28 May 2022 01:11:52 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:03:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:03:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 May 2022 02:05:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:11:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 10:54:15 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sun, 29 May 2022 10:54:21 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Sun, 29 May 2022 10:54:27 GMT
WORKDIR /usr/src/perl
# Sun, 29 May 2022 12:36:50 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.1.tar.xz -o perl-5.34.1.tar.xz     && echo '6d52cf833ff1af27bb5e986870a2c30cec73c044b41e3458cd991f94374039f7 *perl-5.34.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.1.tar.xz -C /usr/src/perl     && rm perl-5.34.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Sun, 29 May 2022 12:36:57 GMT
WORKDIR /
# Sun, 29 May 2022 12:37:04 GMT
CMD ["perl5.34.1" "-de0"]
```

-	Layers:
	-	`sha256:3ab17b7e8f7dffe546de1529b66b42c5d3aaa0aca409effcd962eae29b834d3e`  
		Last Modified: Sat, 28 May 2022 01:22:17 GMT  
		Size: 49.1 MB (49073373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d8359db5e9434db65ff74cbeb6fb2a3c11834bea89c8bc0c7a81edce49d561`  
		Last Modified: Sat, 28 May 2022 02:27:30 GMT  
		Size: 7.3 MB (7272979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11e4fd36af841919e6113b762dace3a649390107a2ed9224e952e9b71cec164`  
		Last Modified: Sat, 28 May 2022 02:27:30 GMT  
		Size: 9.8 MB (9800289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4e1559e22aa070dc273c40b7ca110c836f73f219de789819c50db5abf12294`  
		Last Modified: Sat, 28 May 2022 02:28:18 GMT  
		Size: 50.9 MB (50861197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9edc6014a1d77c037b5ca755cb082ca750b5b0caf9a70fcb56472fcbcfc4050`  
		Last Modified: Sat, 28 May 2022 02:30:21 GMT  
		Size: 180.0 MB (180015753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41eeecc7d122852cc992c1b45a3855154c38d1c0b0b10c569be62f18b681f925`  
		Last Modified: Sun, 29 May 2022 18:48:22 GMT  
		Size: 179.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e61561941b5e57c5d87d653721685b1d37fea7478f27c1fcd69ede04bf225e`  
		Last Modified: Sun, 29 May 2022 18:50:47 GMT  
		Size: 13.6 MB (13619162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded-buster` - linux; ppc64le

```console
$ docker pull perl@sha256:70769c444c7cc8ce1744e4c933d0adff4028b05df2bab0371f9eb94cb175a60e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.5 MB (348463292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49155b04c2976820d106e4319e718fa0120a36fb19e8cf3a6d7a4bd65b8da63a`
-	Default Command: `["perl5.34.1","-de0"]`

```dockerfile
# Sat, 28 May 2022 01:23:18 GMT
ADD file:111395200ed598f754f449a2c278d0de3716fe88c66495506bbfba93a1be60d9 in / 
# Sat, 28 May 2022 01:23:24 GMT
CMD ["bash"]
# Sat, 28 May 2022 03:15:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 03:16:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 May 2022 03:17:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 03:23:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 23:16:48 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 28 May 2022 23:16:51 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Sat, 28 May 2022 23:16:55 GMT
WORKDIR /usr/src/perl
# Sat, 28 May 2022 23:59:06 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.1.tar.xz -o perl-5.34.1.tar.xz     && echo '6d52cf833ff1af27bb5e986870a2c30cec73c044b41e3458cd991f94374039f7 *perl-5.34.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.1.tar.xz -C /usr/src/perl     && rm perl-5.34.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Sat, 28 May 2022 23:59:11 GMT
WORKDIR /
# Sat, 28 May 2022 23:59:14 GMT
CMD ["perl5.34.1" "-de0"]
```

-	Layers:
	-	`sha256:a84717e4877770b3a8a9f0eb6890cb457d0bf1ec5c2013b56c1a2353beb5cbc0`  
		Last Modified: Sat, 28 May 2022 01:32:57 GMT  
		Size: 54.2 MB (54176994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c34161779331d3aba2a35660a49ce70bb924f430f55cd87d24c4a93a50735456`  
		Last Modified: Sat, 28 May 2022 03:37:04 GMT  
		Size: 8.3 MB (8293525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1daa1667acca77ec8c0a28fe3d5e8914209d4ab7d21c9ae4f44667705750e5a2`  
		Last Modified: Sat, 28 May 2022 03:37:04 GMT  
		Size: 10.7 MB (10727643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54afe3a1ca9ebf47897da5bf3470187988793f427ac1efc94b7f4d1d754e7db`  
		Last Modified: Sat, 28 May 2022 03:37:27 GMT  
		Size: 57.5 MB (57457968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d33c72787f5105ae2ebd54d1a426d819f48f61fa4c9b6d1351266d30635844`  
		Last Modified: Sat, 28 May 2022 03:38:12 GMT  
		Size: 203.4 MB (203371098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480da345ad783dc9862a300a5f52bba3e280592c46318281185bb17a7484add8`  
		Last Modified: Sun, 29 May 2022 02:54:44 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a846e82c4e70beb25ae94edadd7e7077b973bc426e5a5685e6fa8ef969b862d`  
		Last Modified: Sun, 29 May 2022 02:56:52 GMT  
		Size: 14.4 MB (14435862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded-buster` - linux; s390x

```console
$ docker pull perl@sha256:e54f2f6da7310b6f4daf8cb38ce30f4013b29db6d920fc3617cf0b25c6f0a094
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.6 MB (309559984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95345901329bb8c9bef7680ba8a6fe55d9c6db4ee0c17971752246dd683f1047`
-	Default Command: `["perl5.36.0","-de0"]`

```dockerfile
# Sat, 28 May 2022 00:43:20 GMT
ADD file:65712051a170cb9d0b18d0085bc26171598119b8946fa55b5ee959661b48a5d2 in / 
# Sat, 28 May 2022 00:43:26 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:25:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:25:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 May 2022 02:25:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:27:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:43:27 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 28 May 2022 05:43:27 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Sat, 28 May 2022 05:43:28 GMT
WORKDIR /usr/src/perl
# Mon, 30 May 2022 18:15:52 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.36.0.tar.xz -o perl-5.36.0.tar.xz     && echo '0f386dccbee8e26286404b2cca144e1005be65477979beb9b1ba272d4819bcf0 *perl-5.36.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.36.0.tar.xz -C /usr/src/perl     && rm perl-5.36.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Mon, 30 May 2022 18:15:56 GMT
WORKDIR /
# Mon, 30 May 2022 18:15:56 GMT
CMD ["perl5.36.0" "-de0"]
```

-	Layers:
	-	`sha256:771d2d61f47933c8d05a5f7e35dcb16848a6225e7531db8e5971d528982538e9`  
		Last Modified: Sat, 28 May 2022 00:50:02 GMT  
		Size: 49.0 MB (49006810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df770b877bc8966d8f5d52cb3a7ab3f8bbd879f885cd61e637b2561657af7817`  
		Last Modified: Sat, 28 May 2022 02:36:01 GMT  
		Size: 7.4 MB (7423705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cfa8ac3a66d83a9351be236e2dad0b6305f4fc7f162891629ed852f205e884e`  
		Last Modified: Sat, 28 May 2022 02:36:01 GMT  
		Size: 9.9 MB (9883325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29bc90555bb48ea3318f33a26a32ad4a827ace919e55dd094bd11e93c555a857`  
		Last Modified: Sat, 28 May 2022 02:36:17 GMT  
		Size: 51.4 MB (51382611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc0c1ea0ceff56a8da88d248fa4aed641749e436417dcebf9e8611397fdebfd`  
		Last Modified: Sat, 28 May 2022 02:36:43 GMT  
		Size: 177.0 MB (176965534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642fcc395e4c7508f73ab4f5856b6ccef98d8b6894d59893ccc66ae8e5f5df7c`  
		Last Modified: Sat, 28 May 2022 08:59:56 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48600de2135b6c01ca9d04ef53fc43ffc3b6c4a4b0659a3923379c36e2246dad`  
		Last Modified: Mon, 30 May 2022 18:37:03 GMT  
		Size: 14.9 MB (14897797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
