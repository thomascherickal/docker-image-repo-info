## `perl:threaded`

```console
$ docker pull perl@sha256:4afa0a5e22dc793d0be2d160c08abe5738607e30679f00849adeb4095768d069
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

### `perl:threaded` - linux; amd64

```console
$ docker pull perl@sha256:6b357e50efe133a022b81b90a7f86bd993eaea8042e877425cd887ebc226e779
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.8 MB (337809595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eff0f97003d52a5b237333b02db8886b4e65ba4db95ca781dbefdcbdd4da16a4`
-	Default Command: `["perl5.36.0","-de0"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:21 GMT
ADD file:c13b430c8699df107ffd9ea5230b92238bc037a8e1cbbe35d6ab664941d575da in / 
# Wed, 21 Dec 2022 01:20:22 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 11:13:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:13:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 21 Dec 2022 11:14:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:15:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 23:21:32 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 21 Dec 2022 23:21:32 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Wed, 21 Dec 2022 23:21:32 GMT
WORKDIR /usr/src/perl
# Wed, 21 Dec 2022 23:38:41 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.0.tar.xz -o perl-5.36.0.tar.xz     && echo '0f386dccbee8e26286404b2cca144e1005be65477979beb9b1ba272d4819bcf0 *perl-5.36.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.0.tar.xz -C /usr/src/perl     && rm perl-5.36.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Wed, 21 Dec 2022 23:38:42 GMT
WORKDIR /
# Wed, 21 Dec 2022 23:38:42 GMT
CMD ["perl5.36.0" "-de0"]
```

-	Layers:
	-	`sha256:32de3c850997ce03b6ff4ae8fb00b34b9d7d7f9a35bfcdb8538e22cc7b77c29d`  
		Last Modified: Wed, 21 Dec 2022 01:24:10 GMT  
		Size: 55.0 MB (55025166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa1d4c8d85a4e064e50cea74d4aa848dc5fc275aef223fcc1f21fbdb1b5dd182`  
		Last Modified: Wed, 21 Dec 2022 11:21:24 GMT  
		Size: 5.2 MB (5163298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c796299bbbddc7aeada9539a4e7874a75fa2b6ff421f8d5ad40f227b40ab4d86`  
		Last Modified: Wed, 21 Dec 2022 11:21:24 GMT  
		Size: 10.9 MB (10876681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81283a9569ad5e90773f038daedd0d565810ca5935eec8f53b8bcb6a199030d6`  
		Last Modified: Wed, 21 Dec 2022 11:21:43 GMT  
		Size: 54.6 MB (54584566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b38700e7fb2cdfac79b15e4c1691a80fe6b4101c7b7fea66b9e7cd64d961cf`  
		Last Modified: Wed, 21 Dec 2022 11:22:19 GMT  
		Size: 196.9 MB (196877183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c621b329def930a947d08a207ada2faa373cf567d37afc61e71fc2ddc81a40`  
		Last Modified: Thu, 22 Dec 2022 00:31:07 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dff339e6ef6accc07c3fd6509e16dbc1493abee5544f63a38cc852a0dbc1a7a`  
		Last Modified: Thu, 22 Dec 2022 00:31:54 GMT  
		Size: 15.3 MB (15282499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded` - linux; arm variant v5

```console
$ docker pull perl@sha256:7e68005a6b0c315423eadd181c30e69968dcf2d46a29979baa8136111f2addfa
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.1 MB (310093759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:629f5b71ea2e026fa73ae32f603be21052f45264a0431d7d598eab51851f2d23`
-	Default Command: `["perl5.36.0","-de0"]`

```dockerfile
# Wed, 21 Dec 2022 01:48:53 GMT
ADD file:81ccc74e0ea343972e2f3f46d2da7e9b808d9718be44d4afa7bec6904b7ab9c6 in / 
# Wed, 21 Dec 2022 01:48:55 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:19:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:19:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 21 Dec 2022 02:20:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:21:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 09:44:28 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 21 Dec 2022 09:44:28 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Wed, 21 Dec 2022 09:44:29 GMT
WORKDIR /usr/src/perl
# Wed, 21 Dec 2022 10:03:46 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.0.tar.xz -o perl-5.36.0.tar.xz     && echo '0f386dccbee8e26286404b2cca144e1005be65477979beb9b1ba272d4819bcf0 *perl-5.36.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.0.tar.xz -C /usr/src/perl     && rm perl-5.36.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Wed, 21 Dec 2022 10:03:46 GMT
WORKDIR /
# Wed, 21 Dec 2022 10:03:46 GMT
CMD ["perl5.36.0" "-de0"]
```

-	Layers:
	-	`sha256:89b6e4f9f2f811282495a047e873c20d6ac2d53c72ad576a6907b1449eb3e635`  
		Last Modified: Wed, 21 Dec 2022 01:53:30 GMT  
		Size: 52.5 MB (52529974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f876819c458b2871612c5a4647e4ff5da60c388225364d795cff2bcbc79491c`  
		Last Modified: Wed, 21 Dec 2022 02:26:35 GMT  
		Size: 5.1 MB (5070971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b790eb42ca76f8c8169b2b48345e75bf2e91e66ff8f5ed85b560d3be62bb79`  
		Last Modified: Wed, 21 Dec 2022 02:26:36 GMT  
		Size: 10.6 MB (10573821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a04b0bdd115f51f2790ff07f31d1297629f80cb94408d6b5b32fd0f3993220`  
		Last Modified: Wed, 21 Dec 2022 02:26:59 GMT  
		Size: 52.3 MB (52321330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e34d4b257cf88984f2609c2b3e1d3b6cf4bd791efe390cee5c480f5410b7975`  
		Last Modified: Wed, 21 Dec 2022 02:27:43 GMT  
		Size: 175.0 MB (175048287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6072a299d1b4f5e33b31944e7527505cc93bd59dd3c3fc1f2436d145820b5021`  
		Last Modified: Wed, 21 Dec 2022 11:05:48 GMT  
		Size: 180.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0be4768675526d34f90fece0be47a741e539cd58d4d37408152342eb6e26fa`  
		Last Modified: Wed, 21 Dec 2022 11:07:09 GMT  
		Size: 14.5 MB (14549196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded` - linux; arm variant v7

```console
$ docker pull perl@sha256:b94953ef7a1b620c16f01b47b9364d97d590cf9a97b1468f81abd558e47c1678
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.4 MB (297385749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:163ec03501a82b6eaa09acb81df7fac28448fc62b192f2bf3cd4b96b8f45189f`
-	Default Command: `["perl5.36.0","-de0"]`

```dockerfile
# Wed, 21 Dec 2022 01:58:09 GMT
ADD file:4b6f71680de34554595f062f9e52037b48edf19ca8f34c75877caa85c42caad3 in / 
# Wed, 21 Dec 2022 01:58:10 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:27:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:27:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 21 Dec 2022 02:28:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:29:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 03:14:38 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 21 Dec 2022 03:14:39 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Wed, 21 Dec 2022 03:14:39 GMT
WORKDIR /usr/src/perl
# Wed, 21 Dec 2022 03:47:29 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.0.tar.xz -o perl-5.36.0.tar.xz     && echo '0f386dccbee8e26286404b2cca144e1005be65477979beb9b1ba272d4819bcf0 *perl-5.36.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.0.tar.xz -C /usr/src/perl     && rm perl-5.36.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Wed, 21 Dec 2022 03:47:29 GMT
WORKDIR /
# Wed, 21 Dec 2022 03:47:29 GMT
CMD ["perl5.36.0" "-de0"]
```

-	Layers:
	-	`sha256:706bb1d74512e1fb9ba97aa9212a32d07726fbfe77e4c7e609406d2065418f57`  
		Last Modified: Wed, 21 Dec 2022 02:04:37 GMT  
		Size: 50.2 MB (50190771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6680cc86b286376b17781e60087f333900d6195e47181a19cc371bdfcabcaa81`  
		Last Modified: Wed, 21 Dec 2022 02:37:59 GMT  
		Size: 4.9 MB (4931334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be4d1bc2e6499ce625dcdda5acd93b321c54ee260c695d77c968071e871021d`  
		Last Modified: Wed, 21 Dec 2022 02:37:59 GMT  
		Size: 10.2 MB (10217819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a65a60d98682702b4ca7c54d1b60f35f73d52dc11af8d26f125673a5962046e`  
		Last Modified: Wed, 21 Dec 2022 02:38:23 GMT  
		Size: 50.3 MB (50342949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863fbc7dd41ea590ace5d8dcbe391137f9b8170091ef531834d3f20d63f10cf1`  
		Last Modified: Wed, 21 Dec 2022 02:39:06 GMT  
		Size: 167.4 MB (167354881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:728346feafecf3fd463a033b9449233b30b6ec897c9889ae38688ad8d2d72757`  
		Last Modified: Wed, 21 Dec 2022 05:48:19 GMT  
		Size: 179.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66b90f143807543a9654532968c0458316a534f1ea374ba9a21fcce5109ac7e2`  
		Last Modified: Wed, 21 Dec 2022 05:50:48 GMT  
		Size: 14.3 MB (14347816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:9361e57de9b5fada9e02eedf4f379435faa1bc115d31f7279b5c39118e761278
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.4 MB (329392272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d1ead34cd684544a6427872f0ed4905810a03021a4eb06d9ea03b46fed43c69`
-	Default Command: `["perl5.36.0","-de0"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:40 GMT
ADD file:5bbdc914ec8ed60ac85293e88ee1aafc3f0290762e320fc86dc9d79fa201834e in / 
# Wed, 21 Dec 2022 01:39:41 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:05:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:06:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 21 Dec 2022 02:06:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:07:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 04:07:17 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 21 Dec 2022 04:07:17 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Wed, 21 Dec 2022 04:07:17 GMT
WORKDIR /usr/src/perl
# Wed, 21 Dec 2022 04:30:21 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.0.tar.xz -o perl-5.36.0.tar.xz     && echo '0f386dccbee8e26286404b2cca144e1005be65477979beb9b1ba272d4819bcf0 *perl-5.36.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.0.tar.xz -C /usr/src/perl     && rm perl-5.36.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Wed, 21 Dec 2022 04:30:21 GMT
WORKDIR /
# Wed, 21 Dec 2022 04:30:21 GMT
CMD ["perl5.36.0" "-de0"]
```

-	Layers:
	-	`sha256:c3e6129b48b69d14c5e7a5605e2b94003fb71aac82eac46b8689f5b8007af2c5`  
		Last Modified: Wed, 21 Dec 2022 01:42:49 GMT  
		Size: 53.7 MB (53681797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef0470f9572d03767b054118fe19e60a9c7e2510168b3a0868d9ac2953d2def5`  
		Last Modified: Wed, 21 Dec 2022 02:12:40 GMT  
		Size: 5.1 MB (5149770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99dfcef0545e5bca269c65c0208385c886321a1e0212977299827be5346dfea5`  
		Last Modified: Wed, 21 Dec 2022 02:12:40 GMT  
		Size: 10.9 MB (10873505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940d63caabf45c64562daab3c243c8724dd47bf45054d902ef3cb6206fc9c3f6`  
		Last Modified: Wed, 21 Dec 2022 02:12:57 GMT  
		Size: 54.7 MB (54682464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f50438bf9d47df748db3fa6d353315cfa3b13c62806c353d37018d50cfa03d9`  
		Last Modified: Wed, 21 Dec 2022 02:13:26 GMT  
		Size: 189.8 MB (189803168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b0279f69163c5398147cb35f4392ca0f75e232708305d95d5269b97d7704fa5`  
		Last Modified: Wed, 21 Dec 2022 05:59:26 GMT  
		Size: 205.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493fc7665c02c4ba02a67f0c1d838a5af06a2f8f4edab1a185c20bcd13e76075`  
		Last Modified: Wed, 21 Dec 2022 06:00:51 GMT  
		Size: 15.2 MB (15201363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded` - linux; 386

```console
$ docker pull perl@sha256:420bd2affe3a63acde4525833f71c9fcb237a7fa5f8bce857653fa2b82abd8e1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **342.9 MB (342852393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1ba5f102fd2f4afb705049d01b5e2685c84193170d8ac3cf452f888092eb0b3`
-	Default Command: `["perl5.36.0","-de0"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:08 GMT
ADD file:10d2f443f55d8ba9512899b3dff08f6e9a6c7ca096f407e3477e9798e1063785 in / 
# Wed, 21 Dec 2022 01:39:09 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 09:52:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 09:52:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 21 Dec 2022 09:53:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 09:53:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 19:55:31 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 21 Dec 2022 19:55:32 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Wed, 21 Dec 2022 19:55:33 GMT
WORKDIR /usr/src/perl
# Wed, 21 Dec 2022 20:14:22 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.0.tar.xz -o perl-5.36.0.tar.xz     && echo '0f386dccbee8e26286404b2cca144e1005be65477979beb9b1ba272d4819bcf0 *perl-5.36.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.0.tar.xz -C /usr/src/perl     && rm perl-5.36.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Wed, 21 Dec 2022 20:14:23 GMT
WORKDIR /
# Wed, 21 Dec 2022 20:14:24 GMT
CMD ["perl5.36.0" "-de0"]
```

-	Layers:
	-	`sha256:bde501e1d960005aee2bdf2fc8c89b26bf694dace8740c72deda4d7705995ab7`  
		Last Modified: Wed, 21 Dec 2022 01:44:18 GMT  
		Size: 56.0 MB (56005267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc88409a7eb6934a31649306963a2d6378f44816008e5431d49956a05b6f53c`  
		Last Modified: Wed, 21 Dec 2022 10:00:21 GMT  
		Size: 5.3 MB (5291055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e6a42ef8edb5198054d515eb6d1b316d81e2a812d8897f9fc72e8be5e09955`  
		Last Modified: Wed, 21 Dec 2022 10:00:21 GMT  
		Size: 11.0 MB (11032532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884b11e49401a005d287945312c7ba4cc5a1e8ec97a947c4195b56c84cc43eb5`  
		Last Modified: Wed, 21 Dec 2022 10:00:41 GMT  
		Size: 55.9 MB (55923189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bd6c0b392a933fa0bcb7cba72e65cc5c58631a3eba3aa9be35706e523ebb20`  
		Last Modified: Wed, 21 Dec 2022 10:01:17 GMT  
		Size: 199.8 MB (199787331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62e0fbf4b3962abbc091935f27f413897f61fb6f569b40b3beea065804a18c99`  
		Last Modified: Wed, 21 Dec 2022 21:14:58 GMT  
		Size: 180.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd035a7285139adbc6d9634833b89f133f3689d4450a679aa5b6d1ec740b6fd`  
		Last Modified: Wed, 21 Dec 2022 21:15:59 GMT  
		Size: 14.8 MB (14812839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded` - linux; mips64le

```console
$ docker pull perl@sha256:abd7a4f2d19041ab9f0cb1e08ebe5a0c8cbfb10cda49d8390df00bd51a41aadc
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **315.6 MB (315639638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26edfe4d951ac86708892984dd62e07846e5487b955fc06526c5667a2406d7f5`
-	Default Command: `["perl5.36.0","-de0"]`

```dockerfile
# Tue, 06 Dec 2022 01:54:55 GMT
ADD file:09d48994a41c54566f7123db033773e6246c0703a518af76843198196cd39645 in / 
# Tue, 06 Dec 2022 01:55:00 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 17:16:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 17:16:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 17:18:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 17:23:43 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 07 Dec 2022 03:40:50 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 07 Dec 2022 03:40:55 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Wed, 07 Dec 2022 03:41:01 GMT
WORKDIR /usr/src/perl
# Wed, 07 Dec 2022 04:27:38 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.0.tar.xz -o perl-5.36.0.tar.xz     && echo '0f386dccbee8e26286404b2cca144e1005be65477979beb9b1ba272d4819bcf0 *perl-5.36.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.0.tar.xz -C /usr/src/perl     && rm perl-5.36.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Wed, 07 Dec 2022 04:27:44 GMT
WORKDIR /
# Wed, 07 Dec 2022 04:27:50 GMT
CMD ["perl5.36.0" "-de0"]
```

-	Layers:
	-	`sha256:acb57a81743c28ead1a32571c107ac15cd970593fea4f2954b57f22e6bbad1d0`  
		Last Modified: Tue, 06 Dec 2022 02:02:59 GMT  
		Size: 53.3 MB (53260631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3775e3b48d5b75d557cd315824f4c6f06a699ddbda90085efdafca39708308cb`  
		Last Modified: Tue, 06 Dec 2022 17:36:12 GMT  
		Size: 4.9 MB (4919540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226edb4ba5e4851b2344de27abb2912005f2259d9a16819ef66c22ca5eff8c4d`  
		Last Modified: Tue, 06 Dec 2022 17:36:14 GMT  
		Size: 10.7 MB (10661692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:983b5b89a87657fcfac5cae3540e343a9cf77d6e10cf3eb736a4e46608390212`  
		Last Modified: Tue, 06 Dec 2022 17:37:02 GMT  
		Size: 53.3 MB (53306766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:005791f776c3cbe2a6500e8c8e134cfb1061735ab9cc82bbda48536dc55c0840`  
		Last Modified: Tue, 06 Dec 2022 17:39:05 GMT  
		Size: 179.0 MB (178979694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe96d7b0f8dba2070c5569b7008d644b52d82e6b8bfe5d9ee45852271c28f477`  
		Last Modified: Wed, 07 Dec 2022 05:59:36 GMT  
		Size: 180.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52c33a08787a01cb2776ed62afb27260a5cdc35a43359106e2a3696b4a39633`  
		Last Modified: Wed, 07 Dec 2022 06:00:35 GMT  
		Size: 14.5 MB (14511135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded` - linux; ppc64le

```console
$ docker pull perl@sha256:6f448f08e72b8ccdee8b3382d6fd3e75819d3fc4c25ced7f7f57b19e8de13185
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.4 MB (346352905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:351cfea933926b98ec013d9b6e4c05795776280a28a2c4d34c284d3ed3fb37fa`
-	Default Command: `["perl5.36.0","-de0"]`

```dockerfile
# Wed, 21 Dec 2022 01:17:21 GMT
ADD file:c95bdb0df70fa9ce48b31a7ceb8a7be0c5b925efcf01c43595868b86994dc192 in / 
# Wed, 21 Dec 2022 01:17:25 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 04:54:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 04:54:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 21 Dec 2022 04:55:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 04:57:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 05:26:03 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 21 Dec 2022 05:26:03 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Wed, 21 Dec 2022 05:26:03 GMT
WORKDIR /usr/src/perl
# Wed, 21 Dec 2022 05:51:42 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.0.tar.xz -o perl-5.36.0.tar.xz     && echo '0f386dccbee8e26286404b2cca144e1005be65477979beb9b1ba272d4819bcf0 *perl-5.36.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.0.tar.xz -C /usr/src/perl     && rm perl-5.36.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Wed, 21 Dec 2022 05:51:43 GMT
WORKDIR /
# Wed, 21 Dec 2022 05:51:44 GMT
CMD ["perl5.36.0" "-de0"]
```

-	Layers:
	-	`sha256:542880f4d15404af17d342ecbb76bb92724fc7cb8a91a5e18f26bd8f8811a38a`  
		Last Modified: Wed, 21 Dec 2022 01:22:46 GMT  
		Size: 58.9 MB (58897040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b0d1697a3bff7991f1c96b22ffd254326c700694ddcf45ba42cd27f8a9cb94`  
		Last Modified: Wed, 21 Dec 2022 05:06:06 GMT  
		Size: 5.4 MB (5413147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5363f0c14d79c77678586642d6ff9ef822416864a8358da267bef743bb215907`  
		Last Modified: Wed, 21 Dec 2022 05:06:07 GMT  
		Size: 11.6 MB (11629527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec399ef8d37e347a1f93e54dd49428d1cec8a8926b5b48c5823c1e9813d561a`  
		Last Modified: Wed, 21 Dec 2022 05:06:38 GMT  
		Size: 58.9 MB (58866093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebe8cb6c21b75ae2fbcc74642a4953de0fae1083c05384c2ee8e1152859f1384`  
		Last Modified: Wed, 21 Dec 2022 05:07:40 GMT  
		Size: 196.2 MB (196229879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a32a6572de312c305c89d009b04110e03dfa48881a7248ed7c67672335b88b7`  
		Last Modified: Wed, 21 Dec 2022 07:10:32 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4751e526954dbf5b0f1ab22508aa4d05b25cc26f4e3c9f912fe74b775d0b05c`  
		Last Modified: Wed, 21 Dec 2022 07:11:55 GMT  
		Size: 15.3 MB (15317017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded` - linux; s390x

```console
$ docker pull perl@sha256:630889513d27b0b80e4918efe231ce8962e8ed41dd9ef28cbed3c4cf53d3f601
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.7 MB (311723326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:778b5594947b1803f9fa7c9270435bfde47bbb3ff3fe6068362d441217a7c4d1`
-	Default Command: `["perl5.36.0","-de0"]`

```dockerfile
# Wed, 21 Dec 2022 01:42:51 GMT
ADD file:22c4f2d41083ce4433bec4a71e7e6ddc5bec8e44e9cf2c9f93d0874b5b4de7c3 in / 
# Wed, 21 Dec 2022 01:42:54 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 05:28:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 05:28:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 21 Dec 2022 05:29:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 05:31:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 06:00:04 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 21 Dec 2022 06:00:04 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Wed, 21 Dec 2022 06:00:05 GMT
WORKDIR /usr/src/perl
# Wed, 21 Dec 2022 06:24:45 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.0.tar.xz -o perl-5.36.0.tar.xz     && echo '0f386dccbee8e26286404b2cca144e1005be65477979beb9b1ba272d4819bcf0 *perl-5.36.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.0.tar.xz -C /usr/src/perl     && rm perl-5.36.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Wed, 21 Dec 2022 06:24:50 GMT
WORKDIR /
# Wed, 21 Dec 2022 06:24:51 GMT
CMD ["perl5.36.0" "-de0"]
```

-	Layers:
	-	`sha256:7f45294776f4c97d23f8dbfca98d4b57701b478eedfcb154a7e7dc6d6954ba44`  
		Last Modified: Wed, 21 Dec 2022 01:48:50 GMT  
		Size: 53.3 MB (53258472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33059268c0ceb39818d5991d1a0e968b0ac63a17cd965fc4a7094dae7b286bff`  
		Last Modified: Wed, 21 Dec 2022 05:41:10 GMT  
		Size: 5.1 MB (5147132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adad3194d340e6c5e79c1917e144d792bb5073c3e126f969f1695bc449822315`  
		Last Modified: Wed, 21 Dec 2022 05:41:11 GMT  
		Size: 10.8 MB (10766081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a479ec115bd827027c66c90c65bac92d04e338c0cc00025b35dbfc756f4fbbd9`  
		Last Modified: Wed, 21 Dec 2022 05:41:30 GMT  
		Size: 54.1 MB (54054846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be60c4ac9a8d51fbb8d4c3843e2016173124b685f731ad093fb907b8b208ea7`  
		Last Modified: Wed, 21 Dec 2022 05:41:58 GMT  
		Size: 172.9 MB (172868922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e5749158b3c28465615cf15dcc1a9465e97d77720758571d6d465daa6aef8b8`  
		Last Modified: Wed, 21 Dec 2022 07:45:54 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399f28b3c6597b0be1853e33b2d0817f4a9230969f86da35a534096411983815`  
		Last Modified: Wed, 21 Dec 2022 07:46:45 GMT  
		Size: 15.6 MB (15627670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
