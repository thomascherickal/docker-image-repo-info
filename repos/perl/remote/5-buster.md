## `perl:5-buster`

```console
$ docker pull perl@sha256:7873a26b03df352497de4e787a114f801e99c497880c6da3edd9ea0d73397dcf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `perl:5-buster` - linux; amd64

```console
$ docker pull perl@sha256:4682d25d665189bf3e2cc63dc937f45c14f5293da56daeee73a3b296b9be7880
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.4 MB (326420357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ec34f23fbee7c653de5c9b9cc72362bfd9cbaa6d239c7bbeabf8f5a40f775b5`
-	Default Command: `["perl5.32.0","-de0"]`

```dockerfile
# Fri, 11 Dec 2020 02:05:52 GMT
ADD file:6014cd9d7466825f80d4a3345847efd6fd7ef600b8135811cab4f0e304f66cd7 in / 
# Fri, 11 Dec 2020 02:05:52 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 20:37:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 20:37:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 11 Dec 2020 20:37:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 20:38:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 12 Dec 2020 14:06:01 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 12 Dec 2020 14:06:01 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Sat, 12 Dec 2020 14:06:01 GMT
WORKDIR /usr/src/perl
# Sat, 12 Dec 2020 14:19:11 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.0.tar.xz -o perl-5.32.0.tar.xz     && echo '6f436b447cf56d22464f980fac1916e707a040e96d52172984c5d184c09b859b *perl-5.32.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.0.tar.xz -C /usr/src/perl     && rm perl-5.32.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Sat, 12 Dec 2020 14:19:11 GMT
WORKDIR /
# Sat, 12 Dec 2020 14:19:12 GMT
CMD ["perl5.32.0" "-de0"]
```

-	Layers:
	-	`sha256:6c33745f49b41daad28b7b192c447938452ea4de9fe8c7cc3edf1433b1366946`  
		Last Modified: Fri, 11 Dec 2020 02:12:07 GMT  
		Size: 50.4 MB (50397728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87cd3c61e278307eaa282fdbb51a5e2415cda64999c70a381ed6c5c724d370a`  
		Last Modified: Fri, 11 Dec 2020 20:44:17 GMT  
		Size: 7.8 MB (7811925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a3c799ec372b93b6dbd4b270effd9f36444dc164e8827ea9ab7aa0d1ef87da`  
		Last Modified: Fri, 11 Dec 2020 20:44:17 GMT  
		Size: 10.0 MB (9996419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61c38f966ac77bd84d7866db24e1f7611b158e51e10e2e73ce009c3ad73f472`  
		Last Modified: Fri, 11 Dec 2020 20:44:36 GMT  
		Size: 51.8 MB (51830085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2dd6d195b6814bc0fc1eb872f13330e352cd881fc3dda45997e398aadfde685`  
		Last Modified: Fri, 11 Dec 2020 20:45:20 GMT  
		Size: 192.3 MB (192314183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a706435cd9cdb91758a629039d8ffbfcdd0af4f797d559adb9b2149bae40ac4`  
		Last Modified: Sat, 12 Dec 2020 16:37:15 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e001147bb4ccdc74d99df6aee3dc61e12a308c40ab314d344b4f3ce03772f99`  
		Last Modified: Sat, 12 Dec 2020 16:37:18 GMT  
		Size: 14.1 MB (14069839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-buster` - linux; arm variant v7

```console
$ docker pull perl@sha256:e14fc7f81ed81ba9f353f74a460e9eb28c3159c601b6d84cb7f32bf9871b7ce0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.4 MB (291415372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4c4d5f711c4fc272f2d2eb429f29df7ee2f12bafad679fdae179deb92fcb2bf`
-	Default Command: `["perl5.32.0","-de0"]`

```dockerfile
# Fri, 11 Dec 2020 02:23:08 GMT
ADD file:af46f686172bae3034ad0b34cc26081a2f8db0f5d4704ef63abb7eeaf06c75e0 in / 
# Fri, 11 Dec 2020 02:23:11 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:24:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:24:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 11 Dec 2020 16:25:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:28:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:49:53 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Fri, 11 Dec 2020 16:49:54 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Fri, 11 Dec 2020 16:49:55 GMT
WORKDIR /usr/src/perl
# Fri, 11 Dec 2020 16:59:30 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.0.tar.xz -o perl-5.32.0.tar.xz     && echo '6f436b447cf56d22464f980fac1916e707a040e96d52172984c5d184c09b859b *perl-5.32.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.0.tar.xz -C /usr/src/perl     && rm perl-5.32.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Fri, 11 Dec 2020 16:59:32 GMT
WORKDIR /
# Fri, 11 Dec 2020 16:59:33 GMT
CMD ["perl5.32.0" "-de0"]
```

-	Layers:
	-	`sha256:709549ab8c597dac59777a5a3666600f3dd986b5f05389aa7b15bd5f9281f809`  
		Last Modified: Fri, 11 Dec 2020 02:32:43 GMT  
		Size: 45.9 MB (45867902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ebb34ef82f207f1fe2804f394d61205a909e4ec6256fc1aa3a30b484c3176f`  
		Last Modified: Fri, 11 Dec 2020 16:43:39 GMT  
		Size: 7.1 MB (7099238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebc4c14c5eea8f2b3009ee1de8df43fcf61c0a0d73af4efa97923119eae19bf`  
		Last Modified: Fri, 11 Dec 2020 16:43:38 GMT  
		Size: 9.3 MB (9343469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc2d9bc5b9d534ac062b6fe74080e2674bdd0caef2d6c12cd1018d79ad0b02a`  
		Last Modified: Fri, 11 Dec 2020 16:44:04 GMT  
		Size: 47.4 MB (47356031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:464e679b47b4193d41aa104658d18c56764a55280587949d2c6906ad683c3f91`  
		Last Modified: Fri, 11 Dec 2020 16:44:59 GMT  
		Size: 168.5 MB (168533599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5a1bd65c07606dc2487d63c1fc0c3acca50eb743f0c68a1274b802b14d1277`  
		Last Modified: Fri, 11 Dec 2020 20:35:09 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb53f7822217e59904727be2fc0d1f0df6a41b93dc1b20636d3cb5c97ac24c93`  
		Last Modified: Fri, 11 Dec 2020 20:35:15 GMT  
		Size: 13.2 MB (13214930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-buster` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:249aa55cd73a82f3b077ce9849ccba4d8ff245b34be36bced6d100186be3ce8f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.9 MB (316898498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9792f132f19d306c43ef7301e85684ead0d1b74b98a41bdb40f7b6a7dd80b1a`
-	Default Command: `["perl5.32.0","-de0"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:23 GMT
ADD file:b08f373022952dba7d08b7fc02909d9e369c9727e0e4f62d6110e41e70e668cc in / 
# Fri, 11 Dec 2020 02:45:25 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 18:52:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 18:53:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 11 Dec 2020 18:53:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 18:55:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 19:17:11 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Fri, 11 Dec 2020 19:17:11 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Fri, 11 Dec 2020 19:17:12 GMT
WORKDIR /usr/src/perl
# Fri, 11 Dec 2020 19:26:17 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.0.tar.xz -o perl-5.32.0.tar.xz     && echo '6f436b447cf56d22464f980fac1916e707a040e96d52172984c5d184c09b859b *perl-5.32.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.0.tar.xz -C /usr/src/perl     && rm perl-5.32.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Fri, 11 Dec 2020 19:26:19 GMT
WORKDIR /
# Fri, 11 Dec 2020 19:26:19 GMT
CMD ["perl5.32.0" "-de0"]
```

-	Layers:
	-	`sha256:99e5136f81cd2a8cc226c42435d6f4f30584d168cc51f4d4afd2d5611e4d2215`  
		Last Modified: Fri, 11 Dec 2020 02:52:45 GMT  
		Size: 49.2 MB (49180317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76c9f56ed15888e5a0a9a8738d53044b1d62ff9f3c8c2857e5cebf782039305`  
		Last Modified: Fri, 11 Dec 2020 19:07:21 GMT  
		Size: 7.7 MB (7682310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33292316eac7d9491a0980a8cc9ba5f3e9cde7e2af0014f8dc10cdae5706b9d8`  
		Last Modified: Fri, 11 Dec 2020 19:07:22 GMT  
		Size: 10.0 MB (9984305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3287f43f5d44b20fe250f2683c57f0330bb0451261ad1d0c3eab9b116b0da52b`  
		Last Modified: Fri, 11 Dec 2020 19:07:44 GMT  
		Size: 52.2 MB (52164628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c6f771d62b3aeedaea9b8db36abed7da0bc14a0ed5e98935de87a1feaeb843`  
		Last Modified: Fri, 11 Dec 2020 19:08:42 GMT  
		Size: 183.9 MB (183870732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c1f330f7b3c416f365d1ed05dfa955800db43d62ac47e4a08e924c7abe0fe0`  
		Last Modified: Fri, 11 Dec 2020 23:02:41 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15019ac0c83e07bf0e3ac2938acb4e74bd87f99ab5499b28a90ca1c381fd4593`  
		Last Modified: Fri, 11 Dec 2020 23:02:46 GMT  
		Size: 14.0 MB (14016006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-buster` - linux; 386

```console
$ docker pull perl@sha256:5e1930bcc7e021267cf028fcc9e3cb9bbcfca51732c51e53937a3aa812c1c08c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.3 MB (335339792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81621864e031bd136d11236d8616c77a3e9a0886a21af2f865753fdd75d71d15`
-	Default Command: `["perl5.32.0","-de0"]`

```dockerfile
# Fri, 11 Dec 2020 02:02:51 GMT
ADD file:5131dbfe4d05a72c50b47e4ee936290486446a3a4dfe832240dd270b0f563542 in / 
# Fri, 11 Dec 2020 02:02:51 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 21:52:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 21:52:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 11 Dec 2020 21:53:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 21:54:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 22:32:49 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Fri, 11 Dec 2020 22:32:49 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Fri, 11 Dec 2020 22:32:49 GMT
WORKDIR /usr/src/perl
# Fri, 11 Dec 2020 22:43:46 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.0.tar.xz -o perl-5.32.0.tar.xz     && echo '6f436b447cf56d22464f980fac1916e707a040e96d52172984c5d184c09b859b *perl-5.32.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.0.tar.xz -C /usr/src/perl     && rm perl-5.32.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Fri, 11 Dec 2020 22:43:46 GMT
WORKDIR /
# Fri, 11 Dec 2020 22:43:47 GMT
CMD ["perl5.32.0" "-de0"]
```

-	Layers:
	-	`sha256:d18c9b676b719f51a76e9b6c9cb0781fbe5c36a18cfdcdac473acae10efbb381`  
		Last Modified: Fri, 11 Dec 2020 02:09:16 GMT  
		Size: 51.2 MB (51161209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e65f6b8ae81f7c117e14ce493f06a12caf05381e28e3e49377f9a8df8faec23`  
		Last Modified: Fri, 11 Dec 2020 22:01:23 GMT  
		Size: 8.0 MB (7981643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550bb3e6c2957b203bf8dd84e95fbae17705a07e090d1494aa9320dec6fae226`  
		Last Modified: Fri, 11 Dec 2020 22:01:23 GMT  
		Size: 10.3 MB (10338820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d57d09060e8546e1c094e2f365eae9cd2fbc6636eb4fa9981b7066d3a3f1400`  
		Last Modified: Fri, 11 Dec 2020 22:01:48 GMT  
		Size: 53.4 MB (53432037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6ddf79278d52d7a566157e88a46bea5b94913cc3d89103617609e99376ae5c`  
		Last Modified: Fri, 11 Dec 2020 22:02:48 GMT  
		Size: 198.9 MB (198860674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4825768dca52ff89aebad399c47ed2a8a04691036ab4ba1cbd767c97a540f0c5`  
		Last Modified: Sat, 12 Dec 2020 03:01:01 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05087b738eb662782a968665778685e393214c4206469b03c0779151b7310064`  
		Last Modified: Sat, 12 Dec 2020 03:01:06 GMT  
		Size: 13.6 MB (13565232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-buster` - linux; ppc64le

```console
$ docker pull perl@sha256:cdab85fa835425dab690fbccdd80f3b1e545f1b968006adcb63925ac79f074e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **347.8 MB (347837271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2594f16862f4b73eb192fc3d657e242717543414bf592f97049df843bf94efd`
-	Default Command: `["perl5.32.0","-de0"]`

```dockerfile
# Fri, 11 Dec 2020 03:33:14 GMT
ADD file:3f6d74a3193dcc81fb8d9c0a830337812d5ed7618d5f16c8eb193d30f827c49d in / 
# Fri, 11 Dec 2020 03:33:24 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 19:24:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 19:25:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 11 Dec 2020 19:26:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 19:36:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 12 Dec 2020 14:01:37 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 12 Dec 2020 14:01:39 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Sat, 12 Dec 2020 14:01:40 GMT
WORKDIR /usr/src/perl
# Sat, 12 Dec 2020 14:08:07 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.0.tar.xz -o perl-5.32.0.tar.xz     && echo '6f436b447cf56d22464f980fac1916e707a040e96d52172984c5d184c09b859b *perl-5.32.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.0.tar.xz -C /usr/src/perl     && rm perl-5.32.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Sat, 12 Dec 2020 14:08:09 GMT
WORKDIR /
# Sat, 12 Dec 2020 14:08:12 GMT
CMD ["perl5.32.0" "-de0"]
```

-	Layers:
	-	`sha256:fbe5c9ac66677a4494c2d36707222498adce02d2dcb8e08d2f8a59a0f10b2582`  
		Last Modified: Fri, 11 Dec 2020 03:41:06 GMT  
		Size: 54.1 MB (54142548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d010cc30cdcf987911ffc599e65919322a99ed67ffbdc58c8dd33b8f7d97e1eb`  
		Last Modified: Fri, 11 Dec 2020 19:52:34 GMT  
		Size: 8.3 MB (8255764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a04c26bc5dbbef0dbb7d925ec93c17327190ae1f877032ddbb9f577df56806c3`  
		Last Modified: Fri, 11 Dec 2020 19:52:33 GMT  
		Size: 10.7 MB (10727480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7cddc612121e26c030f8b0919573ac5f6bf1995d0eaac2e49fd90f93989dca`  
		Last Modified: Fri, 11 Dec 2020 19:53:00 GMT  
		Size: 57.5 MB (57455242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18164c0bbe27de0333c25666afc0a04165412f9346c60daf036cf6f6740bd0e1`  
		Last Modified: Fri, 11 Dec 2020 19:53:49 GMT  
		Size: 203.2 MB (203153740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590c3a8fc7fcc9eed2e31a08f267febbf78ed7664038492d31283646b7068717`  
		Last Modified: Sat, 12 Dec 2020 14:43:18 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28dc711ceff88f002ada905c8a55353b215ad7df90d17fde35153d5cd124bd67`  
		Last Modified: Sat, 12 Dec 2020 14:43:22 GMT  
		Size: 14.1 MB (14102294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-buster` - linux; s390x

```console
$ docker pull perl@sha256:2830db4c18872f3a7c8699e5790e5bd80e0351c1b0f9f47b4fb82ad175c6a7f5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.9 MB (308856469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3b0acb85d4780f95f0b7475f8207f0ae96dc9bf8138b28f5bf9c7a2e6c3b00b`
-	Default Command: `["perl5.32.0","-de0"]`

```dockerfile
# Fri, 11 Dec 2020 02:11:47 GMT
ADD file:b48379f9d2c111607924e8c59c2769c735341a59df0d6819d8a4b3e44f5457b0 in / 
# Fri, 11 Dec 2020 02:11:54 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:02:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:03:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 11 Dec 2020 16:03:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:06:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 12 Dec 2020 01:27:59 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 12 Dec 2020 01:27:59 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Sat, 12 Dec 2020 01:28:00 GMT
WORKDIR /usr/src/perl
# Sat, 12 Dec 2020 01:33:54 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.0.tar.xz -o perl-5.32.0.tar.xz     && echo '6f436b447cf56d22464f980fac1916e707a040e96d52172984c5d184c09b859b *perl-5.32.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.0.tar.xz -C /usr/src/perl     && rm perl-5.32.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Sat, 12 Dec 2020 01:33:58 GMT
WORKDIR /
# Sat, 12 Dec 2020 01:33:59 GMT
CMD ["perl5.32.0" "-de0"]
```

-	Layers:
	-	`sha256:b8cd59e115fe85cdffdb9750beb150c189e768249dc100d22cab4733fb0c7247`  
		Last Modified: Fri, 11 Dec 2020 02:16:44 GMT  
		Size: 49.0 MB (48968242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0eb33d878287686bed77cfef9cecb3fd540caf075a646ed34afdb64288ae74`  
		Last Modified: Fri, 11 Dec 2020 16:15:45 GMT  
		Size: 7.4 MB (7386652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7571827f1162945abd5d70aa40ae2489e866f25a600c027f482c4dbd5bfc88`  
		Last Modified: Fri, 11 Dec 2020 16:15:45 GMT  
		Size: 9.9 MB (9883064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b9e36ebe77bd8ffdf1d40b3ce51f765116b1fdc5aa75b3bd774c9388233fc72`  
		Last Modified: Fri, 11 Dec 2020 16:16:04 GMT  
		Size: 51.4 MB (51379787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01320660a363425b4f9f32a4b413821e56ab6777e437330fb62f29ef4ddca113`  
		Last Modified: Fri, 11 Dec 2020 16:16:38 GMT  
		Size: 176.8 MB (176832403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6628367b425d951164232abf2b8b9654a4ebc3805b3e2f2f205728d7561d7f15`  
		Last Modified: Sat, 12 Dec 2020 02:07:22 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22088909ad5e33612f8ef5b92b5d476d7031dd7769900f8b19c8ce7e3edb3276`  
		Last Modified: Sat, 12 Dec 2020 02:07:24 GMT  
		Size: 14.4 MB (14406118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
