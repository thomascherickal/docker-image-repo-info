## `perl:threaded-bullseye`

```console
$ docker pull perl@sha256:ca76d417026c055842632152d56f2ddc4211957b1ab189d8efebb9c5c29ef775
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

### `perl:threaded-bullseye` - linux; amd64

```console
$ docker pull perl@sha256:bce4cc56a23ce54c970ec22938d5840957a772788b638e8e0e52ba3f0a42777a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.4 MB (336438591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d809ab1b0d438f20f5da1bbeb7d93f833754847c3aa87f0e96d5b7a7bb1b1503`
-	Default Command: `["perl5.34.1","-de0"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:07 GMT
ADD file:e8d512b08fe2ddc6f2c85831c73e4c72b9c850fa428913d19da4bb1a34f84cf2 in / 
# Tue, 29 Mar 2022 00:22:08 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 17:29:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:29:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 17:30:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:31:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 19:50:58 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 29 Mar 2022 19:50:59 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 29 Mar 2022 19:50:59 GMT
WORKDIR /usr/src/perl
# Tue, 29 Mar 2022 20:25:57 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.1.tar.xz -o perl-5.34.1.tar.xz     && echo '6d52cf833ff1af27bb5e986870a2c30cec73c044b41e3458cd991f94374039f7 *perl-5.34.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.1.tar.xz -C /usr/src/perl     && rm perl-5.34.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 29 Mar 2022 20:25:57 GMT
WORKDIR /
# Tue, 29 Mar 2022 20:25:57 GMT
CMD ["perl5.34.1" "-de0"]
```

-	Layers:
	-	`sha256:dbba69284b2786013fe94fefe0c2e66a7d3cecbb20f6d691d71dac891ee37be5`  
		Last Modified: Tue, 29 Mar 2022 00:26:47 GMT  
		Size: 54.9 MB (54937710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9baf437a1badb6aad2dae5f2cd4a7b53a6c7ab6c14cba1ed1ecb42b4822b0e87`  
		Last Modified: Tue, 29 Mar 2022 17:38:08 GMT  
		Size: 5.2 MB (5155705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ade5c59e324bd7cf369c72ad781c23d37e8fb48c9bbb4abbecafafd9be4cc35`  
		Last Modified: Tue, 29 Mar 2022 17:38:08 GMT  
		Size: 10.9 MB (10874957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b19a994f6d4cdbb620339bd2e4ad47b229f14276b542060622ae447649294e5d`  
		Last Modified: Tue, 29 Mar 2022 17:38:33 GMT  
		Size: 54.6 MB (54576420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc2294f89de5e20d0ae12149d6136444bcb8c775ea745f06f2eb775ab4504cd`  
		Last Modified: Tue, 29 Mar 2022 17:39:09 GMT  
		Size: 196.5 MB (196549680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f948b3edb3756e59df65118cd98d0ec931dff3fd64314cbc92bd29ceb7555333`  
		Last Modified: Tue, 29 Mar 2022 22:43:27 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36aa60d8bb961bc6541564268a3905f9b3ed11d75341d73d92d5d0ba6487a1df`  
		Last Modified: Tue, 29 Mar 2022 22:45:01 GMT  
		Size: 14.3 MB (14343920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded-bullseye` - linux; arm variant v5

```console
$ docker pull perl@sha256:7f58847d38377fc66627f9e5220b2225172c9a09e72f513627ce5b6897ce3356
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.8 MB (308792519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cda91d56c4a020085e80dd252472481a519c0de4cfd2151bb366f2bb1bc7981b`
-	Default Command: `["perl5.34.1","-de0"]`

```dockerfile
# Tue, 29 Mar 2022 00:50:03 GMT
ADD file:6cca5eca42975074f53a45a9b4ba83d1f06b95182dd4d8d95622d63cbc206574 in / 
# Tue, 29 Mar 2022 00:50:04 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 07:42:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 07:43:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 07:43:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 07:46:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 09:07:25 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 29 Mar 2022 09:07:26 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 29 Mar 2022 09:07:26 GMT
WORKDIR /usr/src/perl
# Tue, 29 Mar 2022 10:18:23 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.1.tar.xz -o perl-5.34.1.tar.xz     && echo '6d52cf833ff1af27bb5e986870a2c30cec73c044b41e3458cd991f94374039f7 *perl-5.34.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.1.tar.xz -C /usr/src/perl     && rm perl-5.34.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 29 Mar 2022 10:18:24 GMT
WORKDIR /
# Tue, 29 Mar 2022 10:18:25 GMT
CMD ["perl5.34.1" "-de0"]
```

-	Layers:
	-	`sha256:cfb93eae062e68427eb7e96f51a690313db08e4118ca20b5a644c29fecb784db`  
		Last Modified: Tue, 29 Mar 2022 01:04:42 GMT  
		Size: 52.5 MB (52475868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d69db2a0aac9ea7e48801a42d0b5e9e3a116bd0cdc20079aea745dd5653a7a`  
		Last Modified: Tue, 29 Mar 2022 08:05:43 GMT  
		Size: 5.1 MB (5065379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcddb47fa9924cdf33c6afa828fb4fa1365d464069ed1a63a5063b7daabbabe1`  
		Last Modified: Tue, 29 Mar 2022 08:05:45 GMT  
		Size: 10.6 MB (10572944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a5b09c9df3962b241df6ed71a37e9f3febeec33fcff083e6417ada9551f79c`  
		Last Modified: Tue, 29 Mar 2022 08:06:39 GMT  
		Size: 52.3 MB (52316733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4143c8cd4d6b7dbf43776eeea503e09e9f990a31f2a36d8d25ccb1b46227d436`  
		Last Modified: Tue, 29 Mar 2022 08:08:25 GMT  
		Size: 174.8 MB (174751086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c710986b8174e5e0b9274da75110672c25dc6be156f8359a7b8deebbfb8a6140`  
		Last Modified: Tue, 29 Mar 2022 14:25:30 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0070094fc5c5a8ec10ea7ffd022bbba357280ba2be2c44401c33b526de51b196`  
		Last Modified: Tue, 29 Mar 2022 14:28:18 GMT  
		Size: 13.6 MB (13610309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded-bullseye` - linux; arm variant v7

```console
$ docker pull perl@sha256:5ab43a58f6a63019d6a8c1e794a833ad31af7f3d4807f1550db96a52c2c7bf8a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.0 MB (296007866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:355cbc38884bcc4b3d22aed169422b2f85da48c63e340a4a0cf361aa17ebc2ea`
-	Default Command: `["perl5.34.1","-de0"]`

```dockerfile
# Thu, 17 Mar 2022 09:30:27 GMT
ADD file:a76bfdf79974fef637725f4c4d8afd998baacd9f3852ac94ce4db52fd65edd8c in / 
# Thu, 17 Mar 2022 09:30:28 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 02:52:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 02:52:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 02:53:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 02:55:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 04:29:06 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 19 Mar 2022 04:29:06 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Sat, 19 Mar 2022 04:29:07 GMT
WORKDIR /usr/src/perl
# Sat, 19 Mar 2022 05:25:51 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.1.tar.xz -o perl-5.34.1.tar.xz     && echo '6d52cf833ff1af27bb5e986870a2c30cec73c044b41e3458cd991f94374039f7 *perl-5.34.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.1.tar.xz -C /usr/src/perl     && rm perl-5.34.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Sat, 19 Mar 2022 05:25:52 GMT
WORKDIR /
# Sat, 19 Mar 2022 05:25:52 GMT
CMD ["perl5.34.1" "-de0"]
```

-	Layers:
	-	`sha256:4a0c373b7fd878320ee1d0810692c38f8079bd0783a53740b236b67ccd6eab4f`  
		Last Modified: Thu, 17 Mar 2022 09:45:54 GMT  
		Size: 50.1 MB (50122251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a9d199c77419ab8067bd77407cb0151e23cf09849e1fc7f550156c8d5ff053`  
		Last Modified: Sat, 19 Mar 2022 03:29:05 GMT  
		Size: 4.9 MB (4922780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a175e3c76032f69174aba6e645720559d1bef82bbf1946d37266a8543cec9b75`  
		Last Modified: Sat, 19 Mar 2022 03:29:07 GMT  
		Size: 10.2 MB (10216952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8ef8cc586469458a5d1e2e47026303e46cf29e47935386efe16d91d34fe708c`  
		Last Modified: Sat, 19 Mar 2022 03:29:56 GMT  
		Size: 50.3 MB (50328447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291fb16f7bcc8b0503109f50011e8ac9d4d161603ba3b1cf31678c8cb42e60d8`  
		Last Modified: Sat, 19 Mar 2022 03:31:44 GMT  
		Size: 167.0 MB (166993565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6228a6637948e1e479515a5ca28b082fb8226711fcccb227539ebf43014e2015`  
		Last Modified: Sat, 19 Mar 2022 09:05:28 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d0cb614bb1a2c247f49724561cec25edff39cb40201d609cf4201e716100aa`  
		Last Modified: Sat, 19 Mar 2022 09:08:17 GMT  
		Size: 13.4 MB (13423668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded-bullseye` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:e9e8621f9036827c4c3e677bafd947b4aa76941b3f4a0acfc2bec918b9680c97
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.6 MB (327600275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df86f863321c0e9191a068f1515312841586a8329e6d8b5a8176501a5cabf9cb`
-	Default Command: `["perl5.34.1","-de0"]`

```dockerfile
# Thu, 17 Mar 2022 03:21:41 GMT
ADD file:5effc7e0ab7312f14a7ee81c06c71400aae31219d477ebe1a4f7a9156797c42a in / 
# Thu, 17 Mar 2022 03:21:42 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 22:10:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 22:11:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Mar 2022 22:11:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 22:12:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 02:05:17 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Fri, 18 Mar 2022 02:05:18 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Fri, 18 Mar 2022 02:05:19 GMT
WORKDIR /usr/src/perl
# Sat, 19 Mar 2022 16:34:02 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.1.tar.xz -o perl-5.34.1.tar.xz     && echo '6d52cf833ff1af27bb5e986870a2c30cec73c044b41e3458cd991f94374039f7 *perl-5.34.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.1.tar.xz -C /usr/src/perl     && rm perl-5.34.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Sat, 19 Mar 2022 16:34:03 GMT
WORKDIR /
# Sat, 19 Mar 2022 16:34:04 GMT
CMD ["perl5.34.1" "-de0"]
```

-	Layers:
	-	`sha256:260ad8146ed2447d5587608b10fed4f80de80cdc559e619f3a235d3ba09eaf7b`  
		Last Modified: Thu, 17 Mar 2022 03:28:04 GMT  
		Size: 53.6 MB (53616308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1399f445da611be3789923cf26d158e3f4f80449b7295fa069a8eaecaaf137e6`  
		Last Modified: Thu, 17 Mar 2022 22:20:58 GMT  
		Size: 4.9 MB (4937558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd9e43777fa6c09c341f3aa922f47b5b3ace26de1d779124afd2f1d435731d9`  
		Last Modified: Thu, 17 Mar 2022 22:20:58 GMT  
		Size: 10.7 MB (10655858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f81267e40a2df9e572fe797e45dbc086008422eb2216df18b7a91f1cf13e22b`  
		Last Modified: Thu, 17 Mar 2022 22:21:21 GMT  
		Size: 54.7 MB (54671322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460c4ae3ed9f0c0fe1ee94e09cfb3993206231793fc9e841ad8f0975895ddb9e`  
		Last Modified: Thu, 17 Mar 2022 22:22:00 GMT  
		Size: 189.5 MB (189453989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a3318085adda56f0955b1da37fb63e594a29d4238b1db1a8b64d97f49696ac`  
		Last Modified: Fri, 18 Mar 2022 03:48:13 GMT  
		Size: 179.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9dc6d5b681b34eb02bf53f22b187a214572aa5f687d638b701c7dbe6daad954`  
		Last Modified: Sat, 19 Mar 2022 17:25:55 GMT  
		Size: 14.3 MB (14265061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded-bullseye` - linux; 386

```console
$ docker pull perl@sha256:21cd7f7edbe2bdf214720d02fd235538fa2a29024af1b05319504d4d27fa33c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **341.7 MB (341736060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc5bb4bfbac54d64b86488f95e35968acf26f76219db0fa58119af8b51de87c8`
-	Default Command: `["perl5.34.1","-de0"]`

```dockerfile
# Thu, 17 Mar 2022 08:15:32 GMT
ADD file:db8b3d2a46fd5f7f175e96ecfedbb16788e0232263c4d22fd79f2c997c6dc9d5 in / 
# Thu, 17 Mar 2022 08:15:32 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 14:26:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 14:27:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Mar 2022 14:27:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 14:28:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 15:08:42 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 29 Mar 2022 15:08:43 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 29 Mar 2022 15:08:43 GMT
WORKDIR /usr/src/perl
# Tue, 29 Mar 2022 15:34:48 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.1.tar.xz -o perl-5.34.1.tar.xz     && echo '6d52cf833ff1af27bb5e986870a2c30cec73c044b41e3458cd991f94374039f7 *perl-5.34.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.1.tar.xz -C /usr/src/perl     && rm perl-5.34.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 29 Mar 2022 15:34:48 GMT
WORKDIR /
# Tue, 29 Mar 2022 15:34:49 GMT
CMD ["perl5.34.1" "-de0"]
```

-	Layers:
	-	`sha256:c46f89774ba16a64f47622b4e0890ea7dfdf72f98f9c0fe3a99b594f399ce289`  
		Last Modified: Thu, 17 Mar 2022 08:23:24 GMT  
		Size: 55.9 MB (55942412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062efdde483971aec1766d9a277cc1611b0f018b2694acb118e5938eeea0ec3c`  
		Last Modified: Fri, 18 Mar 2022 14:43:37 GMT  
		Size: 5.3 MB (5283288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da05aae7c571a7d0a7b2e1180210da68186bf520efade8e0bfbe91fe18c970c`  
		Last Modified: Fri, 18 Mar 2022 14:43:38 GMT  
		Size: 11.3 MB (11250684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6825211753c1c85f2d11bfa499b352d42cb70363540c66428d136a97e6d4cc7`  
		Last Modified: Fri, 18 Mar 2022 14:44:06 GMT  
		Size: 55.9 MB (55920045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5bcfa3fde35dadae573e5cecf3531e2f895ebd560cb7708f1dfd8758afc532a`  
		Last Modified: Fri, 18 Mar 2022 14:45:00 GMT  
		Size: 199.5 MB (199488816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df1568404ac6defe50c982fa5c79858b097be42a1f5906af7afcf586a35ca6a`  
		Last Modified: Tue, 29 Mar 2022 17:16:31 GMT  
		Size: 181.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f49c3ea8751cbabd7b23a5339c0b8d38172808d68c46c798251896e2794c51f`  
		Last Modified: Tue, 29 Mar 2022 17:18:29 GMT  
		Size: 13.9 MB (13850634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded-bullseye` - linux; mips64le

```console
$ docker pull perl@sha256:5a89e4e2369b55beb10c6df15dc555ad69e82dc03c1dcbb1673ec31e9b26ac4b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.4 MB (314380216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfee7330095e93c3065031d0c89fb50f705134c900709c048f2fb45d47af11b0`
-	Default Command: `["perl5.34.1","-de0"]`

```dockerfile
# Tue, 29 Mar 2022 07:41:51 GMT
ADD file:40fc6f06ccce55e9889d1c94556c29242d1ac62870cb9895da64d37bac45ab5e in / 
# Tue, 29 Mar 2022 07:41:56 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 08:27:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 08:27:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 08:29:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 08:35:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 10:41:13 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 29 Mar 2022 10:41:18 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 29 Mar 2022 10:41:24 GMT
WORKDIR /usr/src/perl
# Tue, 29 Mar 2022 12:22:24 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.1.tar.xz -o perl-5.34.1.tar.xz     && echo '6d52cf833ff1af27bb5e986870a2c30cec73c044b41e3458cd991f94374039f7 *perl-5.34.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.1.tar.xz -C /usr/src/perl     && rm perl-5.34.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 29 Mar 2022 12:22:30 GMT
WORKDIR /
# Tue, 29 Mar 2022 12:22:37 GMT
CMD ["perl5.34.1" "-de0"]
```

-	Layers:
	-	`sha256:efb90a274e1b19eec263e44f7fbc1f9c9c6c393210c27b03ebde7c2b0a2b6482`  
		Last Modified: Tue, 29 Mar 2022 07:52:16 GMT  
		Size: 53.2 MB (53199386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7959b932ae1363e586ef79fc1ab6afdaee0b7a9f97e0a507c1868cfc6dd47778`  
		Last Modified: Tue, 29 Mar 2022 08:57:32 GMT  
		Size: 4.9 MB (4912295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3b22f54d8b49fd2d7d246274c6016cdcff9377c15befaa4323d44c3b1e75ac`  
		Last Modified: Tue, 29 Mar 2022 08:57:35 GMT  
		Size: 10.7 MB (10660105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d388c5955683d48c342f8d6b2291b7cedf59d2fcfb9343f5aa240f4b5f56da3`  
		Last Modified: Tue, 29 Mar 2022 08:58:23 GMT  
		Size: 53.3 MB (53297457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5cb02e44057e09f6326c9e36eed5fc0f3826629151ef1cccd58806a443496cb`  
		Last Modified: Tue, 29 Mar 2022 09:00:27 GMT  
		Size: 178.7 MB (178702640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d2a96d6fbc4ef7f553e35f0350ecbbb61e1646e2f5fd781f49a208d348e995`  
		Last Modified: Tue, 29 Mar 2022 18:52:12 GMT  
		Size: 181.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c34ebd4b27b3f0bf06862d2d009765fecbb467ba48cf38d007cbd832172fde2`  
		Last Modified: Tue, 29 Mar 2022 18:54:35 GMT  
		Size: 13.6 MB (13608152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded-bullseye` - linux; ppc64le

```console
$ docker pull perl@sha256:3c6f2fcb621796ffbea7ad57a8f899fece6964782376aa571eec822fd03c8b89
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **345.0 MB (345016520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab4a27f9a0d043680fe93567e6311d55670a668ca4002512eb1b3d294737bfbd`
-	Default Command: `["perl5.34.1","-de0"]`

```dockerfile
# Thu, 17 Mar 2022 11:17:18 GMT
ADD file:c923f87aafa36beb6a65a06ebafd39557c7aa7cbd28e30202aae5219292bb1f7 in / 
# Thu, 17 Mar 2022 11:17:22 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 05:39:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 05:39:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 05:41:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 05:47:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 07:55:55 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 19 Mar 2022 07:55:56 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Sat, 19 Mar 2022 07:55:58 GMT
WORKDIR /usr/src/perl
# Sat, 19 Mar 2022 08:45:18 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.1.tar.xz -o perl-5.34.1.tar.xz     && echo '6d52cf833ff1af27bb5e986870a2c30cec73c044b41e3458cd991f94374039f7 *perl-5.34.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.1.tar.xz -C /usr/src/perl     && rm perl-5.34.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Sat, 19 Mar 2022 08:45:22 GMT
WORKDIR /
# Sat, 19 Mar 2022 08:45:26 GMT
CMD ["perl5.34.1" "-de0"]
```

-	Layers:
	-	`sha256:3eba077833cc07e760f6d7835470f68bfa37da9e30e164c5acb55a2be317cb9a`  
		Last Modified: Thu, 17 Mar 2022 11:27:38 GMT  
		Size: 58.8 MB (58842629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606a8f23e2e92dfe52c8d6766e424128de38f3daf03ac630fcb4485deab4f2d5`  
		Last Modified: Sat, 19 Mar 2022 06:39:33 GMT  
		Size: 5.4 MB (5402016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f42cb9c0e6100c969995a76b5e25614396bdb4079794a9e37b61a6e13a0badd`  
		Last Modified: Sat, 19 Mar 2022 06:39:34 GMT  
		Size: 11.6 MB (11626006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf6a22b7fd2790b3af2d142ff1f5f3601c6fbcaf889c3b37511fca470154f99`  
		Last Modified: Sat, 19 Mar 2022 06:40:22 GMT  
		Size: 58.9 MB (58854408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f4bb633d127e55dbbfa2fce49955f044b7dd4cc21212dd1ecb2ffb1633ff7e`  
		Last Modified: Sat, 19 Mar 2022 06:42:12 GMT  
		Size: 195.9 MB (195920453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716857d25cff31296312c40f66109cbfa55c599ff95298a9bc96f7a58d683892`  
		Last Modified: Sat, 19 Mar 2022 11:38:22 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b88f5cf4d4dfad8b2c28a44ed777b7a277f69945471a17251e747ca5818a029e`  
		Last Modified: Sat, 19 Mar 2022 11:40:40 GMT  
		Size: 14.4 MB (14370806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded-bullseye` - linux; s390x

```console
$ docker pull perl@sha256:7152bb45f89a4e2917ee5f6b0cae25f339a2c3d36fc571dc506a870bb6f81487
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.4 MB (310387074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:326b825fe3a352f845f5dd1532d9ad89305af2f3e5e4893534d2dd3d42379fc6`
-	Default Command: `["perl5.34.1","-de0"]`

```dockerfile
# Thu, 17 Mar 2022 03:06:38 GMT
ADD file:75b45e65d2ec2c6822b1ddc46ff159dd10ac56bf9dff8b0996ac589a1ede22ff in / 
# Thu, 17 Mar 2022 03:06:42 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 18:20:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 18:20:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Mar 2022 18:21:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 18:21:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 12:50:26 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Fri, 18 Mar 2022 12:50:27 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Fri, 18 Mar 2022 12:50:27 GMT
WORKDIR /usr/src/perl
# Sat, 19 Mar 2022 03:17:20 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.1.tar.xz -o perl-5.34.1.tar.xz     && echo '6d52cf833ff1af27bb5e986870a2c30cec73c044b41e3458cd991f94374039f7 *perl-5.34.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.1.tar.xz -C /usr/src/perl     && rm perl-5.34.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Sat, 19 Mar 2022 03:17:22 GMT
WORKDIR /
# Sat, 19 Mar 2022 03:17:22 GMT
CMD ["perl5.34.1" "-de0"]
```

-	Layers:
	-	`sha256:ae9f1a186a2633be1ad71c317c2f195b221cef89502f9edc510b3a2049723758`  
		Last Modified: Thu, 17 Mar 2022 03:12:26 GMT  
		Size: 53.2 MB (53217527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d6229369d1bac8aa97bfefe6dd7990a66c0a3e98f420c282a39a279df7c391`  
		Last Modified: Thu, 17 Mar 2022 18:29:06 GMT  
		Size: 5.1 MB (5137013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf171d8059efb2bc6c026904c68dddd3487a129cd53d33def9589665326d56f`  
		Last Modified: Thu, 17 Mar 2022 18:29:07 GMT  
		Size: 10.8 MB (10761392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cdad8e45654b094c248eb6bc86e3e0d8dda7b0e1df7c2792f2abb3a0d18cc8`  
		Last Modified: Thu, 17 Mar 2022 18:29:23 GMT  
		Size: 54.0 MB (54044974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e2828c31b6d51c45569d0b8f772cf386976b6fe283da599e6548b290f167d0`  
		Last Modified: Thu, 17 Mar 2022 18:29:49 GMT  
		Size: 172.5 MB (172540992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d01256dcc79614112ad2cf28e7273cc1bae7b91599b8499c10fe0ad9148713`  
		Last Modified: Fri, 18 Mar 2022 14:02:12 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7631278c649d7e96560b86df6832acb28d9737a4636d4c224e258724a10eb96`  
		Last Modified: Sat, 19 Mar 2022 04:16:53 GMT  
		Size: 14.7 MB (14684974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
