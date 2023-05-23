## `perl:5-threaded-bullseye`

```console
$ docker pull perl@sha256:6103fed419fc51fddd66eab18a02edea8d2842b9ca90e0cd9016ee7757e69eb6
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

### `perl:5-threaded-bullseye` - linux; amd64

```console
$ docker pull perl@sha256:e967797d3b9b0e06cf09a0efcf9bb7aca689c4a34ca14020cc220bd8c153d70d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.5 MB (337518473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69e04169d477ff63f932de568a60f5695d42e7fd17535c5579125f4a413a2068`
-	Default Command: `["perl5.36.1","-de0"]`

```dockerfile
# Tue, 02 May 2023 23:46:50 GMT
ADD file:fc290cf8ddb984325474583faa79c5a98c5ea0ec7f606bf360251f63acecf389 in / 
# Tue, 02 May 2023 23:46:51 GMT
CMD ["bash"]
# Wed, 03 May 2023 19:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 19:58:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 19:59:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 11:27:10 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 04 May 2023 11:27:10 GMT
WORKDIR /usr/src/perl
# Thu, 04 May 2023 11:43:35 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.1.tar.xz -o perl-5.36.1.tar.xz     && echo 'bd91217ea8a8c8b81f21ebbb6cefdf0d13ae532013f944cdece2cd51aef4b6a7 *perl-5.36.1.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.1.tar.xz -C /usr/src/perl     && rm perl-5.36.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Thu, 04 May 2023 11:43:35 GMT
WORKDIR /
# Thu, 04 May 2023 11:43:35 GMT
CMD ["perl5.36.1" "-de0"]
```

-	Layers:
	-	`sha256:918547b9432687b1e1d238e82dc1e0ea0b736aafbf3c402eea98c6db81a9cb65`  
		Last Modified: Tue, 02 May 2023 23:49:58 GMT  
		Size: 55.0 MB (55049070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d79063a01c561833dc6546d4e647fda0121a59e1a9a17874a3e30854555475e`  
		Last Modified: Wed, 03 May 2023 20:13:04 GMT  
		Size: 15.8 MB (15760340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eedd9c5abf7e5f63753a5e788cb0872a715fa1141e8ce5ea87638e6cd370a41`  
		Last Modified: Wed, 03 May 2023 20:13:22 GMT  
		Size: 54.6 MB (54584552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cdadd40055fb82fef74a0a38f29fb1ee7b6922e18370ebdc3502ec66f79fa3f`  
		Last Modified: Wed, 03 May 2023 20:13:55 GMT  
		Size: 196.8 MB (196849980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1ebd6889fb6a38eaf6ba56596b0c1ae222d98afde0c0d8322ed23786b15173`  
		Last Modified: Thu, 04 May 2023 12:56:42 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94367a685d17f3c98238e437f6c3e268b2cee9f8657ab2bb841e91da2410982`  
		Last Modified: Thu, 04 May 2023 12:57:31 GMT  
		Size: 15.3 MB (15274364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-threaded-bullseye` - linux; arm variant v5

```console
$ docker pull perl@sha256:947a8a4e70a08641f9f43a8f5758a0c12bb0420083d8cce1bd2f546f08789347
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.8 MB (309839859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cf1214afabbe50559c30d716b4c8b094ce63762d8761a1a8a03684865fb3bdd`
-	Default Command: `["perl5.36.1","-de0"]`

```dockerfile
# Tue, 23 May 2023 00:48:32 GMT
ADD file:9572a8fcb9c86e8a9dbfe623c732cc4ba1c4f5670490191a7e639a272d5b6e97 in / 
# Tue, 23 May 2023 00:48:33 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:15:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:16:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:18:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:25:18 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 23 May 2023 02:25:18 GMT
WORKDIR /usr/src/perl
# Tue, 23 May 2023 02:42:37 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.1.tar.xz -o perl-5.36.1.tar.xz     && echo 'bd91217ea8a8c8b81f21ebbb6cefdf0d13ae532013f944cdece2cd51aef4b6a7 *perl-5.36.1.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.1.tar.xz -C /usr/src/perl     && rm perl-5.36.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Tue, 23 May 2023 02:42:37 GMT
WORKDIR /
# Tue, 23 May 2023 02:42:37 GMT
CMD ["perl5.36.1" "-de0"]
```

-	Layers:
	-	`sha256:b053976742ca5b01bcefb7df8fc77a58d0becb4ce508792491574463930569c4`  
		Last Modified: Tue, 23 May 2023 00:50:55 GMT  
		Size: 52.5 MB (52546536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae14fc3c88d12fab00e99f27b0c64eebba1d2189ed894e16dc646bb11ce7b1e7`  
		Last Modified: Tue, 23 May 2023 01:21:39 GMT  
		Size: 15.4 MB (15368887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a1500719862236236c344334787e4d127985e5b0c19ab45a58919bd48dc45b`  
		Last Modified: Tue, 23 May 2023 01:21:57 GMT  
		Size: 52.3 MB (52340730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f9974f69bcb0ce7b86ce364224c7b0bb40e305c4765d2d082e13c6961a563e`  
		Last Modified: Tue, 23 May 2023 01:22:36 GMT  
		Size: 175.0 MB (175045616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f3637b12c91405769832c0b499e3bbd37bd6727a7a238e66a5157b238678ce`  
		Last Modified: Tue, 23 May 2023 03:59:26 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e462c6c3339b71185bae6dbb5ebe070d845db550735642ab0f3d26433275b23e`  
		Last Modified: Tue, 23 May 2023 04:00:36 GMT  
		Size: 14.5 MB (14537923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-threaded-bullseye` - linux; arm variant v7

```console
$ docker pull perl@sha256:fd411871bd421fb18dd6f1f65b38c645cd2cd15075de8d8d131ff8a077876250
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.1 MB (297097715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:811e716c4d594c32b5474685de46de0e686a7c7ac0d3b0e5dec409b32bb7d8b0`
-	Default Command: `["perl5.36.1","-de0"]`

```dockerfile
# Tue, 02 May 2023 23:47:46 GMT
ADD file:668ced72eb3825a6cfd123f77fed6c64b8ad5bf1f4aa8e78ede9512198ca65ad in / 
# Tue, 02 May 2023 23:47:47 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:53:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:53:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:54:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 08:54:21 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 04 May 2023 08:54:21 GMT
WORKDIR /usr/src/perl
# Thu, 04 May 2023 09:10:33 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.1.tar.xz -o perl-5.36.1.tar.xz     && echo 'bd91217ea8a8c8b81f21ebbb6cefdf0d13ae532013f944cdece2cd51aef4b6a7 *perl-5.36.1.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.1.tar.xz -C /usr/src/perl     && rm perl-5.36.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Thu, 04 May 2023 09:10:33 GMT
WORKDIR /
# Thu, 04 May 2023 09:10:33 GMT
CMD ["perl5.36.1" "-de0"]
```

-	Layers:
	-	`sha256:755944445ece6eac276e067f465680b57daac59a0ed9ce97e7c501f1cde8621d`  
		Last Modified: Tue, 02 May 2023 23:51:06 GMT  
		Size: 50.2 MB (50210011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7979fe7914af9b87a93e67c054d2be5b1a2a0b052f4257f06ce7dc8c03570892`  
		Last Modified: Wed, 03 May 2023 22:09:00 GMT  
		Size: 14.9 MB (14868556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8937bdf171eebc34da9237ba41374e2d9cfe64d3c99485469a9f2af16f53ca2`  
		Last Modified: Wed, 03 May 2023 22:09:18 GMT  
		Size: 50.4 MB (50355586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a897e09a5d8e6a7f113828ec77a909ec9cfa4629bc4998204328f6d665d4acac`  
		Last Modified: Wed, 03 May 2023 22:09:49 GMT  
		Size: 167.3 MB (167322995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0019bb8f9fad73fce14d1124caebac89e918fdc65d698fec88552f8748fa6501`  
		Last Modified: Thu, 04 May 2023 10:21:42 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b1a5de2087a339364f286bfc8191b2423d0964742bf6956ee260ff69a8e851`  
		Last Modified: Thu, 04 May 2023 10:22:33 GMT  
		Size: 14.3 MB (14340401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-threaded-bullseye` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:b9a021ccb00b2cf391d8e15b73cc5a1de7d822b95e7039d19545c00059ed8b5a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.1 MB (329085052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e7fff892cd8e6a46e167e096d4494ae886a4f0319029f8955e21256ddca9d77`
-	Default Command: `["perl5.36.1","-de0"]`

```dockerfile
# Wed, 03 May 2023 00:22:41 GMT
ADD file:f930fdb659332a615b0042ca415d6d7feda9ba6b2f58222e3e5bbed326db4d40 in / 
# Wed, 03 May 2023 00:22:42 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:21:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 17:21:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 17:22:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 04:46:14 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 04 May 2023 04:46:14 GMT
WORKDIR /usr/src/perl
# Thu, 04 May 2023 04:59:50 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.1.tar.xz -o perl-5.36.1.tar.xz     && echo 'bd91217ea8a8c8b81f21ebbb6cefdf0d13ae532013f944cdece2cd51aef4b6a7 *perl-5.36.1.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.1.tar.xz -C /usr/src/perl     && rm perl-5.36.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Thu, 04 May 2023 04:59:50 GMT
WORKDIR /
# Thu, 04 May 2023 04:59:50 GMT
CMD ["perl5.36.1" "-de0"]
```

-	Layers:
	-	`sha256:d677c78be691f8dcbe9d44ce576b97ad205b3dd78557dc62794e59eb19553ee9`  
		Last Modified: Wed, 03 May 2023 00:25:31 GMT  
		Size: 53.7 MB (53692705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73587d290df17347645f166c8385f0a2d320a31f4803658f619f2887a5d88faf`  
		Last Modified: Wed, 03 May 2023 17:36:59 GMT  
		Size: 15.7 MB (15746737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd49b43770afa984b42a50282487e41b4ca05ba0e9f8bf233e6fc6d2fa99353e`  
		Last Modified: Wed, 03 May 2023 17:37:15 GMT  
		Size: 54.7 MB (54675990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a96e84daab7feb81c20a699d776f6cb02383bdcc7f2b02d4f3af942e740c2a`  
		Last Modified: Wed, 03 May 2023 17:37:47 GMT  
		Size: 189.8 MB (189773685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8cdeaac08960251f07e280a22facc797b1ba5e465cdc229cd22b0476ac6a96`  
		Last Modified: Thu, 04 May 2023 06:00:21 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c280f22c0fbd3f06383bd715b2f4ac4f357e3c2c7d5dea7d28e0a97e711d215a`  
		Last Modified: Thu, 04 May 2023 06:01:09 GMT  
		Size: 15.2 MB (15195767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-threaded-bullseye` - linux; 386

```console
$ docker pull perl@sha256:0feb4becb9ce8c3d7318dd2b95337c8790c92ffe52c0a73532ddf4a06da65add
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **342.8 MB (342787857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09cdfa26b45281f4456438c30114c4e1aae4415904cf5c15432c9682b4065a1e`
-	Default Command: `["perl5.36.1","-de0"]`

```dockerfile
# Wed, 03 May 2023 00:00:45 GMT
ADD file:59d53253d7691be0330c735eb4b57791a8fc5894572d3deaeb7138cce45132ad in / 
# Wed, 03 May 2023 00:00:46 GMT
CMD ["bash"]
# Wed, 03 May 2023 22:28:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 22:29:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 22:30:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 08:20:01 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 04 May 2023 08:20:01 GMT
WORKDIR /usr/src/perl
# Thu, 04 May 2023 08:49:03 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.1.tar.xz -o perl-5.36.1.tar.xz     && echo 'bd91217ea8a8c8b81f21ebbb6cefdf0d13ae532013f944cdece2cd51aef4b6a7 *perl-5.36.1.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.1.tar.xz -C /usr/src/perl     && rm perl-5.36.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Thu, 04 May 2023 08:49:03 GMT
WORKDIR /
# Thu, 04 May 2023 08:49:03 GMT
CMD ["perl5.36.1" "-de0"]
```

-	Layers:
	-	`sha256:6ac0eb37fce5e6fca952bf804df5de5ebb63724d4d44bf23abc5d5736ee32afd`  
		Last Modified: Wed, 03 May 2023 00:04:44 GMT  
		Size: 56.0 MB (56029150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de21dcd769e703c034c16b0e5b92aecd56468d2eb0a9c1719775735654f8cf3`  
		Last Modified: Wed, 03 May 2023 22:36:04 GMT  
		Size: 16.3 MB (16263234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed46c5383778b8d3b20b09e9296d4d8ecdb363c3436f0188d69ef066bed07cbb`  
		Last Modified: Wed, 03 May 2023 22:36:26 GMT  
		Size: 55.9 MB (55922651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa5b0eba28a6e85b96b76f161af708d6f1d0015d7e7955e025f7fcddc506141`  
		Last Modified: Wed, 03 May 2023 22:37:11 GMT  
		Size: 199.8 MB (199763056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d78abfc63f6b23a746817d59932bd2afc1caa6b5f25cad0109a47a5f7e1382aa`  
		Last Modified: Thu, 04 May 2023 10:54:43 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5618ebcdcb2448e45444e6cd20a18ce3141c458219911e72b61a108948f5957`  
		Last Modified: Thu, 04 May 2023 10:55:36 GMT  
		Size: 14.8 MB (14809600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-threaded-bullseye` - linux; mips64le

```console
$ docker pull perl@sha256:215710cc68a3a33061a2d6b80e7af9876698005c1b1495d6541441be77ad80cf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **315.8 MB (315765711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9425c481b0ffe141a0e815b96edcb608c3890b30c1418abe56a98e34cfcce60b`
-	Default Command: `["perl5.36.1","-de0"]`

```dockerfile
# Tue, 02 May 2023 23:49:00 GMT
ADD file:578ecc56a9b7fe8d8ebea195fcf6c3a8d78941e9c4b5da71f8b4b821b6db9f87 in / 
# Tue, 02 May 2023 23:49:06 GMT
CMD ["bash"]
# Thu, 04 May 2023 01:06:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 01:08:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 01:14:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 12:11:18 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 04 May 2023 12:11:24 GMT
WORKDIR /usr/src/perl
# Thu, 04 May 2023 12:57:50 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.1.tar.xz -o perl-5.36.1.tar.xz     && echo 'bd91217ea8a8c8b81f21ebbb6cefdf0d13ae532013f944cdece2cd51aef4b6a7 *perl-5.36.1.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.1.tar.xz -C /usr/src/perl     && rm perl-5.36.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Thu, 04 May 2023 12:57:57 GMT
WORKDIR /
# Thu, 04 May 2023 12:58:03 GMT
CMD ["perl5.36.1" "-de0"]
```

-	Layers:
	-	`sha256:4753f7ffbf9149ce1d9cc543018c00a2946e14c08b1a2aa37a0ac347d08b0e29`  
		Last Modified: Tue, 02 May 2023 23:57:30 GMT  
		Size: 53.3 MB (53261131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617edd93224e221bb1aa9a0bddc7d1dbef99ad4432443e495de9f03a672bcf1c`  
		Last Modified: Thu, 04 May 2023 01:26:04 GMT  
		Size: 15.7 MB (15724646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba522bd98dad310cd8745185df0afdc5fe59b44d154b9e1c7830557cf77657da`  
		Last Modified: Thu, 04 May 2023 01:26:49 GMT  
		Size: 53.3 MB (53306639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc2b2f70fe61dbefa21d8bd20d5d8c1534f993aa9c16e96c57b6c6ff8c89826b`  
		Last Modified: Thu, 04 May 2023 01:28:44 GMT  
		Size: 179.0 MB (178966719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c4babf59fdce67047e8c116324061d35f52bcf6cfee7ea14d9cafde110a502`  
		Last Modified: Thu, 04 May 2023 15:15:49 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b99e48a2cb6d40bd1e002dde543652025d7984efd347a06231f47e4172385640`  
		Last Modified: Thu, 04 May 2023 15:16:42 GMT  
		Size: 14.5 MB (14506441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-threaded-bullseye` - linux; ppc64le

```console
$ docker pull perl@sha256:715f0c6d618d36b57356882cfc9aa127ea9cea7dc9958e9d675b9379c662f6d7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.1 MB (346052662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02307141a74d85b68dda3d0cba9174317e4b44a41ada122f41988c3f11d4dba3`
-	Default Command: `["perl5.36.1","-de0"]`

```dockerfile
# Wed, 03 May 2023 00:31:28 GMT
ADD file:39e4cb0fbb759c45690e34c0392acb89ac2b180e261843426f24ce0fe0189e84 in / 
# Wed, 03 May 2023 00:31:32 GMT
CMD ["bash"]
# Wed, 03 May 2023 23:13:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 23:14:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 23:16:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 15:10:11 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 04 May 2023 15:10:12 GMT
WORKDIR /usr/src/perl
# Thu, 04 May 2023 15:28:34 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.1.tar.xz -o perl-5.36.1.tar.xz     && echo 'bd91217ea8a8c8b81f21ebbb6cefdf0d13ae532013f944cdece2cd51aef4b6a7 *perl-5.36.1.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.1.tar.xz -C /usr/src/perl     && rm perl-5.36.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Thu, 04 May 2023 15:28:35 GMT
WORKDIR /
# Thu, 04 May 2023 15:28:36 GMT
CMD ["perl5.36.1" "-de0"]
```

-	Layers:
	-	`sha256:0c356fc795c1bdfb3883bd87c64008fffdc0d8bdc8f0ecb386016a31fe5864fb`  
		Last Modified: Wed, 03 May 2023 00:36:26 GMT  
		Size: 58.9 MB (58924002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9eaacc3a94a866678cbdd938b63593e68d36a42077af256c70dd182c240ec01`  
		Last Modified: Wed, 03 May 2023 23:37:02 GMT  
		Size: 16.8 MB (16752867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35c5701220ac1341c97c6b9c8187191a0b07d8d046ba9046213d80c10b2580d`  
		Last Modified: Wed, 03 May 2023 23:37:29 GMT  
		Size: 58.9 MB (58865156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea046ab7c583867ab12e083559705bf801d7097ee514dd7f6626c65a2a9f6df`  
		Last Modified: Wed, 03 May 2023 23:38:27 GMT  
		Size: 196.2 MB (196192888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdfdf676dc23f6c965125ccc00243c389af8801bddd57001df1377fce3f6fcd1`  
		Last Modified: Thu, 04 May 2023 16:23:11 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b741b91755c5cfe683f28fb3815733bf1c3a3e636c998e86a434c3d9986fb0`  
		Last Modified: Thu, 04 May 2023 16:23:51 GMT  
		Size: 15.3 MB (15317580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-threaded-bullseye` - linux; s390x

```console
$ docker pull perl@sha256:015641a8e5a54558bc8f1799d016a3e28fdb4365e431b48d2d0a0bbc36e9d424
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.5 MB (311465967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35fa3712a7da579edb77d9b68055d16a8d7aa2f225f3d8adbc0e17aa89582929`
-	Default Command: `["perl5.36.1","-de0"]`

```dockerfile
# Wed, 03 May 2023 03:41:38 GMT
ADD file:c518f614279e4b34edf6331c6ed36be5ff220ae28cf9bda3433158c45c858caa in / 
# Wed, 03 May 2023 03:41:43 GMT
CMD ["bash"]
# Wed, 03 May 2023 22:20:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 22:20:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 22:21:16 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 05 May 2023 02:55:54 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Fri, 05 May 2023 02:55:54 GMT
WORKDIR /usr/src/perl
# Fri, 05 May 2023 03:08:09 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.1.tar.xz -o perl-5.36.1.tar.xz     && echo 'bd91217ea8a8c8b81f21ebbb6cefdf0d13ae532013f944cdece2cd51aef4b6a7 *perl-5.36.1.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.1.tar.xz -C /usr/src/perl     && rm perl-5.36.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Fri, 05 May 2023 03:08:10 GMT
WORKDIR /
# Fri, 05 May 2023 03:08:10 GMT
CMD ["perl5.36.1" "-de0"]
```

-	Layers:
	-	`sha256:c05abc724fd71022253a33351707dac122d940b2d0569f0bf779ac1416f31abd`  
		Last Modified: Wed, 03 May 2023 03:44:45 GMT  
		Size: 53.3 MB (53282138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3f3844dec99042b575308abefcfc0fe7af51d4563b2a48c3864c89cddfff77`  
		Last Modified: Wed, 03 May 2023 22:31:51 GMT  
		Size: 15.6 MB (15631901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e4adc5f823d8824e5e89f648778aa7e0adf12c040b52537020264363550684`  
		Last Modified: Wed, 03 May 2023 22:32:05 GMT  
		Size: 54.1 MB (54061763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab29723cb580b0655eb4ef28c3901bfcf5cdaa362ef71bd0b41b323e848cf212`  
		Last Modified: Wed, 03 May 2023 22:32:31 GMT  
		Size: 172.9 MB (172858800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2969d5d6868f131a32af3771c1576a69928d81347b8d3b0e0d47d79dd7ca916`  
		Last Modified: Fri, 05 May 2023 03:45:46 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a469e35493567645a83be8859345e9be616ada4312bc356cc3647836c5349d`  
		Last Modified: Fri, 05 May 2023 03:46:08 GMT  
		Size: 15.6 MB (15631199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
