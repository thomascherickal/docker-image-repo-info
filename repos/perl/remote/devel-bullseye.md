## `perl:devel-bullseye`

```console
$ docker pull perl@sha256:8f4f8bd9457d38cf073c456a7abfe3210637409c270cd3fc53cca55902090f39
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

### `perl:devel-bullseye` - linux; amd64

```console
$ docker pull perl@sha256:ca4f68beb7290bdcb357d0d7779c32d86fdf742f8eb564b939f89841e2ef7d50
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.9 MB (337874756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9a2124f97194d6ae75d92b2107751dab725565af465e6f3bcf4827c20524175`
-	Default Command: `["perl5.39.2","-de0"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:57 GMT
ADD file:20f89ff93bfbd6c9fb1a97058a1f3de4485a8974e8a83892072c511fbd2e4134 in / 
# Wed, 16 Aug 2023 00:59:58 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 06:59:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 06:59:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 07:00:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 10:50:53 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 16 Aug 2023 10:50:53 GMT
WORKDIR /usr/src/perl
# Tue, 22 Aug 2023 20:44:09 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.2.tar.xz -o perl-5.39.2.tar.xz     && echo 'b7ae33d3c6ff80107d14c92dfb3d8d4944fec926b11bcc40c8764b73c710694f *perl-5.39.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.2.tar.xz -C /usr/src/perl     && rm perl-5.39.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 22 Aug 2023 20:44:10 GMT
WORKDIR /usr/src/app
# Tue, 22 Aug 2023 20:44:10 GMT
CMD ["perl5.39.2" "-de0"]
```

-	Layers:
	-	`sha256:6a70103cc499a199e10e379794c60aa524d9598587cc2bdfe2995642c2da8df7`  
		Last Modified: Wed, 16 Aug 2023 01:04:50 GMT  
		Size: 55.1 MB (55056621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb4221e2c63c35bb16b63f6d24c104c7ea5d453997636c2244b66884f540537`  
		Last Modified: Wed, 16 Aug 2023 07:13:46 GMT  
		Size: 15.8 MB (15760534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe6e67e69c83952779c1fb8add0b6f81ba6fb03f6290c62225fbdae94c28661`  
		Last Modified: Wed, 16 Aug 2023 07:14:03 GMT  
		Size: 54.6 MB (54584778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea30286b46fb9b823a797bdd0875e26853140b5424981da88967cd7131ccef8b`  
		Last Modified: Wed, 16 Aug 2023 07:14:33 GMT  
		Size: 196.9 MB (196851887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b6b644af1675587ab2b873e3aba5ccf4d50c6e3d877c13a0ea352ca655420e`  
		Last Modified: Wed, 16 Aug 2023 14:37:00 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472c970762300f7ea91226efc3f905cc7d4d997515e6b8a1b7120ee6f9b89235`  
		Last Modified: Tue, 22 Aug 2023 21:22:34 GMT  
		Size: 15.6 MB (15620603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879267bd4618c6d2f930e3f4323c4a550aa955827f6a40b5fb7b35a9ad5a6a99`  
		Last Modified: Tue, 22 Aug 2023 21:22:31 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-bullseye` - linux; arm variant v5

```console
$ docker pull perl@sha256:6f01d3ecc3f810c16483b0928908101f5b246d1a6406d029081fd7672f4f659c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.2 MB (310232092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93c277348dc0e81d76e411c6665ea96a351378900fc4ad5bb1a8286f061adc12`
-	Default Command: `["perl5.39.2","-de0"]`

```dockerfile
# Tue, 15 Aug 2023 23:48:40 GMT
ADD file:d044e64aab907424be649252b5ff1d9f5e8c9494db5b60c0e54f5962bfb73478 in / 
# Tue, 15 Aug 2023 23:48:40 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:42:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:42:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:44:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:52:11 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 16 Aug 2023 00:52:11 GMT
WORKDIR /usr/src/perl
# Tue, 22 Aug 2023 19:53:54 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.2.tar.xz -o perl-5.39.2.tar.xz     && echo 'b7ae33d3c6ff80107d14c92dfb3d8d4944fec926b11bcc40c8764b73c710694f *perl-5.39.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.2.tar.xz -C /usr/src/perl     && rm perl-5.39.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 22 Aug 2023 19:53:55 GMT
WORKDIR /usr/src/app
# Tue, 22 Aug 2023 19:53:55 GMT
CMD ["perl5.39.2" "-de0"]
```

-	Layers:
	-	`sha256:0b63bbf2e6f6026dfaed9cbedf777472a04812b7d291501b1d416e49e3ce885e`  
		Last Modified: Tue, 15 Aug 2023 23:51:54 GMT  
		Size: 52.6 MB (52558130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf207734195f34506f2f636cb92d7f51b200a26c1264dcbb6ba6e8de4ad0a3f1`  
		Last Modified: Wed, 16 Aug 2023 00:48:08 GMT  
		Size: 15.4 MB (15369116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24def812da7393c114766d8e90ea33083736120f2e8410c43c6e3293f0c5c898`  
		Last Modified: Wed, 16 Aug 2023 00:48:25 GMT  
		Size: 52.3 MB (52340723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997fb3aae8d3febae5665017c86770b153edfad7973f9c0f8799ae76c9cc4e9a`  
		Last Modified: Wed, 16 Aug 2023 00:48:57 GMT  
		Size: 175.0 MB (175039510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2145c651d163302efc0dcddf4ac4d742e40fb23eaed2c5b6793ce28818d075f9`  
		Last Modified: Wed, 16 Aug 2023 02:31:37 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098ad51d94c154d87fc34d286820206c31610887707a77b1a293991169f6b10b`  
		Last Modified: Tue, 22 Aug 2023 20:13:05 GMT  
		Size: 14.9 MB (14924279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:817ec0473bd9615aa1717e7430da4d1e0a6acf064f88ab76cd730a9924b97d8d`  
		Last Modified: Tue, 22 Aug 2023 20:13:01 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-bullseye` - linux; arm variant v7

```console
$ docker pull perl@sha256:3a71a5f187717ca6c6cdde4a4ded27e239681aabeee2d1072a3e5c3d252a512b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.5 MB (297497883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3eed47b1cdcf5ed60ba4165d673d0c26ca13e7960573689bb5129d605396ae0d`
-	Default Command: `["perl5.39.2","-de0"]`

```dockerfile
# Wed, 16 Aug 2023 00:17:21 GMT
ADD file:b529de8b48c1e507ad6f29320c3c5cd83d8d06fa66e8d89bb62faff62700e9f2 in / 
# Wed, 16 Aug 2023 00:17:22 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:30:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:30:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:31:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 08:02:14 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 16 Aug 2023 08:02:14 GMT
WORKDIR /usr/src/perl
# Tue, 22 Aug 2023 20:14:12 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.2.tar.xz -o perl-5.39.2.tar.xz     && echo 'b7ae33d3c6ff80107d14c92dfb3d8d4944fec926b11bcc40c8764b73c710694f *perl-5.39.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.2.tar.xz -C /usr/src/perl     && rm perl-5.39.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 22 Aug 2023 20:14:12 GMT
WORKDIR /usr/src/app
# Tue, 22 Aug 2023 20:14:12 GMT
CMD ["perl5.39.2" "-de0"]
```

-	Layers:
	-	`sha256:c53151c23650f086e15d3652b8a931fb4623765c0112e8adc74eb8853c8c9232`  
		Last Modified: Wed, 16 Aug 2023 00:21:46 GMT  
		Size: 50.2 MB (50219496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbe9a81a850f9760477ffa3083b63d636090316a05f81146ffd62a60638926a`  
		Last Modified: Wed, 16 Aug 2023 05:48:44 GMT  
		Size: 14.9 MB (14868833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c49800a0424211a8cc1edf5a26d1ebd1afb7c017be3b08cadf2d25abb85d291b`  
		Last Modified: Wed, 16 Aug 2023 05:49:04 GMT  
		Size: 50.4 MB (50355668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea65231b804ff3a87553e9e8aacba0dd7e706dcceac6cf36be583fbfde69d20`  
		Last Modified: Wed, 16 Aug 2023 05:49:40 GMT  
		Size: 167.3 MB (167333015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd87a0cb0e419ebff2f18626e853664381e0d3e69678cd791cdfd1b54d08197a`  
		Last Modified: Wed, 16 Aug 2023 11:55:35 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9e1c027861a0e598968eefa3be18cf5c2f32d68dc9ed556a37e275f7cb29d2`  
		Last Modified: Tue, 22 Aug 2023 20:50:41 GMT  
		Size: 14.7 MB (14720536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99f81b0a00fd6ee586a015ee8dae40ede1da67095f3030bd5d3a9c7c83246ea`  
		Last Modified: Tue, 22 Aug 2023 20:50:37 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-bullseye` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:308078429fbc7c72c59d4f08a0a383f0409b878d203cc708948fd9538d856088
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.5 MB (329465537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7b18e3c649fdd4fe953f681b8a881f86677f4a9862efe09045dad8869045c26`
-	Default Command: `["perl5.39.2","-de0"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:03 GMT
ADD file:8973cddb2d84a543b71001635599951bea6485a3526ae4ff916443b584864c83 in / 
# Tue, 15 Aug 2023 23:40:04 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:23:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:23:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:24:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 10:44:00 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 16 Aug 2023 10:44:00 GMT
WORKDIR /usr/src/perl
# Tue, 22 Aug 2023 20:22:14 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.2.tar.xz -o perl-5.39.2.tar.xz     && echo 'b7ae33d3c6ff80107d14c92dfb3d8d4944fec926b11bcc40c8764b73c710694f *perl-5.39.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.2.tar.xz -C /usr/src/perl     && rm perl-5.39.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 22 Aug 2023 20:22:15 GMT
WORKDIR /usr/src/app
# Tue, 22 Aug 2023 20:22:15 GMT
CMD ["perl5.39.2" "-de0"]
```

-	Layers:
	-	`sha256:e837d9f05c625de5b814b851adbc03559ba02ea7078f57c81a01e18fc65bf42b`  
		Last Modified: Tue, 15 Aug 2023 23:43:37 GMT  
		Size: 53.7 MB (53704779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abd0588cbb35597a784666f0dc97746829b8b4b730b73e8781fb90678ffef22`  
		Last Modified: Wed, 16 Aug 2023 01:39:26 GMT  
		Size: 15.7 MB (15746520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a8864a846a08e10fbf877e73678d1f0803227b00a1b16d9ba948070c6e58f6`  
		Last Modified: Wed, 16 Aug 2023 01:39:40 GMT  
		Size: 54.7 MB (54676094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db5ec7e6673db06ba035c7c57c4c31b84c89e803ceeb3268a02b5175537b120`  
		Last Modified: Wed, 16 Aug 2023 01:40:04 GMT  
		Size: 189.8 MB (189777874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e05d57fc6aae481fa7ca468fcecaf1f96ac373106db91f979cb97f39ec2ea41`  
		Last Modified: Wed, 16 Aug 2023 13:47:42 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9988662eb29a83a9311251c41adb5c52101f4ca31dea331b4132441ac299624f`  
		Last Modified: Tue, 22 Aug 2023 20:53:38 GMT  
		Size: 15.6 MB (15559937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d03fd5b3d7056398e22be9f04433d910b6ac9febedb8806cf31b6684272bf9`  
		Last Modified: Tue, 22 Aug 2023 20:53:35 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-bullseye` - linux; 386

```console
$ docker pull perl@sha256:c4effa700bb247542a3b105364abb2af87d38120e8090e18acc041bf25a6021e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.1 MB (343118271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aeee04fe4dea38a8d12a000b91b98473738d662fb563057958a5cc7cda3e26f6`
-	Default Command: `["perl5.39.2","-de0"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:11 GMT
ADD file:efc88a19b31e68ca41f555bcc51338b0f135cbbd72b90637d8c73969d53addd2 in / 
# Tue, 15 Aug 2023 23:39:12 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:27:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:28:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:29:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 09:56:57 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 16 Aug 2023 09:56:57 GMT
WORKDIR /usr/src/perl
# Tue, 22 Aug 2023 20:03:14 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.2.tar.xz -o perl-5.39.2.tar.xz     && echo 'b7ae33d3c6ff80107d14c92dfb3d8d4944fec926b11bcc40c8764b73c710694f *perl-5.39.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.2.tar.xz -C /usr/src/perl     && rm perl-5.39.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 22 Aug 2023 20:03:14 GMT
WORKDIR /usr/src/app
# Tue, 22 Aug 2023 20:03:14 GMT
CMD ["perl5.39.2" "-de0"]
```

-	Layers:
	-	`sha256:822e033fa7b169545d5890de01438a9dd87774ff938ff440e823a3ec3f73996d`  
		Last Modified: Tue, 15 Aug 2023 23:43:47 GMT  
		Size: 56.0 MB (56040520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52269d7973f191a6cedbd1545cfe71ec1c659072be43d51f8741b18f05423e2b`  
		Last Modified: Wed, 16 Aug 2023 00:36:01 GMT  
		Size: 16.3 MB (16263743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16fc8bca4c44908804dd201eac5ad8d9316cffd0de391511a9da2fcb3fb48c0`  
		Last Modified: Wed, 16 Aug 2023 00:36:22 GMT  
		Size: 55.9 MB (55922930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da0010c52f973a4d9c39043ad90ee5727579d72d1a34209b0ccc3f1f80515cc`  
		Last Modified: Wed, 16 Aug 2023 00:37:05 GMT  
		Size: 199.8 MB (199768301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cd9bd865e76a6c08b116e558ac330e4e6a9a7c2d60eb90d6a678a57904e899`  
		Last Modified: Wed, 16 Aug 2023 16:28:51 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7b4f7c248542e703629c3f6b5bb738902632a1b08bcedf65e2acef875ee117`  
		Last Modified: Tue, 22 Aug 2023 21:07:26 GMT  
		Size: 15.1 MB (15122443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbbfbde97cde79292dae10bedb29778bf379f668b8c7dd9698d3ddc542596e0f`  
		Last Modified: Tue, 22 Aug 2023 21:07:22 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-bullseye` - linux; mips64le

```console
$ docker pull perl@sha256:156a796627b130ec75c93bbccf23d98ed03c67e7a42fa093ca33ca15029c3e64
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **315.9 MB (315907071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6be7a1eb78eff3428b4f4af8a93fc3a80b436daf50cd56f66086bde5a40e488`
-	Default Command: `["perl5.39.2","-de0"]`

```dockerfile
# Wed, 16 Aug 2023 00:09:18 GMT
ADD file:c0b984cd41325dc5f83fb228f8b95bd38027d8860098ac574a960400eaf0d976 in / 
# Wed, 16 Aug 2023 00:09:23 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 14:42:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 14:44:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 14:49:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 15:29:36 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 17 Aug 2023 15:29:42 GMT
WORKDIR /usr/src/perl
# Tue, 22 Aug 2023 20:30:39 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.2.tar.xz -o perl-5.39.2.tar.xz     && echo 'b7ae33d3c6ff80107d14c92dfb3d8d4944fec926b11bcc40c8764b73c710694f *perl-5.39.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.2.tar.xz -C /usr/src/perl     && rm perl-5.39.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 22 Aug 2023 20:30:46 GMT
WORKDIR /usr/src/app
# Tue, 22 Aug 2023 20:30:52 GMT
CMD ["perl5.39.2" "-de0"]
```

-	Layers:
	-	`sha256:4a039678eb41cc8e7dbd73bbab533513108157d96943588a97c7fac7c940eaca`  
		Last Modified: Wed, 16 Aug 2023 00:20:18 GMT  
		Size: 53.3 MB (53271564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37719351c516618a1b419df971327e9fc181adfb609ab0d1e1a494bcdc589ec5`  
		Last Modified: Wed, 16 Aug 2023 15:03:41 GMT  
		Size: 15.5 MB (15520474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a7c370f765877745d0fcdbd981faf357168fab30f68042ea0c34904352a04a`  
		Last Modified: Wed, 16 Aug 2023 15:04:24 GMT  
		Size: 53.3 MB (53306356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff1c96b496d2d806cd19b41b6a58f4be261e3322ff930f29f13175e3302718a`  
		Last Modified: Wed, 16 Aug 2023 15:06:18 GMT  
		Size: 179.0 MB (178973985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2b7eeb564300e7745d6646d32f019258d091fd26a956c53bf4e4a035580bc32`  
		Last Modified: Thu, 17 Aug 2023 21:51:10 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68337cb57b146b24665cb650fcab962f935f19639068736e7d20524556ac678f`  
		Last Modified: Tue, 22 Aug 2023 21:46:18 GMT  
		Size: 14.8 MB (14834424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d945be6ee08f564feb467875257699679e46f7b5a29e7817f4c1cf1954cde8`  
		Last Modified: Tue, 22 Aug 2023 21:46:05 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-bullseye` - linux; ppc64le

```console
$ docker pull perl@sha256:08a83c9280125e412c2432850873d84a15494b809d31e1b3384c71de2715d922
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.4 MB (346370065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7a1ac130ae3d5910d7a01da86ec718d4e4a813c5fbdf37b0c12b0fec54ee3c0`
-	Default Command: `["perl5.39.2","-de0"]`

```dockerfile
# Wed, 16 Aug 2023 01:09:50 GMT
ADD file:23fe4ecb2d3d302e0df50109aee416120a138fad47d1614500f98b65fa288281 in / 
# Wed, 16 Aug 2023 01:09:54 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:43:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:44:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:48:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 09:22:44 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 16 Aug 2023 09:22:44 GMT
WORKDIR /usr/src/perl
# Tue, 22 Aug 2023 20:38:10 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.2.tar.xz -o perl-5.39.2.tar.xz     && echo 'b7ae33d3c6ff80107d14c92dfb3d8d4944fec926b11bcc40c8764b73c710694f *perl-5.39.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.2.tar.xz -C /usr/src/perl     && rm perl-5.39.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 22 Aug 2023 20:38:11 GMT
WORKDIR /usr/src/app
# Tue, 22 Aug 2023 20:38:12 GMT
CMD ["perl5.39.2" "-de0"]
```

-	Layers:
	-	`sha256:148c97e5e41c60dd4fc440664aeee1e57ab7158b53ea7d1f9132198b3d35bc5e`  
		Last Modified: Wed, 16 Aug 2023 01:16:30 GMT  
		Size: 58.9 MB (58928436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901a6153e1feb9026260a32acce3bc3acf29f7186a1458d2b343ee865d054c45`  
		Last Modified: Wed, 16 Aug 2023 02:11:21 GMT  
		Size: 16.8 MB (16753019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264ca3322295f7e8f8f191650911a824de696e167ce08aee16d14b5704ea4d14`  
		Last Modified: Wed, 16 Aug 2023 02:11:48 GMT  
		Size: 58.9 MB (58865273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c8e5a575991fb77e9e7207e17459595a4a3bd1add713086e44f7190d05ac9b`  
		Last Modified: Wed, 16 Aug 2023 02:12:43 GMT  
		Size: 196.2 MB (196199625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f970dc377ab9f9b0b9ace3e122802d5fdb696ddda896cb8122abfeaa21d758b0`  
		Last Modified: Wed, 16 Aug 2023 11:47:00 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4420feffd2f326df42656fe92c5cc7ba2fed985979dfa77e803f9d192baf9e`  
		Last Modified: Tue, 22 Aug 2023 21:05:57 GMT  
		Size: 15.6 MB (15623379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a79bbcfcbb6f60a6f3204b53cd1e7c1d11a21cdc5cbed972139e43f58cba2ee`  
		Last Modified: Tue, 22 Aug 2023 21:05:52 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-bullseye` - linux; s390x

```console
$ docker pull perl@sha256:9ec597c5d6582637f93c2b61d5e1b8560c008a5e0721230f7a0c8d1b9ee3e9da
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.8 MB (311819316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09a4bc40618296d9cf7dd149bede1534b88d0bbf350fb1073af54a1d62d991ba`
-	Default Command: `["perl5.39.2","-de0"]`

```dockerfile
# Tue, 15 Aug 2023 23:42:43 GMT
ADD file:021ebd89eb6b326058b4fc3aeca5d0d93925ed29a443618fedef034618e8f2db in / 
# Tue, 15 Aug 2023 23:42:48 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 04:22:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:22:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:24:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 11:53:13 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 16 Aug 2023 11:53:13 GMT
WORKDIR /usr/src/perl
# Tue, 22 Aug 2023 19:56:41 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.2.tar.xz -o perl-5.39.2.tar.xz     && echo 'b7ae33d3c6ff80107d14c92dfb3d8d4944fec926b11bcc40c8764b73c710694f *perl-5.39.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.2.tar.xz -C /usr/src/perl     && rm perl-5.39.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 22 Aug 2023 19:56:42 GMT
WORKDIR /usr/src/app
# Tue, 22 Aug 2023 19:56:42 GMT
CMD ["perl5.39.2" "-de0"]
```

-	Layers:
	-	`sha256:cf9beb6f1941863d1df3b7a9c4f925894662762a3ceeba920f164d9e8c8bab57`  
		Last Modified: Tue, 15 Aug 2023 23:48:07 GMT  
		Size: 53.3 MB (53290642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431e34cc72373b43e9a06943d5dbedf8eb4769be085ac405ff5a810430093689`  
		Last Modified: Wed, 16 Aug 2023 04:37:08 GMT  
		Size: 15.6 MB (15631927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a44c13aebe3a1d06fd7930da9581f9ac789e148f33dd9a84008de9e5da614208`  
		Last Modified: Wed, 16 Aug 2023 04:37:22 GMT  
		Size: 54.1 MB (54061692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e83fba4183bca79f260d587a76c94532cc7c3a0419169722dbbee232fee2d9dc`  
		Last Modified: Wed, 16 Aug 2023 04:37:47 GMT  
		Size: 172.9 MB (172855751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e0ec8719ff07f468ab925aa52161fdac4d223f2e7bddfeae2ed608467e36a1`  
		Last Modified: Wed, 16 Aug 2023 12:42:17 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f32b0ea529fabcabf8fe62ee0c495790ab6ea1be11c4a1602c5ee1b36ac58f`  
		Last Modified: Tue, 22 Aug 2023 20:16:56 GMT  
		Size: 16.0 MB (15978969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:246c63a4e7b27cb3e54fe7f2d0554436d0efb12b6cf7c1a477ff91738663e12c`  
		Last Modified: Tue, 22 Aug 2023 20:16:52 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
