## `perl:buster`

```console
$ docker pull perl@sha256:3885949a6d0da48012b7cde85ace611ae4d0c2897a8ab64b11953b0b95016811
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `perl:buster` - linux; amd64

```console
$ docker pull perl@sha256:c0d81277aa27c13f0e0ac17c7916ee3f08a0fe609a54b365f3344c17cf01c6de
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.5 MB (327514621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2f618eaf7e6a776c65c7522cb6ea4d8cf757ee89106320493bf1e4e13880adc`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Tue, 19 Dec 2023 01:21:00 GMT
ADD file:e5e3f2fedf4fa6382f3bbf6203060ba68df1aadc7ebfa3350df20bf31b102f0e in / 
# Tue, 19 Dec 2023 01:21:01 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 04:35:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 04:35:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 04:36:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 08:30:06 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 19 Dec 2023 08:30:06 GMT
WORKDIR /usr/src/perl
# Tue, 19 Dec 2023 08:35:36 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 19 Dec 2023 08:35:36 GMT
WORKDIR /usr/src/app
# Tue, 19 Dec 2023 08:35:36 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:30b73a2ffaab3c39355a8bcc5eae8ba1465bd7d9467f197b91f7635816b16bc9`  
		Last Modified: Tue, 19 Dec 2023 01:25:58 GMT  
		Size: 50.5 MB (50500409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b38726aed64a0804777af4106983e9686ea639add75dae8538ecaad0c0e6a58`  
		Last Modified: Tue, 19 Dec 2023 04:43:15 GMT  
		Size: 17.6 MB (17583877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea388039df9c5c51dda7a2d1d6908eac88ae220452b81495739aff1428c1f847`  
		Last Modified: Tue, 19 Dec 2023 04:43:30 GMT  
		Size: 51.9 MB (51874049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dd4fbda45c5750b2808bd8a3385ffd64974432821cfa42ae41da8450163d1f1`  
		Last Modified: Tue, 19 Dec 2023 04:44:01 GMT  
		Size: 191.9 MB (191908351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf651e796cae79c3698068fabc40132f43945d2832d787146b161a36f17d5924`  
		Last Modified: Tue, 19 Dec 2023 12:24:03 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c32c278b38e49945fe9bf09f9bd0fa74881b6a02806b5b94e11221dc291758`  
		Last Modified: Tue, 19 Dec 2023 12:24:06 GMT  
		Size: 15.6 MB (15647602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7017aa188c7b7459bc4468242840db4a033a90b8d0393473de7929d7df4f61fc`  
		Last Modified: Tue, 19 Dec 2023 12:24:03 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:buster` - linux; arm variant v7

```console
$ docker pull perl@sha256:975b1f9703fcc30976479e051277df17f0afc5e331346b031bad2316fbc3fa64
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.5 MB (292467451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c56ef24b04de992a3970dfd4523285bbe6308a495f48b1687001a3e914967509`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Tue, 21 Nov 2023 03:58:12 GMT
ADD file:e69e944c7b28ca650586e3fa2bcb51c4c99491167bee97c4ab32982eeab66750 in / 
# Tue, 21 Nov 2023 03:58:13 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 14:07:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 14:07:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 14:08:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 14:39:19 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 21 Nov 2023 14:39:19 GMT
WORKDIR /usr/src/perl
# Thu, 30 Nov 2023 19:13:16 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Thu, 30 Nov 2023 19:13:16 GMT
WORKDIR /usr/src/app
# Thu, 30 Nov 2023 19:13:17 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:859d411365ce23ca0a7fbddedc1babff0039e814c09756ad01c59527ebe62dc8`  
		Last Modified: Tue, 21 Nov 2023 04:02:56 GMT  
		Size: 46.0 MB (45966309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:934694a3a163c892d9694911102dffb8ebb1f12f68a415dcb5d3541126843231`  
		Last Modified: Tue, 21 Nov 2023 14:16:09 GMT  
		Size: 16.2 MB (16215654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1de4e1a75f9848810a987d71b29b0bba9fe490d66f3b182aececdef19ab65af`  
		Last Modified: Tue, 21 Nov 2023 14:16:25 GMT  
		Size: 47.4 MB (47410944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c1aa8dd2c0542f76fcbe22cb4412107b5a6ba0a5180b163a4b0c6fe5a87636`  
		Last Modified: Tue, 21 Nov 2023 14:16:55 GMT  
		Size: 168.1 MB (168106662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b651d9d5b9e9b601d65e99ce01fe00993b66ade961f8fa16610e1c7b414d4b`  
		Last Modified: Tue, 21 Nov 2023 16:27:58 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a0ca0eb3581d3dcc6b497d8162e00e8663b4603e5f0ede7ad4f669adc973a1`  
		Last Modified: Thu, 30 Nov 2023 22:07:35 GMT  
		Size: 14.8 MB (14767549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71dba2fdecb742cfd202adf42abf0c76d684cd0180f3a2ba157bc3ea3b96f067`  
		Last Modified: Thu, 30 Nov 2023 22:07:31 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:buster` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:e16a1ca872c3c2868b6ae6e0ff1238d4e3496752c3b143c4acb0bc7d192ced07
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.0 MB (318021575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cac5a72f328db9c980cc86ee272b9c6004b71c57645d5e0a26195ade63bf51da`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:31 GMT
ADD file:df5e5dd39efc6ae3cc9132f6ca6bb569731f7a37cf4b41f87bcb7aa1ba9771e8 in / 
# Tue, 19 Dec 2023 01:41:32 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 11:36:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 11:36:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 11:37:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 14:39:20 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 19 Dec 2023 14:39:20 GMT
WORKDIR /usr/src/perl
# Tue, 19 Dec 2023 14:43:41 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 19 Dec 2023 14:43:41 GMT
WORKDIR /usr/src/app
# Tue, 19 Dec 2023 14:43:41 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:93507f9712ced9fbfd0d0f689cf7b55fb245cef88530c07ac5dc5cad20fa889d`  
		Last Modified: Tue, 19 Dec 2023 01:45:40 GMT  
		Size: 49.3 MB (49289026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d548003bf6042e58cd00488bd9dec02acb1fd956797b04f2aacc5f11f2e1a6eb`  
		Last Modified: Tue, 19 Dec 2023 11:44:06 GMT  
		Size: 17.5 MB (17455285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64eb6e6e06a1244843fc7372bcd9203e91c1434ac505900a1ce0f6c242e66f8c`  
		Last Modified: Tue, 19 Dec 2023 11:44:20 GMT  
		Size: 52.2 MB (52209354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aafa5b1d6e0dc63601c97af2f608815a7d2888e261e971240e521209e0d5aad`  
		Last Modified: Tue, 19 Dec 2023 11:44:44 GMT  
		Size: 183.5 MB (183475777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:046cb7b550b55297b3d5b48a708dffb1c93004ed3c689b2432043deba5f1a92c`  
		Last Modified: Tue, 19 Dec 2023 16:05:30 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:125b385d771ebe591c9a99aac9fc03afa8bb60863d485b426449ed0e0f755aa8`  
		Last Modified: Tue, 19 Dec 2023 16:05:32 GMT  
		Size: 15.6 MB (15591800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd201ee1ed9144002dc02b676a18ee14eb7c61916fb4ef3ad3ca14bf3a098b7`  
		Last Modified: Tue, 19 Dec 2023 16:05:30 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:buster` - linux; 386

```console
$ docker pull perl@sha256:46c5b2dc50446d674cdca9aa2c877399085345658b9c1d2fa0163439c4552035
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.4 MB (336437175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbd66f433a6cf1f8a635ffdd443ea1c4b35d74e48b31b3bb265fc9cbd94f6708`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Tue, 19 Dec 2023 01:39:40 GMT
ADD file:4c009b0d408e3df297246382d87b0be68c34886e13ed79ba47feb8ff51acb863 in / 
# Tue, 19 Dec 2023 01:39:41 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:28:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:29:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:30:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 09:55:39 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 19 Dec 2023 09:55:40 GMT
WORKDIR /usr/src/perl
# Tue, 19 Dec 2023 10:05:04 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 19 Dec 2023 10:05:04 GMT
WORKDIR /usr/src/app
# Tue, 19 Dec 2023 10:05:04 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:8d351f5ab6958b8ca5f2b8e463c49cba65be4285ead8bdbc1378b5ce2c8cd736`  
		Last Modified: Tue, 19 Dec 2023 01:44:53 GMT  
		Size: 51.3 MB (51255444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d92ef590e153dccaba28c33feb3c21c9c8fd8e2f421a31659859531d5368bad9`  
		Last Modified: Tue, 19 Dec 2023 03:38:54 GMT  
		Size: 18.1 MB (18099404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8899b7af5c2eb679d56ee31148fbe43b672bf3bdec30689f9fe7cbcd3698d34e`  
		Last Modified: Tue, 19 Dec 2023 03:39:14 GMT  
		Size: 53.5 MB (53487920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da21dce6f09c3eeff5569d78b6aa0e3607d894e61dd8a5d8f600c5215807c569`  
		Last Modified: Tue, 19 Dec 2023 03:39:59 GMT  
		Size: 198.4 MB (198448371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed552913f3fd5bce9f6455bc75a7bc8e7b8a08d1ade76238fbaee3f70498db7`  
		Last Modified: Tue, 19 Dec 2023 16:35:33 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d6e33725b77de928103bb78c03a9506a871a34a11a10924734f33a648436de`  
		Last Modified: Tue, 19 Dec 2023 16:35:38 GMT  
		Size: 15.1 MB (15145702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92122556c54c63c15e73707f505791df6716d2bb4e9b41da31b5f8a2343b3ff`  
		Last Modified: Tue, 19 Dec 2023 16:35:33 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
