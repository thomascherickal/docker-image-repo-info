## `perl:devel-threaded-bullseye`

```console
$ docker pull perl@sha256:7b15181896d7e724c87882ef718c592a65d03d2edc009807b13a7f708f6fd060
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

### `perl:devel-threaded-bullseye` - linux; amd64

```console
$ docker pull perl@sha256:7758bb1aa082d7ec16020d1b8c2b7c14e4337ff92f6c6d583bda7be636a64d11
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.9 MB (337927455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d4848057e7b3ca41869653cf8882076e8620fcd60da655a62f4fad0ce777eb7`
-	Default Command: `["perl5.39.3","-de0"]`

```dockerfile
# Wed, 20 Sep 2023 04:55:51 GMT
ADD file:85db4f4c5016f51f7112a5d09cb7d4620f565a1379ae4b8a03c5ffc23886a876 in / 
# Wed, 20 Sep 2023 04:55:51 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:22:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:22:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:23:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 12:31:20 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 20 Sep 2023 12:31:20 GMT
WORKDIR /usr/src/perl
# Mon, 25 Sep 2023 20:56:44 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.3.tar.xz -o perl-5.39.3.tar.xz     && echo '93c38a6ff969e3930d7eb08e69a883204a4d835c7122df47c4903950e6fc758a *perl-5.39.3.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.3.tar.xz -C /usr/src/perl     && rm perl-5.39.3.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Mon, 25 Sep 2023 20:56:44 GMT
WORKDIR /usr/src/app
# Mon, 25 Sep 2023 20:56:45 GMT
CMD ["perl5.39.3" "-de0"]
```

-	Layers:
	-	`sha256:ddf874abf16cc990e0fd75a154a34ca0a03ee310ad895a18fb62ae15bf4171fb`  
		Last Modified: Wed, 20 Sep 2023 05:00:41 GMT  
		Size: 55.1 MB (55056714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1459d3ab8b5e46ac1a0a00134fe2f7b693474eb6d75ace97ecbe811a6f5b0e`  
		Last Modified: Wed, 20 Sep 2023 09:31:06 GMT  
		Size: 15.8 MB (15760408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab00e7798a04602c3f6e2dc445a994d75e96c45533cd44701f58509982a8c5`  
		Last Modified: Wed, 20 Sep 2023 09:31:23 GMT  
		Size: 54.6 MB (54584790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7883a473306cf6632abe7e913e0f1a21ac2fed038a4116473b25738b8b88b294`  
		Last Modified: Wed, 20 Sep 2023 09:31:55 GMT  
		Size: 196.8 MB (196842512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52b3edeb95fa7a0041689ffc83f83c850c381908d41acdd82e901f87878cdfd`  
		Last Modified: Wed, 20 Sep 2023 16:26:00 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f04eea7a37064b65653734ac94735c1c0ef785c7bfe868f9f34efaa9cd85fea8`  
		Last Modified: Mon, 25 Sep 2023 21:14:08 GMT  
		Size: 15.7 MB (15682700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26953fd9e26fe2aa39f09627c9f20663371e9b55ca8a26331aaeab5f871e37d9`  
		Last Modified: Mon, 25 Sep 2023 21:14:05 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-threaded-bullseye` - linux; arm variant v5

```console
$ docker pull perl@sha256:9d73fe11dd75222ad789fa3a9a4e4ee93ec41aa120c303bca6bd3107a21e380e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.3 MB (310274092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cca43cf724539ed6cf756f710a4fa57225597df3f8f84f009f7c9ecb5cc3445`
-	Default Command: `["perl5.39.3","-de0"]`

```dockerfile
# Wed, 20 Sep 2023 00:50:08 GMT
ADD file:36b8026af7713ecb15198f7cb7beff053db2fb1d0cdbba2e05ede6d2067120be in / 
# Wed, 20 Sep 2023 00:50:08 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:57:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:57:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:59:16 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 13:33:51 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 20 Sep 2023 13:33:51 GMT
WORKDIR /usr/src/perl
# Mon, 25 Sep 2023 20:07:25 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.3.tar.xz -o perl-5.39.3.tar.xz     && echo '93c38a6ff969e3930d7eb08e69a883204a4d835c7122df47c4903950e6fc758a *perl-5.39.3.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.3.tar.xz -C /usr/src/perl     && rm perl-5.39.3.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Mon, 25 Sep 2023 20:07:25 GMT
WORKDIR /usr/src/app
# Mon, 25 Sep 2023 20:07:25 GMT
CMD ["perl5.39.3" "-de0"]
```

-	Layers:
	-	`sha256:791ab9666f498037db4451bb82dd3cb63afd5ef69c2068959d5516a7832d373b`  
		Last Modified: Wed, 20 Sep 2023 00:55:10 GMT  
		Size: 52.6 MB (52558199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37002420bf0e3d73b89ed87c7e321032a64691875353cde3cc0370cc78f07f50`  
		Last Modified: Wed, 20 Sep 2023 10:06:18 GMT  
		Size: 15.4 MB (15369135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43ccaa88e1d24c47bf1c55018f8d61128185b8b108f3c5c1d641a7f96a0fea0`  
		Last Modified: Wed, 20 Sep 2023 10:06:36 GMT  
		Size: 52.3 MB (52340617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d334d3272118e82d2944c89ec38c02adf4d2140b4b133805f538ad58e6449e9d`  
		Last Modified: Wed, 20 Sep 2023 10:07:22 GMT  
		Size: 175.1 MB (175056831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e9593005fb4011362fc25e6666a5242fc03a6ed144d8fe97e1329537aa522bc`  
		Last Modified: Wed, 20 Sep 2023 15:11:17 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d730027a66eb58df03fe109962fa0f051940f2683e4868a31cce29162c8c81ba`  
		Last Modified: Mon, 25 Sep 2023 20:15:19 GMT  
		Size: 14.9 MB (14948978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6b5559befea6168f72341fbc13aca5d3c72388c041e428000aa84da96d81ce`  
		Last Modified: Mon, 25 Sep 2023 20:15:15 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-threaded-bullseye` - linux; arm variant v7

```console
$ docker pull perl@sha256:dc728d5eb7f5c1aa907ead00114e7eae902ebd6e69fdfdd44d5e7b4ec7a5f0fd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.5 MB (297505466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fd9a32fb5d19ffe27fd703521b96b671075fcdb3a0886d7e63892f9d0ad56d7`
-	Default Command: `["perl5.39.3","-de0"]`

```dockerfile
# Wed, 20 Sep 2023 04:57:26 GMT
ADD file:3bf3380482840b3a4166e82c3f951812076851ba1527261fdd1da780662b2de1 in / 
# Wed, 20 Sep 2023 04:57:26 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 15:26:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 15:26:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 15:28:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 17:08:11 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 20 Sep 2023 17:08:11 GMT
WORKDIR /usr/src/perl
# Mon, 25 Sep 2023 20:48:40 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.3.tar.xz -o perl-5.39.3.tar.xz     && echo '93c38a6ff969e3930d7eb08e69a883204a4d835c7122df47c4903950e6fc758a *perl-5.39.3.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.3.tar.xz -C /usr/src/perl     && rm perl-5.39.3.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Mon, 25 Sep 2023 20:48:40 GMT
WORKDIR /usr/src/app
# Mon, 25 Sep 2023 20:48:40 GMT
CMD ["perl5.39.3" "-de0"]
```

-	Layers:
	-	`sha256:1d4e041d2204b383d6d6893cfcf5b852394f34744a85cea9ec0b3fb65cbc6143`  
		Last Modified: Wed, 20 Sep 2023 05:01:34 GMT  
		Size: 50.2 MB (50219551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbd770246538a809113f7f8fd84fedf3bd2bee5ed2f4fad2ab81cca9a78580d`  
		Last Modified: Wed, 20 Sep 2023 15:36:25 GMT  
		Size: 14.9 MB (14868646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145367a45c553b855c9dec20850966d6ec435636dba00c32133a9181c6f0b3e9`  
		Last Modified: Wed, 20 Sep 2023 15:36:43 GMT  
		Size: 50.4 MB (50355432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733e5937f159c4788716aa1891265686c96fd934eeccd3bbf46f01ea4bf34b5e`  
		Last Modified: Wed, 20 Sep 2023 15:37:14 GMT  
		Size: 167.3 MB (167322461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a4eefac99ecab3d08e3423a9068da1a56190345657fd930cb09711ccd4b24f`  
		Last Modified: Wed, 20 Sep 2023 21:28:54 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437e17663c58c51a19e6b7d2b0c9e54aad93f1d0892c6f86469a0c52061c588e`  
		Last Modified: Mon, 25 Sep 2023 21:06:08 GMT  
		Size: 14.7 MB (14739045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c8b3b26a0dfc75b52b4e480c6accf8a10a8b0808d65759729d5101aedba007`  
		Last Modified: Mon, 25 Sep 2023 21:06:04 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-threaded-bullseye` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:c8bb0187e8d6123d779b33344346f41dab56365286ef7d4c94b1193e32b14534
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.5 MB (329500953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6da4e02db4ed096d73dd55e6fb7d056cbe4e76227c90790ef511d0d9c127ada1`
-	Default Command: `["perl5.39.3","-de0"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:20 GMT
ADD file:46dcdcde338d2c01fed5db3fac9041736d9305145d8fc2039dd5b3714d38ede8 in / 
# Wed, 20 Sep 2023 02:44:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:24:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:25:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:26:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 12:49:59 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 20 Sep 2023 12:49:59 GMT
WORKDIR /usr/src/perl
# Mon, 25 Sep 2023 20:20:23 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.3.tar.xz -o perl-5.39.3.tar.xz     && echo '93c38a6ff969e3930d7eb08e69a883204a4d835c7122df47c4903950e6fc758a *perl-5.39.3.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.3.tar.xz -C /usr/src/perl     && rm perl-5.39.3.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Mon, 25 Sep 2023 20:20:24 GMT
WORKDIR /usr/src/app
# Mon, 25 Sep 2023 20:20:24 GMT
CMD ["perl5.39.3" "-de0"]
```

-	Layers:
	-	`sha256:31f5dc1f52c865588c43d8ec718f14d430e149b28f0b28232da825da7ae28f76`  
		Last Modified: Wed, 20 Sep 2023 02:47:53 GMT  
		Size: 53.7 MB (53704892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb60045eb75c62e890b95d28e4893132a6c7d61ec9979104ee4ff6e86c4badee`  
		Last Modified: Wed, 20 Sep 2023 09:33:11 GMT  
		Size: 15.7 MB (15746671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292737ab468ef80c6f78bdde4896157b8953d1e5556e1e526f40aeadcb547573`  
		Last Modified: Wed, 20 Sep 2023 09:33:26 GMT  
		Size: 54.7 MB (54676309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d93979d624211374be152eee1c99ed4ca9e6bae68694135fc440ab6c8fd2044`  
		Last Modified: Wed, 20 Sep 2023 09:33:51 GMT  
		Size: 189.8 MB (189778334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1117f9029f2f12e3c0ea1a49d453513b6d3c4ec5a2cf433fd56be576e3c53290`  
		Last Modified: Wed, 20 Sep 2023 15:58:14 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac170b2c2c6931f9cdf3fa86c93d47fc6197ba477194ff062823e8781f31e855`  
		Last Modified: Mon, 25 Sep 2023 20:35:04 GMT  
		Size: 15.6 MB (15594414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11d17a270b9b51dad036fd8cdf8f05efde766b784c32b2b05be6604ed6967b9`  
		Last Modified: Mon, 25 Sep 2023 20:35:01 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-threaded-bullseye` - linux; 386

```console
$ docker pull perl@sha256:a396fd8c593d14e5dda15561a7b228904e1c8657191523272179f117b6bd8ab0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343208446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c20e09b1e075075e32df731fa301268c3a08987f34c6c7de81b6d99370c3080d`
-	Default Command: `["perl5.39.3","-de0"]`

```dockerfile
# Wed, 20 Sep 2023 00:42:07 GMT
ADD file:342c36522089238a534c0912491a4cf64b89133969e051cdad2e694ec761142c in / 
# Wed, 20 Sep 2023 00:42:07 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 11:27:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 11:27:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 11:29:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 17:56:41 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 20 Sep 2023 17:56:42 GMT
WORKDIR /usr/src/perl
# Mon, 25 Sep 2023 20:42:01 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.3.tar.xz -o perl-5.39.3.tar.xz     && echo '93c38a6ff969e3930d7eb08e69a883204a4d835c7122df47c4903950e6fc758a *perl-5.39.3.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.3.tar.xz -C /usr/src/perl     && rm perl-5.39.3.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Mon, 25 Sep 2023 20:42:01 GMT
WORKDIR /usr/src/app
# Mon, 25 Sep 2023 20:42:01 GMT
CMD ["perl5.39.3" "-de0"]
```

-	Layers:
	-	`sha256:00121bf241b18e981bcc804f905be7b34f95cce415db622599e21dc1a496ee8d`  
		Last Modified: Wed, 20 Sep 2023 00:47:11 GMT  
		Size: 56.0 MB (56040498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656938def9400b0af510c0a87c5dd1a6daf011fd1270e3c56c71d6ec54b5ab1b`  
		Last Modified: Wed, 20 Sep 2023 11:38:25 GMT  
		Size: 16.3 MB (16263804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d08fdcc11a9302a19159b5ae4e19e22d42c914e371c0d7a532d73d7d45d3aed`  
		Last Modified: Wed, 20 Sep 2023 11:38:47 GMT  
		Size: 55.9 MB (55922986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3eabd2ad72b1eaa8ae1de02f17e175b40c5e4605b70269e10ad0283db90d6ac`  
		Last Modified: Wed, 20 Sep 2023 11:39:33 GMT  
		Size: 199.8 MB (199763042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f668da9214843ad6056e9e105b863ab71207238514ff5139841abff5acfb1342`  
		Last Modified: Thu, 21 Sep 2023 00:46:49 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2495fa23e844010df7b8b80ffbe699f0d10b4a50d6458bcafaff265bd9dda357`  
		Last Modified: Mon, 25 Sep 2023 21:09:23 GMT  
		Size: 15.2 MB (15217784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f51e1c1dd2dec20fd5071409ebec187cb950ba2f682e3a3807f78b409e8383c`  
		Last Modified: Mon, 25 Sep 2023 21:09:18 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-threaded-bullseye` - linux; mips64le

```console
$ docker pull perl@sha256:5dd498f4dcfb69a2e3fa8f30054edae76e331a5106b649684271d3991cab9e13
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.0 MB (315966840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41eeb4bca7a81dec0b4d5b7435035efaa4fd8a5461c65290151c3d51d7fc00ff`
-	Default Command: `["perl5.39.2","-de0"]`

```dockerfile
# Wed, 20 Sep 2023 03:10:35 GMT
ADD file:bf259f6a910dbc8dc738b19ecb6ee305bd4c4542ed155da31ec4169aafd244ff in / 
# Wed, 20 Sep 2023 03:10:40 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 21:53:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 21:55:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 22:01:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Sep 2023 05:18:59 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Fri, 22 Sep 2023 05:19:05 GMT
WORKDIR /usr/src/perl
# Fri, 22 Sep 2023 08:23:30 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.2.tar.xz -o perl-5.39.2.tar.xz     && echo 'b7ae33d3c6ff80107d14c92dfb3d8d4944fec926b11bcc40c8764b73c710694f *perl-5.39.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.2.tar.xz -C /usr/src/perl     && rm perl-5.39.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Fri, 22 Sep 2023 08:23:37 GMT
WORKDIR /usr/src/app
# Fri, 22 Sep 2023 08:23:43 GMT
CMD ["perl5.39.2" "-de0"]
```

-	Layers:
	-	`sha256:0c3ff68a43fe24d06c5623f35f7584c7f4260e244cb03f0be25b1b638b3b2f12`  
		Last Modified: Wed, 20 Sep 2023 03:21:44 GMT  
		Size: 53.3 MB (53271571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a5697015f5ab9ec0f1015233f9b7db31aeab37a53be5980438956f17f323bcf`  
		Last Modified: Wed, 20 Sep 2023 22:23:58 GMT  
		Size: 15.5 MB (15520488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902172eeced877afc9ac8166efa3aa8e216a40cc08607df275d2edff23a4dc33`  
		Last Modified: Wed, 20 Sep 2023 22:24:44 GMT  
		Size: 53.3 MB (53306542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00231754162cc10558113d1b98c11ceefa39e66f31857c94734b6c960190c3f1`  
		Last Modified: Wed, 20 Sep 2023 22:26:42 GMT  
		Size: 179.0 MB (178967400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:949a9797b53e9a387d11d57e3815c62070dcfd2bc997928d2a78272f77405b40`  
		Last Modified: Fri, 22 Sep 2023 08:24:32 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abf29a523d029855082da16084ed2db988e9302959ff9b5f775d71de8c2d148`  
		Last Modified: Fri, 22 Sep 2023 08:27:51 GMT  
		Size: 14.9 MB (14900573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1708e5b1fdcd43c4bbf75643a26e04488c4f46b04327f48de556ca7a2f651ad6`  
		Last Modified: Fri, 22 Sep 2023 08:27:39 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-threaded-bullseye` - linux; ppc64le

```console
$ docker pull perl@sha256:bc47854eb385fca18637b4ffdcd444991d2e3ca06ae192f6c44f57afac9a3943
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.5 MB (346483627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5e78bc599dac46039b1a9e83e7a655bec4aaadb0b7802bcaecd584673964c8a`
-	Default Command: `["perl5.39.3","-de0"]`

```dockerfile
# Wed, 20 Sep 2023 07:53:09 GMT
ADD file:c12b11abfba27478510c84d05abdd8fec539db9ec30af6d042671f4d5bf793e5 in / 
# Wed, 20 Sep 2023 07:53:12 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:53:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:54:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:59:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 18:37:52 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 20 Sep 2023 18:37:53 GMT
WORKDIR /usr/src/perl
# Mon, 25 Sep 2023 20:43:54 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.3.tar.xz -o perl-5.39.3.tar.xz     && echo '93c38a6ff969e3930d7eb08e69a883204a4d835c7122df47c4903950e6fc758a *perl-5.39.3.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.3.tar.xz -C /usr/src/perl     && rm perl-5.39.3.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Mon, 25 Sep 2023 20:43:56 GMT
WORKDIR /usr/src/app
# Mon, 25 Sep 2023 20:43:57 GMT
CMD ["perl5.39.3" "-de0"]
```

-	Layers:
	-	`sha256:9f3507d882ae95f06b3672497cdd3317bd4f8e0255e73d10f1f263e5d780f102`  
		Last Modified: Wed, 20 Sep 2023 08:50:16 GMT  
		Size: 58.9 MB (58928499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04a84a3dd07e7f4a4117efeb4dfb2cd5752a6495b332adc44482bd2964626ce9`  
		Last Modified: Wed, 20 Sep 2023 10:22:16 GMT  
		Size: 16.8 MB (16752924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca2a058b7253284355cf28252852be40a5207eb0fd8a7a9cbc7e2b0dd48e61e`  
		Last Modified: Wed, 20 Sep 2023 10:22:39 GMT  
		Size: 58.9 MB (58865110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22fa6f995be18d5920224ffc49bfb41e404969a3667799383a06921bd5d2ee3f`  
		Last Modified: Wed, 20 Sep 2023 10:23:33 GMT  
		Size: 196.2 MB (196219105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a390c85f40b92dcbe3893e7ad6e637ebfc32d7c7c783941d22945b0b9ec02d`  
		Last Modified: Wed, 20 Sep 2023 20:53:09 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d45f8fceaef37f8bfed7e64b7cbc66310ccbe32d67a6ae8025d5f25cffd10fa`  
		Last Modified: Mon, 25 Sep 2023 20:54:55 GMT  
		Size: 15.7 MB (15717659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cafb3a30e3ce2cab53d0fa20cab7febb75bc10b1e8bfd988eca128611dab0d`  
		Last Modified: Mon, 25 Sep 2023 20:54:49 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-threaded-bullseye` - linux; s390x

```console
$ docker pull perl@sha256:a88c76b877029c19f9422d6f4ef5d43c9ee655189db7a1da4bb33c0181ec224f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.9 MB (311890767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bf7aa8eda0377209f8e19e475b628a07da57a2cee447fb6d2c0fcb609c6744c`
-	Default Command: `["perl5.39.3","-de0"]`

```dockerfile
# Wed, 20 Sep 2023 02:54:37 GMT
ADD file:eedfa120b98e158d4eeb9ecad39e28c5715c44bddec3545f61b78ecebd01cc11 in / 
# Wed, 20 Sep 2023 02:54:41 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:51:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:51:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:52:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 10:51:57 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 20 Sep 2023 10:51:58 GMT
WORKDIR /usr/src/perl
# Mon, 25 Sep 2023 20:01:48 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.3.tar.xz -o perl-5.39.3.tar.xz     && echo '93c38a6ff969e3930d7eb08e69a883204a4d835c7122df47c4903950e6fc758a *perl-5.39.3.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.3.tar.xz -C /usr/src/perl     && rm perl-5.39.3.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Mon, 25 Sep 2023 20:01:49 GMT
WORKDIR /usr/src/app
# Mon, 25 Sep 2023 20:01:49 GMT
CMD ["perl5.39.3" "-de0"]
```

-	Layers:
	-	`sha256:d0496e15eebca8286145e6a2cb12c47bb17a28a89cc286a0f7a94763f7713716`  
		Last Modified: Wed, 20 Sep 2023 03:00:01 GMT  
		Size: 53.3 MB (53290747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ffb65667eeb2d3b6696a39c6bee7f8e530b0ca44e4ffdce5129fae1417349ab`  
		Last Modified: Wed, 20 Sep 2023 09:59:26 GMT  
		Size: 15.6 MB (15631894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7bdcba55b78b8074e079cbf178f213bba5f35b2e940b37ef069b50b092ef5f`  
		Last Modified: Wed, 20 Sep 2023 09:59:39 GMT  
		Size: 54.1 MB (54061720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b281045931687b0edd0ac8da65d377622620e8468caf6cc573c45dbbf7611951`  
		Last Modified: Wed, 20 Sep 2023 10:00:06 GMT  
		Size: 172.9 MB (172874403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b6e23b4762781e09acfe749b4c9e2aec50b0d43b1af223af370c5217a7680a`  
		Last Modified: Wed, 20 Sep 2023 12:30:42 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eff5e70fda3a7978364d18a98373c07a58be8572003999bc68a1e5e8b1c8a45`  
		Last Modified: Mon, 25 Sep 2023 20:10:09 GMT  
		Size: 16.0 MB (16031670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2bf0214428355aca9ed105c84383617b30fa8c86cac33baf11ba8363b72f3c0`  
		Last Modified: Mon, 25 Sep 2023 20:10:07 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
