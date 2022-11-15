## `perl:bullseye`

```console
$ docker pull perl@sha256:196d1c7f1cb66c13927a5133dead109cf8e67da3d6eec484b6849391660560bc
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

### `perl:bullseye` - linux; amd64

```console
$ docker pull perl@sha256:517f8c39ab0a2e8b3c7be37373c253a6d42c28d40be3306d96acf0d8484031f7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.8 MB (337765207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75a16f98ad6cb52946f9c2475b2721029e43642db713920902193e420c218d97`
-	Default Command: `["perl5.36.0","-de0"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:42 GMT
ADD file:26702ba2c3e94cb21cdb3c550cf01cf848823d160f3417b559116d4c718e5df0 in / 
# Tue, 25 Oct 2022 01:43:42 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:23:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:23:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 09:23:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:24:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 10:53:33 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 25 Oct 2022 10:53:33 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 25 Oct 2022 10:53:33 GMT
WORKDIR /usr/src/perl
# Tue, 25 Oct 2022 10:58:59 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.0.tar.xz -o perl-5.36.0.tar.xz     && echo '0f386dccbee8e26286404b2cca144e1005be65477979beb9b1ba272d4819bcf0 *perl-5.36.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.0.tar.xz -C /usr/src/perl     && rm perl-5.36.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Tue, 25 Oct 2022 10:58:59 GMT
WORKDIR /
# Tue, 25 Oct 2022 10:58:59 GMT
CMD ["perl5.36.0" "-de0"]
```

-	Layers:
	-	`sha256:17c9e6141fdb3387e5a1c07d4f9b6a05ac1498e96029fa3ea55470d4504f7770`  
		Last Modified: Tue, 25 Oct 2022 01:47:28 GMT  
		Size: 55.0 MB (55046332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4a4c6caea8801bb0b7377e10220a914da403bc93fa79663cbf2dcf1800b6f1`  
		Last Modified: Tue, 25 Oct 2022 09:47:36 GMT  
		Size: 5.2 MB (5164775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4edced8587e6c18412817019074f5e04a8ede4e2fc89d06af13df3f80d78a70d`  
		Last Modified: Tue, 25 Oct 2022 09:47:36 GMT  
		Size: 10.9 MB (10877322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7969cffbf46e6a91291fd76b19ecbe93c03ea4ded0d14042aecb4c0c4211a43`  
		Last Modified: Tue, 25 Oct 2022 09:47:56 GMT  
		Size: 54.6 MB (54586464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74fbfde6af91271fb88f0a1716224dcce5c0ebead3609943792a9cb6ba4d6d3d`  
		Last Modified: Tue, 25 Oct 2022 09:48:34 GMT  
		Size: 196.9 MB (196869249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a255ac7c71762c1731ee1858c0ed6a266025ded826209faa952e0651f93603a`  
		Last Modified: Tue, 25 Oct 2022 13:15:49 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb9068c7d44d6f5394bd36a52112c33b9ec14846e2bde01515a6bac3141d5c9`  
		Last Modified: Tue, 25 Oct 2022 13:15:53 GMT  
		Size: 15.2 MB (15220866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:bullseye` - linux; arm variant v5

```console
$ docker pull perl@sha256:83677635821e4d47887a4c24dee588ad9c8602a25607a59b5f5568d6ee2c2be6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.1 MB (310075384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e90743903f4fd8944efb4ecc8f7227ea18d522dbc97e833a7a214d676a83705`
-	Default Command: `["perl5.36.0","-de0"]`

```dockerfile
# Tue, 15 Nov 2022 01:49:01 GMT
ADD file:1301cc1a3eec72236eb8cfb02c81a3e956e32a32025a89995435b641e1d9330d in / 
# Tue, 15 Nov 2022 01:49:02 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:42:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 05:42:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 05:42:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 05:43:43 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 05:59:48 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 15 Nov 2022 05:59:48 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 15 Nov 2022 05:59:48 GMT
WORKDIR /usr/src/perl
# Tue, 15 Nov 2022 06:05:36 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.0.tar.xz -o perl-5.36.0.tar.xz     && echo '0f386dccbee8e26286404b2cca144e1005be65477979beb9b1ba272d4819bcf0 *perl-5.36.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.0.tar.xz -C /usr/src/perl     && rm perl-5.36.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Tue, 15 Nov 2022 06:05:37 GMT
WORKDIR /
# Tue, 15 Nov 2022 06:05:37 GMT
CMD ["perl5.36.0" "-de0"]
```

-	Layers:
	-	`sha256:0655cdb20ead0094190060645bdf853e9427b58a64f0c7d92ae439b80ca81fdf`  
		Last Modified: Tue, 15 Nov 2022 01:53:55 GMT  
		Size: 52.5 MB (52542295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbb37740fe3185bdb0707209ff5ad54853d540c2a95c40ae3d998c9d4dcbe26`  
		Last Modified: Tue, 15 Nov 2022 05:48:21 GMT  
		Size: 5.1 MB (5072242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce25a37fc4ddb3f5200d17fea7e9ac780e294a18828ae0381ccb9c923c0d0f4f`  
		Last Modified: Tue, 15 Nov 2022 05:48:22 GMT  
		Size: 10.6 MB (10574332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28570b06bbb5d744b44244a4402740ce8f46ce1521152a97286cf795ccd833ff`  
		Last Modified: Tue, 15 Nov 2022 05:48:46 GMT  
		Size: 52.3 MB (52322588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e615eccf33dd8f0357cf8753f2820b809b923fd77333de02aede7b12d01186`  
		Last Modified: Tue, 15 Nov 2022 05:49:30 GMT  
		Size: 175.0 MB (175043532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9226f198562f80be9a566fefe6f6ee07027b6b73d7b8122e63594d03078550`  
		Last Modified: Tue, 15 Nov 2022 07:19:32 GMT  
		Size: 179.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970cc2974b60895d1147950ee99af621dc65fc4377667bc79d576ea7be2f323d`  
		Last Modified: Tue, 15 Nov 2022 07:19:36 GMT  
		Size: 14.5 MB (14520216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:bullseye` - linux; arm variant v7

```console
$ docker pull perl@sha256:41c97b51b1035ce324c1bca13b76d9fd7ea6069a56df9615cf48eb6b582fe5f1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.3 MB (297328698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b98854072b21737a0652249963c31e027f483934cbdd4b9487a38a38bc8f6dc`
-	Default Command: `["perl5.36.0","-de0"]`

```dockerfile
# Tue, 25 Oct 2022 03:14:06 GMT
ADD file:94d6b607b174c11c18753fac156b0ca5ecda941da3d456e136b8b14457810d37 in / 
# Tue, 25 Oct 2022 03:14:06 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 04:36:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 04:36:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Oct 2022 04:36:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 04:37:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 05:34:26 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 26 Oct 2022 05:34:26 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Wed, 26 Oct 2022 05:34:26 GMT
WORKDIR /usr/src/perl
# Wed, 26 Oct 2022 05:39:51 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.0.tar.xz -o perl-5.36.0.tar.xz     && echo '0f386dccbee8e26286404b2cca144e1005be65477979beb9b1ba272d4819bcf0 *perl-5.36.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.0.tar.xz -C /usr/src/perl     && rm perl-5.36.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Wed, 26 Oct 2022 05:39:52 GMT
WORKDIR /
# Wed, 26 Oct 2022 05:39:52 GMT
CMD ["perl5.36.0" "-de0"]
```

-	Layers:
	-	`sha256:a9bec1cbb822a75428a679c01f232b1af10cce0bdc1bf6507d26e8d79ad54300`  
		Last Modified: Tue, 25 Oct 2022 03:20:41 GMT  
		Size: 50.2 MB (50209987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9e47cd2446328779ff30de254793eaf539fec260638990e7d8dd3d29342fca`  
		Last Modified: Wed, 26 Oct 2022 05:10:38 GMT  
		Size: 4.9 MB (4932764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8deb44fa055f393de7346c484ab2ff3ef90e7efc4ebb018f932b377361e3b45`  
		Last Modified: Wed, 26 Oct 2022 05:10:38 GMT  
		Size: 10.2 MB (10218474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e22aca21bac1ccd293dcbdab0f501e5f245365480a29e4d11572ddc5092e2287`  
		Last Modified: Wed, 26 Oct 2022 05:11:04 GMT  
		Size: 50.3 MB (50345195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2b77379ff89ee066b0897ebbce4d7d188c6297407870d242677270cfe61ae2`  
		Last Modified: Wed, 26 Oct 2022 05:11:45 GMT  
		Size: 167.3 MB (167307103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4964124370795b0daa97fd6bfe9bb40885961136be0db4cee192db5598a2b4dd`  
		Last Modified: Wed, 26 Oct 2022 07:59:10 GMT  
		Size: 179.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f41776c56af91dd8c9fee2f5b271f14366553bfd35b180c90656b81cb87fef4f`  
		Last Modified: Wed, 26 Oct 2022 07:59:14 GMT  
		Size: 14.3 MB (14314996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:bullseye` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:5bd9f30617a0648eb21afb8a02c71be6fbc26233a45563edbb86d09fddde9a1d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.3 MB (329341112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e300a871b2d2cf19c5e73afa64ebd7658503202c3d432f6411fa568525c06ce`
-	Default Command: `["perl5.36.0","-de0"]`

```dockerfile
# Tue, 25 Oct 2022 05:45:55 GMT
ADD file:b16745ece8ef84c028d7e9ac4bf026ac64f885d4170bfcc9d435f237144a1b99 in / 
# Tue, 25 Oct 2022 05:45:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:58:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:58:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 07:59:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:00:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 14:06:25 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 25 Oct 2022 14:06:25 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 25 Oct 2022 14:06:25 GMT
WORKDIR /usr/src/perl
# Tue, 25 Oct 2022 14:10:36 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.0.tar.xz -o perl-5.36.0.tar.xz     && echo '0f386dccbee8e26286404b2cca144e1005be65477979beb9b1ba272d4819bcf0 *perl-5.36.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.0.tar.xz -C /usr/src/perl     && rm perl-5.36.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Tue, 25 Oct 2022 14:10:37 GMT
WORKDIR /
# Tue, 25 Oct 2022 14:10:37 GMT
CMD ["perl5.36.0" "-de0"]
```

-	Layers:
	-	`sha256:8e1d92e7d04d2a9a9880cb45dc3c32c2805912cd86abed96d0ada3ff28748205`  
		Last Modified: Tue, 25 Oct 2022 05:48:40 GMT  
		Size: 53.7 MB (53701966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66eadbf427bb41b3e329a95935c65b09c6d3b7a9c2fa8e08417e497df02ed996`  
		Last Modified: Tue, 25 Oct 2022 08:30:22 GMT  
		Size: 5.2 MB (5151506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9731f4e3bc3680179c10cece663cf0cfe0488918d6795406f4b76f07b787de`  
		Last Modified: Tue, 25 Oct 2022 08:30:22 GMT  
		Size: 10.9 MB (10874174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d337cb12fd7c6fe341850cd38e880f1806d49a65832c9804b06d00f9032382e0`  
		Last Modified: Tue, 25 Oct 2022 08:30:42 GMT  
		Size: 54.7 MB (54683990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a719597fe1ca78e1dc4c43fffc424754228514a791abcb0e0c06302ad022b8ca`  
		Last Modified: Tue, 25 Oct 2022 08:31:12 GMT  
		Size: 189.8 MB (189760702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f43b97d9d2198e6008d843c64ec91c3a39afdfbbfef8a1809c3125361da8cc2`  
		Last Modified: Tue, 25 Oct 2022 15:58:17 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc1163a8fc5541c5456afe6330133252aa187b4f9859a4b3157ba5a1d8f0d71b`  
		Last Modified: Tue, 25 Oct 2022 15:58:19 GMT  
		Size: 15.2 MB (15168574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:bullseye` - linux; 386

```console
$ docker pull perl@sha256:4e2b519a886befa60adcbe8a801d6557387e9b4c144dc80a601d3972edb8e4d4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **342.6 MB (342550404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3ce3c940ecff562e25a4dce261eb080a1040b4158bc0d5271c50c57baeb6b40`
-	Default Command: `["perl5.36.0","-de0"]`

```dockerfile
# Tue, 25 Oct 2022 02:22:19 GMT
ADD file:aa26f69b37c3e144d08e17bb9be7302ec89ae0579121c874a35f336d7077fd3b in / 
# Tue, 25 Oct 2022 02:22:19 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:15:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:15:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 05:15:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:16:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 11:46:26 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 25 Oct 2022 11:46:27 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 25 Oct 2022 11:46:27 GMT
WORKDIR /usr/src/perl
# Tue, 25 Oct 2022 11:52:41 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.0.tar.xz -o perl-5.36.0.tar.xz     && echo '0f386dccbee8e26286404b2cca144e1005be65477979beb9b1ba272d4819bcf0 *perl-5.36.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.0.tar.xz -C /usr/src/perl     && rm perl-5.36.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Tue, 25 Oct 2022 11:52:42 GMT
WORKDIR /
# Tue, 25 Oct 2022 11:52:43 GMT
CMD ["perl5.36.0" "-de0"]
```

-	Layers:
	-	`sha256:8caf426a2703f99fb0be4b03411ecaa580d102f7c47ef43b422b6d7c13c380e2`  
		Last Modified: Tue, 25 Oct 2022 02:27:54 GMT  
		Size: 56.0 MB (56023960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b92a2ff5c72653a0679aa7f5e2bc695011c0a71faa424229e560957d204dab`  
		Last Modified: Tue, 25 Oct 2022 05:27:37 GMT  
		Size: 5.1 MB (5086887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6856a3002e686ceb6d48d078731366f576ed3adcb73bd49dcb300057732904`  
		Last Modified: Tue, 25 Oct 2022 05:27:38 GMT  
		Size: 11.0 MB (11032526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e88080d3b5ba1edc8623a97d068bd040dfb89f2bc7bdfc0984d11fc35ff5885`  
		Last Modified: Tue, 25 Oct 2022 05:28:00 GMT  
		Size: 55.9 MB (55924404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b19879261038142328725a860507e23c40804ec5e04f1b7cf8f0dc88ded89d`  
		Last Modified: Tue, 25 Oct 2022 05:28:37 GMT  
		Size: 199.8 MB (199768743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cfcd38b2a7682689aad3b5093a6316f9f47dcec30de8673b07fdb544cee4eb`  
		Last Modified: Tue, 25 Oct 2022 14:26:32 GMT  
		Size: 180.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29543ef9743a5ca5c44ffaf52013e1a256e7be0c5fae655c336abf8d22e52299`  
		Last Modified: Tue, 25 Oct 2022 14:26:36 GMT  
		Size: 14.7 MB (14713704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:bullseye` - linux; mips64le

```console
$ docker pull perl@sha256:7a2f2fb99e08971a446a8e80b2d7ae9aa82137f7bf9558cbdf386fcd95f47c95
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **315.6 MB (315571535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48d47b81b8e669114995f4f18609c6949084759aef005006c08f703bc6cdfdb6`
-	Default Command: `["perl5.36.0","-de0"]`

```dockerfile
# Tue, 25 Oct 2022 04:38:51 GMT
ADD file:617ca04150550c7e3a178e3ac85bb359b17a390090ce6ce72a6f2ed1db10ab63 in / 
# Tue, 25 Oct 2022 04:38:57 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:30:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:31:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 09:33:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:38:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 14:03:27 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 25 Oct 2022 14:03:33 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 25 Oct 2022 14:03:38 GMT
WORKDIR /usr/src/perl
# Tue, 25 Oct 2022 14:25:48 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.0.tar.xz -o perl-5.36.0.tar.xz     && echo '0f386dccbee8e26286404b2cca144e1005be65477979beb9b1ba272d4819bcf0 *perl-5.36.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.0.tar.xz -C /usr/src/perl     && rm perl-5.36.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Tue, 25 Oct 2022 14:25:54 GMT
WORKDIR /
# Tue, 25 Oct 2022 14:26:01 GMT
CMD ["perl5.36.0" "-de0"]
```

-	Layers:
	-	`sha256:e3c84cb4c321de8db072180e3509c5bbcf8e562ff11c03241bdf082184fe74d6`  
		Last Modified: Tue, 25 Oct 2022 04:46:42 GMT  
		Size: 53.3 MB (53265848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3db3e162cf97fdacf5ea7f9f3912781648668e28872229f94c59a0ede7eb374`  
		Last Modified: Tue, 25 Oct 2022 09:51:57 GMT  
		Size: 4.9 MB (4919493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb2f56957fe9f71a2e7c596a334686320ab2569f1a54e243bfcd3f42ebae17c`  
		Last Modified: Tue, 25 Oct 2022 09:51:59 GMT  
		Size: 10.7 MB (10661828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a57a581172d92713c67937b8552f2518b0661de8146176b186886f6dd01ea188`  
		Last Modified: Tue, 25 Oct 2022 09:52:48 GMT  
		Size: 53.3 MB (53306457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ccceb68786948a50ce81154df52feaca73cb5a8119bd60d29ccf783800f1151`  
		Last Modified: Tue, 25 Oct 2022 09:54:52 GMT  
		Size: 179.0 MB (178980924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e1efefd27f95a1c90511128671f60cedadb21ad92cbb646004d3f8b8077284`  
		Last Modified: Tue, 25 Oct 2022 18:48:46 GMT  
		Size: 179.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05d64f197c024dad88f6b8682bc2e4ef59028a7582cbe77cb3ae319b4c53320`  
		Last Modified: Tue, 25 Oct 2022 18:48:59 GMT  
		Size: 14.4 MB (14436806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:bullseye` - linux; ppc64le

```console
$ docker pull perl@sha256:8c08dbcff7d2427310889d86feefb7e4ad95dc4501520736825e7493c8f11cbf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.3 MB (346259241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de3c6f3a013669be011663319367c06a29e1633c0ef3f62fba5a844ac88f32bb`
-	Default Command: `["perl5.36.0","-de0"]`

```dockerfile
# Tue, 25 Oct 2022 03:13:28 GMT
ADD file:c01a6cc4222fbeeda5c2d679c5b355539880a02c792c64861eb17b81a3678f45 in / 
# Tue, 25 Oct 2022 03:13:31 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:13:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:14:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:14:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:16:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:41:21 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 25 Oct 2022 09:41:22 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 25 Oct 2022 09:41:22 GMT
WORKDIR /usr/src/perl
# Tue, 25 Oct 2022 09:49:01 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.0.tar.xz -o perl-5.36.0.tar.xz     && echo '0f386dccbee8e26286404b2cca144e1005be65477979beb9b1ba272d4819bcf0 *perl-5.36.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.0.tar.xz -C /usr/src/perl     && rm perl-5.36.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Tue, 25 Oct 2022 09:49:02 GMT
WORKDIR /
# Tue, 25 Oct 2022 09:49:03 GMT
CMD ["perl5.36.0" "-de0"]
```

-	Layers:
	-	`sha256:ee5a342763ed1d31bef8cebe9f4cc5dd6d427f630da679a87da0427be7b22e3d`  
		Last Modified: Tue, 25 Oct 2022 03:18:52 GMT  
		Size: 58.9 MB (58916374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a4727f39cbcb19b39abdbd847eeceed842ef65f8514372024c48b913bc951a`  
		Last Modified: Tue, 25 Oct 2022 06:49:00 GMT  
		Size: 5.4 MB (5414507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe601e6c8a1ec9c69c49c65a53339202a65cea9d4f01d161fb34905c06a4a99`  
		Last Modified: Tue, 25 Oct 2022 06:49:01 GMT  
		Size: 11.6 MB (11630153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5055e27b58426c2b637b1c8c179e6abe306e3dfb55a9c170c73fb0d581c6cf3e`  
		Last Modified: Tue, 25 Oct 2022 06:49:31 GMT  
		Size: 58.9 MB (58867355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a503b0a90ce32a745c9586bc6c28360d8de222565d7105d079b530524e1e38`  
		Last Modified: Tue, 25 Oct 2022 06:50:32 GMT  
		Size: 196.2 MB (196199961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88f3626cf5cae999d9e83a8ae4aadfc9558242017c9f3df41a3681f98efaafbb`  
		Last Modified: Tue, 25 Oct 2022 11:21:37 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0867ccb3ef00629edfaf4c42df02dc86330a235525b4afcb54730564f33a684`  
		Last Modified: Tue, 25 Oct 2022 11:21:42 GMT  
		Size: 15.2 MB (15230689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:bullseye` - linux; s390x

```console
$ docker pull perl@sha256:1b2222d547d7baacc0806c007f3fce94310d3a5af047a9ff110318ed73df7c4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.7 MB (311669567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c3192fec8298324f4b358c19d85d8eb7424a1e24ba5772ad47f0a229a53dfc3`
-	Default Command: `["perl5.36.0","-de0"]`

```dockerfile
# Tue, 15 Nov 2022 01:42:23 GMT
ADD file:85bcb55b71ee57dffe1ea720e85546e314d2691e98658779a6f732d13e2e1038 in / 
# Tue, 15 Nov 2022 01:42:32 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 06:24:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 06:24:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 06:25:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 06:26:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 08:23:58 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 15 Nov 2022 08:23:59 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 15 Nov 2022 08:23:59 GMT
WORKDIR /usr/src/perl
# Tue, 15 Nov 2022 08:30:49 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.0.tar.xz -o perl-5.36.0.tar.xz     && echo '0f386dccbee8e26286404b2cca144e1005be65477979beb9b1ba272d4819bcf0 *perl-5.36.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.0.tar.xz -C /usr/src/perl     && rm perl-5.36.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Tue, 15 Nov 2022 08:30:50 GMT
WORKDIR /
# Tue, 15 Nov 2022 08:30:50 GMT
CMD ["perl5.36.0" "-de0"]
```

-	Layers:
	-	`sha256:4b50a7f3d916ceefc2228edab7fc6bc3e2fd142f385b7a04544973edc988c99f`  
		Last Modified: Tue, 15 Nov 2022 01:47:12 GMT  
		Size: 53.3 MB (53271656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0393fb4aa0f74da410291e84bc30299dd564dd10213b10075a53b1b031b797`  
		Last Modified: Tue, 15 Nov 2022 06:35:54 GMT  
		Size: 5.1 MB (5148419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4197b7e030ccca45de7e8f69883bb8230075d4a2145a8eed213e69d9a4f4fcd1`  
		Last Modified: Tue, 15 Nov 2022 06:35:54 GMT  
		Size: 10.8 MB (10766709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87598e81fefd40a632a983853aa6fa90eeff5c83a684745ea038f9ef64dd666`  
		Last Modified: Tue, 15 Nov 2022 06:36:11 GMT  
		Size: 54.1 MB (54055740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617a31a0869734f277432537b66e996de511d0e2ed2dbab793dade4cdb29525b`  
		Last Modified: Tue, 15 Nov 2022 06:36:41 GMT  
		Size: 172.8 MB (172834217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:621ae8f401d908886d57ad53b0e9dc17cc8ece4b9bae1aff66cd323344b86179`  
		Last Modified: Tue, 15 Nov 2022 10:26:26 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27245b00a221bc2e9c11a683b5c65e94e3811e8f75e96a8d05f0667fa4493617`  
		Last Modified: Tue, 15 Nov 2022 10:26:29 GMT  
		Size: 15.6 MB (15592623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
