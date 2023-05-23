## `perl:devel`

```console
$ docker pull perl@sha256:c63edfb855469a883fa994dc5b2843336e5988730a86ad18cb0b3fa01ba7973f
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

### `perl:devel` - linux; amd64

```console
$ docker pull perl@sha256:3d7893754d58c4b19fc1662e3133ff0f8aae3f1c2311615b8e24f5764aff6ed0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.9 MB (337867197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4270423aaf77eb655ca4c1b812616deecf2d4635e317128f7bccef43ce58433`
-	Default Command: `["perl5.37.11","-de0"]`

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
# Thu, 04 May 2023 12:38:19 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.37.11.tar.xz -o perl-5.37.11.tar.xz     && echo '3946b00266595ccc44df28275e2fbb7b86c1482934cbeab2780db304a75ffd58 *perl-5.37.11.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.37.11.tar.xz -C /usr/src/perl     && rm perl-5.37.11.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Thu, 04 May 2023 12:38:19 GMT
WORKDIR /
# Thu, 04 May 2023 12:38:19 GMT
CMD ["perl5.37.11" "-de0"]
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
	-	`sha256:63f4197ea835600e623bff7b001195f5d823c13a4fe32f0afb73df6eb2e53a4e`  
		Last Modified: Thu, 04 May 2023 13:00:05 GMT  
		Size: 15.6 MB (15623088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel` - linux; arm variant v5

```console
$ docker pull perl@sha256:dc225f582c8cd96b29e459954f4d098276780f7b7f7c3fcb12c1886db9d9b90e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.2 MB (310212225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e423f35329ba6cfe9d53165775df233a854b0b6b3296d148609078da762d106`
-	Default Command: `["perl5.37.11","-de0"]`

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
# Tue, 23 May 2023 03:40:21 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.37.11.tar.xz -o perl-5.37.11.tar.xz     && echo '3946b00266595ccc44df28275e2fbb7b86c1482934cbeab2780db304a75ffd58 *perl-5.37.11.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.37.11.tar.xz -C /usr/src/perl     && rm perl-5.37.11.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Tue, 23 May 2023 03:40:22 GMT
WORKDIR /
# Tue, 23 May 2023 03:40:22 GMT
CMD ["perl5.37.11" "-de0"]
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
	-	`sha256:9fff8dd2c753b12498ab5d4364540e99a2a534dee771b3f88efb971192c51c1e`  
		Last Modified: Tue, 23 May 2023 04:03:39 GMT  
		Size: 14.9 MB (14910289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel` - linux; arm variant v7

```console
$ docker pull perl@sha256:c6bd7df668e9a7349336b5e6c379cb6e5fc9f6285595df7b5e49def2ef882fce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.5 MB (297472619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94593eb996871a26a28ea3a0a58caa33efef5625493d707e69f5bf58c95a6cad`
-	Default Command: `["perl5.37.11","-de0"]`

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
# Thu, 04 May 2023 10:03:50 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.37.11.tar.xz -o perl-5.37.11.tar.xz     && echo '3946b00266595ccc44df28275e2fbb7b86c1482934cbeab2780db304a75ffd58 *perl-5.37.11.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.37.11.tar.xz -C /usr/src/perl     && rm perl-5.37.11.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Thu, 04 May 2023 10:03:51 GMT
WORKDIR /
# Thu, 04 May 2023 10:03:51 GMT
CMD ["perl5.37.11" "-de0"]
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
	-	`sha256:adabb555b32635a06d7c9ca8c7a306db32a9a0267ca8dcf6bcd8ef09919ce333`  
		Last Modified: Thu, 04 May 2023 10:25:07 GMT  
		Size: 14.7 MB (14715305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:be66bd94ddd25bad80dd7b28aa88f421208d5f64859db6086fe67537910f0e20
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.4 MB (329449337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fda39be6a03b6051c3f3d27bb1ba3f090b23fe828b53629584f70b8cbca9c9b`
-	Default Command: `["perl5.37.11","-de0"]`

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
# Thu, 04 May 2023 05:45:06 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.37.11.tar.xz -o perl-5.37.11.tar.xz     && echo '3946b00266595ccc44df28275e2fbb7b86c1482934cbeab2780db304a75ffd58 *perl-5.37.11.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.37.11.tar.xz -C /usr/src/perl     && rm perl-5.37.11.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Thu, 04 May 2023 05:45:07 GMT
WORKDIR /
# Thu, 04 May 2023 05:45:07 GMT
CMD ["perl5.37.11" "-de0"]
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
	-	`sha256:44a060c3698917597cd010a61cdd26d0c0874706be3d40e2773ba09be9f63a08`  
		Last Modified: Thu, 04 May 2023 06:03:39 GMT  
		Size: 15.6 MB (15560052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel` - linux; 386

```console
$ docker pull perl@sha256:b49e9e6af7e4d847f02d774a406af595410f10bfbcfea6bd197113ba89f4916f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.1 MB (343100576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1f553d455c7492510804aa1e6e349bdf075646631eba8b7e83b609ee8873e72`
-	Default Command: `["perl5.37.11","-de0"]`

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
# Thu, 04 May 2023 10:24:06 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.37.11.tar.xz -o perl-5.37.11.tar.xz     && echo '3946b00266595ccc44df28275e2fbb7b86c1482934cbeab2780db304a75ffd58 *perl-5.37.11.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.37.11.tar.xz -C /usr/src/perl     && rm perl-5.37.11.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Thu, 04 May 2023 10:24:06 GMT
WORKDIR /
# Thu, 04 May 2023 10:24:06 GMT
CMD ["perl5.37.11" "-de0"]
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
	-	`sha256:710efc59cac609072393055442bce507ed6f6d62d348b53c6d7ead24c2b0360c`  
		Last Modified: Thu, 04 May 2023 10:58:23 GMT  
		Size: 15.1 MB (15122319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel` - linux; mips64le

```console
$ docker pull perl@sha256:27523b9c443a9ad8ff3bde74316b88f898e04065727a734ce445b55d924e33a8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.1 MB (316084969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ed3aba13515f9bbc44ec94742d003dabc021493bd58f6bee63bc50fe937ab0f`
-	Default Command: `["perl5.37.11","-de0"]`

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
# Thu, 04 May 2023 14:50:08 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.37.11.tar.xz -o perl-5.37.11.tar.xz     && echo '3946b00266595ccc44df28275e2fbb7b86c1482934cbeab2780db304a75ffd58 *perl-5.37.11.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.37.11.tar.xz -C /usr/src/perl     && rm perl-5.37.11.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Thu, 04 May 2023 14:50:15 GMT
WORKDIR /
# Thu, 04 May 2023 14:50:21 GMT
CMD ["perl5.37.11" "-de0"]
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
	-	`sha256:5dc65bef110ab492bf070930ac636cab1968febf65dc659fadb2be63fcddfe30`  
		Last Modified: Thu, 04 May 2023 15:19:09 GMT  
		Size: 14.8 MB (14825699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel` - linux; ppc64le

```console
$ docker pull perl@sha256:a79003dde93f0e831e8399fa7936178d161cd7c36dcc0079ba21c597fc1622d2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.4 MB (346357805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25c8d34a9038d87efd2550c85dc7220cd2e1374d282b349de62d9310f5dc1cf7`
-	Default Command: `["perl5.37.11","-de0"]`

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
# Thu, 04 May 2023 16:12:59 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.37.11.tar.xz -o perl-5.37.11.tar.xz     && echo '3946b00266595ccc44df28275e2fbb7b86c1482934cbeab2780db304a75ffd58 *perl-5.37.11.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.37.11.tar.xz -C /usr/src/perl     && rm perl-5.37.11.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Thu, 04 May 2023 16:13:00 GMT
WORKDIR /
# Thu, 04 May 2023 16:13:00 GMT
CMD ["perl5.37.11" "-de0"]
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
	-	`sha256:4abd9e44e684f778041f4b5db537be327893289edb282a5a43a6e36089ba16ef`  
		Last Modified: Thu, 04 May 2023 16:25:47 GMT  
		Size: 15.6 MB (15622723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel` - linux; s390x

```console
$ docker pull perl@sha256:722fcc8608717f98b36ec20e45d9156850646213dc4c02e524e20ed05047eb5b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.8 MB (311814669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:569a79ecb9397ffc0b661fc77d73b454ae6e4eac4ddd293dcb7b2e5434c406fb`
-	Default Command: `["perl5.37.11","-de0"]`

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
# Fri, 05 May 2023 03:38:02 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.37.11.tar.xz -o perl-5.37.11.tar.xz     && echo '3946b00266595ccc44df28275e2fbb7b86c1482934cbeab2780db304a75ffd58 *perl-5.37.11.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.37.11.tar.xz -C /usr/src/perl     && rm perl-5.37.11.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Fri, 05 May 2023 03:38:03 GMT
WORKDIR /
# Fri, 05 May 2023 03:38:03 GMT
CMD ["perl5.37.11" "-de0"]
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
	-	`sha256:c40dd611831e3445888c2b25084103a288bfedc28ce2f4bac7b017981f3b33a5`  
		Last Modified: Fri, 05 May 2023 03:47:10 GMT  
		Size: 16.0 MB (15979901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
