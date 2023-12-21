## `perl:threaded-bookworm`

```console
$ docker pull perl@sha256:197762c44989f03abee3c98e62095565a34e9912e566a2bd975f8b25220b29e9
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 13
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v5
	-	unknown; unknown
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	unknown; unknown
	-	linux; mips64le
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `perl:threaded-bookworm` - linux; amd64

```console
$ docker pull perl@sha256:91fd290a1b921bb673467cb225aeed38feb24e84fc3d736c77f4ecdea863c8ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **364.5 MB (364530493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0b41cb2075ea52586c53d7a79da8722c9be66b1811cfa2dee7205bf03d24b81`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Thu, 30 Nov 2023 02:54:02 GMT
ADD file:7d8adf68670e8dc2af6b8603870ea610fc65ecbb08799f2ca6a3134f5d47d289 in / 
# Thu, 30 Nov 2023 02:54:02 GMT
CMD ["bash"]
# Thu, 30 Nov 2023 02:54:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 30 Nov 2023 02:54:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 30 Nov 2023 02:54:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 30 Nov 2023 02:54:02 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 30 Nov 2023 02:54:02 GMT
WORKDIR /usr/src/perl
# Thu, 30 Nov 2023 02:54:02 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version # buildkit
# Thu, 30 Nov 2023 02:54:02 GMT
WORKDIR /usr/src/app
# Thu, 30 Nov 2023 02:54:02 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:bc0734b949dcdcabe5bfdf0c8b9f44491e0fce04cb10c9c6e76282b9f6abdf01`  
		Last Modified: Tue, 19 Dec 2023 01:24:35 GMT  
		Size: 49.6 MB (49561579 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b5de22c0f5cd2ea2bb6c0524478db95bff5a294c99419ccd4a9d3ccc9873bad9`  
		Last Modified: Tue, 19 Dec 2023 04:41:08 GMT  
		Size: 24.0 MB (24046123 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:917ee5330e73737d6095a802333d311648959399ff2c067150890162e720f863`  
		Last Modified: Tue, 19 Dec 2023 04:41:27 GMT  
		Size: 64.1 MB (64131542 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b43bd898d5fbe0e1606380820047fd1e8b421722c9e69ac12757474305bd6702`  
		Last Modified: Tue, 19 Dec 2023 04:42:04 GMT  
		Size: 211.1 MB (211097790 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5f2a99ea5c6870f9360c22a8c0b6692e2a35e3c619ddb12d2a8b142c903c8064`  
		Last Modified: Wed, 20 Dec 2023 20:16:28 GMT  
		Size: 136.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b8f128b9a3cc29e35d84fd7b99733118e8663f6a84bebc6ae3bc293a6757e35c`  
		Last Modified: Wed, 20 Dec 2023 20:16:29 GMT  
		Size: 15.7 MB (15693191 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1f511aa8a8844cdcc893f530c04850ac556168e98df7c560c57a91b15d0e17a4`  
		Last Modified: Wed, 20 Dec 2023 20:16:28 GMT  
		Size: 132.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `perl:threaded-bookworm` - unknown; unknown

```console
$ docker pull perl@sha256:6f82172795597f9d84c9e939350e696ef3c62b2fe44e86a0a9c6bf2e766f9fcb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13421378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a6b3ff4b3ca82cd90a5c3e81f5de71b249a11391997809d74e8c3a5872c2565`

```dockerfile
```

-	Layers:
	-	`sha256:b5483afc36a51324c8fbc515fb7f255195078d5c048a48c82763a82ec3f0eb00`  
		Last Modified: Wed, 20 Dec 2023 20:16:29 GMT  
		Size: 13.4 MB (13403331 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:922bcb619a834b81af4c2c1c1a17f3f5ef80e318df2626afdef0d070905a2a8b`  
		Last Modified: Wed, 20 Dec 2023 20:16:28 GMT  
		Size: 18.0 KB (18047 bytes)  
		MIME: application/vnd.in-toto+json

### `perl:threaded-bookworm` - linux; arm variant v5

```console
$ docker pull perl@sha256:65fca4128be8114e3b8053144d6f90b5a974fa0b09ecbd76f4ebb2bb3a5a3fff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.9 MB (330927032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ba71c857f4784ab5fadea18f01d162e5a20ee071162e434541de66c6a59e4a9`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Thu, 30 Nov 2023 02:54:02 GMT
ADD file:a6a83a649ad34de44e3b18ac2ef474733028a38445b36395b37a47906a17e460 in / 
# Thu, 30 Nov 2023 02:54:02 GMT
CMD ["bash"]
# Thu, 30 Nov 2023 02:54:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 30 Nov 2023 02:54:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 30 Nov 2023 02:54:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 30 Nov 2023 02:54:02 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 30 Nov 2023 02:54:02 GMT
WORKDIR /usr/src/perl
# Thu, 30 Nov 2023 02:54:02 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version # buildkit
# Thu, 30 Nov 2023 02:54:02 GMT
WORKDIR /usr/src/app
# Thu, 30 Nov 2023 02:54:02 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:f3aac8ada11b4cd51c598b397af8986343d5ffa06ce2a7a7c7c80f4ea6f5e522`  
		Last Modified: Tue, 19 Dec 2023 01:58:07 GMT  
		Size: 47.3 MB (47319238 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a0fd25a16876a3944cbd080157b9e23fe47b07ccfaa03a3b8075979027a60208`  
		Last Modified: Tue, 19 Dec 2023 05:31:23 GMT  
		Size: 22.7 MB (22724641 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f6dd8a0a191b42cdb49dcb6ca7c111242e7ef4d447f3b729605f30173433bba2`  
		Last Modified: Tue, 19 Dec 2023 05:31:46 GMT  
		Size: 61.5 MB (61508870 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fe5ddaed1389aec60f80faad6640540555cb8a57f3acbc1566f210c60f5773d9`  
		Last Modified: Tue, 19 Dec 2023 05:32:27 GMT  
		Size: 184.4 MB (184416924 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9eb572e40cc22058b20b4f79a200e14f80a5200853df4aa2bbf0e0cf3a47c7c4`  
		Last Modified: Wed, 20 Dec 2023 20:46:02 GMT  
		Size: 135.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:629cc3b1dd844aa9bc933cf77be050adaaa2b4bc4a95c2007986149878b48aff`  
		Last Modified: Wed, 20 Dec 2023 21:27:37 GMT  
		Size: 15.0 MB (14957092 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c8597f894fb9730cc15cc15bddcbab4b1f3f2baa7b459e1f6162899e757e230`  
		Last Modified: Wed, 20 Dec 2023 21:27:36 GMT  
		Size: 132.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `perl:threaded-bookworm` - unknown; unknown

```console
$ docker pull perl@sha256:26b2a51f2bdf8151804c9ba57ffbabdea6d1bd45572344b8f30239d2e524231b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 KB (17287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4afe858a36146345e114e070e803d39bffc96dc6d69aca518028661422dd910`

```dockerfile
```

-	Layers:
	-	`sha256:0133c0b4a2728bd022f72d6cfc42039c7909f869dbb43f05f88d9ec9b4bf4276`  
		Last Modified: Wed, 20 Dec 2023 21:27:36 GMT  
		Size: 17.3 KB (17287 bytes)  
		MIME: application/vnd.in-toto+json

### `perl:threaded-bookworm` - linux; arm variant v7

```console
$ docker pull perl@sha256:4cb0dc6abc93d42b9e2b218e217bf79c12cf7938ba082c4da5e0df86b0b22f39
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.1 MB (316141812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5e4fa06168de3ed7682d4c761ef5b81e18881cf8d0e109dfdb39354b9c5dc9e`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Tue, 19 Dec 2023 02:07:39 GMT
ADD file:1633615de1824a95e35747f0133e90ab5ddc138574a83fb9c4f337cf45762574 in / 
# Tue, 19 Dec 2023 02:07:39 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 07:54:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 07:55:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 07:56:32 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 16:58:53 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 19 Dec 2023 16:58:53 GMT
WORKDIR /usr/src/perl
# Tue, 19 Dec 2023 17:21:19 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 19 Dec 2023 17:21:19 GMT
WORKDIR /usr/src/app
# Tue, 19 Dec 2023 17:21:19 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:89cc9e7932dc0f797e6c3fc84b4c6868fedaca1b174b38a51e152a23a643be7a`  
		Last Modified: Tue, 19 Dec 2023 02:11:28 GMT  
		Size: 45.2 MB (45156699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1cce8fac77d35b90037c77fcb46603ed4cdc1388009887c5132cbdf3531132`  
		Last Modified: Tue, 19 Dec 2023 08:06:19 GMT  
		Size: 21.9 MB (21949134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258af69dcb8426bcc3ebc63b670048d9d4191fd206986dd72f83a247768f7f65`  
		Last Modified: Tue, 19 Dec 2023 08:06:39 GMT  
		Size: 59.2 MB (59216125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba6fc4113c5eec43c041f3fe9cca3eae36c8a6cffe2cc7fe2b7089fba2bf7cb`  
		Last Modified: Tue, 19 Dec 2023 08:07:16 GMT  
		Size: 175.1 MB (175078779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33a345ee848040f93d1430a7a30ca912f0847f9c0459c6437b4d0770d9d18e9`  
		Last Modified: Tue, 19 Dec 2023 18:55:57 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b58b17ce991c9aee5be5004d43a48b4e47c704257e935b9efc22b4db4f51d9`  
		Last Modified: Tue, 19 Dec 2023 18:57:15 GMT  
		Size: 14.7 MB (14740742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd35297e7f46cb23ff66dab3f74b2173a22f6d5cd596d062edb8671ec3dbac30`  
		Last Modified: Tue, 19 Dec 2023 18:57:11 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded-bookworm` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:2aa93250f4cef6617596ec5254065334e4de9281666e9127dd6160596ea42c82
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.3 MB (355293798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7409280a8c64341300fd81269cff552242794c44c002b0ae9e22319dbf6a092e`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:02 GMT
ADD file:412f80f75ed3e520f767e70b6b27fc81807f62fc5c6e5adf756507e33af9fa6b in / 
# Tue, 19 Dec 2023 01:41:02 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 11:33:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 11:34:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 11:34:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 14:30:19 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 19 Dec 2023 14:30:19 GMT
WORKDIR /usr/src/perl
# Tue, 19 Dec 2023 14:48:36 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 19 Dec 2023 14:48:36 GMT
WORKDIR /usr/src/app
# Tue, 19 Dec 2023 14:48:37 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:b66b4ecd3ecfb67b3b7a2a44b0199cbdfc94965c8bd3fefab75cd2e612799740`  
		Last Modified: Tue, 19 Dec 2023 01:44:14 GMT  
		Size: 49.6 MB (49592259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c641d36985b2db859fc64c43a6dbf7c25cdf73e5d16d107fab1d95a840bb4e1`  
		Last Modified: Tue, 19 Dec 2023 11:42:17 GMT  
		Size: 23.6 MB (23582271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd8544b6e15c7a4096b1f48a67fb5bed2efba509fca597f1c164b582ab01c02`  
		Last Modified: Tue, 19 Dec 2023 11:42:35 GMT  
		Size: 64.0 MB (63988289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae58c7c06d64a1a86430205c774637c7615d1365a575b256801bb23390ad5260`  
		Last Modified: Tue, 19 Dec 2023 11:43:05 GMT  
		Size: 202.5 MB (202484237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeea1e4e4e1d28f65d8bc4a034973f51e95438dafe279afe1c64c6bbba959dc7`  
		Last Modified: Tue, 19 Dec 2023 16:04:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2126f44d4231fb9376e908a221cd3e07d6f2eb810637b35533ff2c041d989632`  
		Last Modified: Tue, 19 Dec 2023 16:05:58 GMT  
		Size: 15.6 MB (15646406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba6ad408c41c0eb36e837b0947a47ea0896c28ccae8f6e18038114ac86a1926`  
		Last Modified: Tue, 19 Dec 2023 16:05:55 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded-bookworm` - linux; 386

```console
$ docker pull perl@sha256:dd0edc320c6aa5f096d7a68e68d7748523fb8390f2fa0f4b57e71c9f0392ac72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **366.7 MB (366713785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:910375d767806176db5ed5908606811a8ed2620e8fecd33fbaeccdc95f96421e`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Thu, 30 Nov 2023 02:54:02 GMT
ADD file:c20aace531a43765f8c1b69c75d7f46a4ab443377a663ab47e0bb2ceb013a611 in / 
# Thu, 30 Nov 2023 02:54:02 GMT
CMD ["bash"]
# Thu, 30 Nov 2023 02:54:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 30 Nov 2023 02:54:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 30 Nov 2023 02:54:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 30 Nov 2023 02:54:02 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 30 Nov 2023 02:54:02 GMT
WORKDIR /usr/src/perl
# Thu, 30 Nov 2023 02:54:02 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version # buildkit
# Thu, 30 Nov 2023 02:54:02 GMT
WORKDIR /usr/src/app
# Thu, 30 Nov 2023 02:54:02 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:9b51fe964cb335e4bc3b61dca07146c7a0aa4c31e5ae9fec90f2a950818a21a4`  
		Last Modified: Tue, 19 Dec 2023 01:43:18 GMT  
		Size: 50.6 MB (50582312 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:55fb12d611be5489722de01a39ed212f0e3a188c63409b25d91b51db39be5cb9`  
		Last Modified: Tue, 19 Dec 2023 03:36:07 GMT  
		Size: 24.9 MB (24883625 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:134a33947619311fada004e8d19522ee356dc9b4aefb1e43a67f9b239a793bef`  
		Last Modified: Tue, 19 Dec 2023 03:36:31 GMT  
		Size: 66.0 MB (65980921 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7f0d6b307a56e19161f69c60eb7c94378540e6b20f49d8b1039becdeb53cdde5`  
		Last Modified: Tue, 19 Dec 2023 03:37:24 GMT  
		Size: 210.0 MB (210025484 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8b5a05c77949378c0801d78048b42200785042a2138373fa32088caccb44ea26`  
		Last Modified: Wed, 20 Dec 2023 20:23:53 GMT  
		Size: 135.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:16baf308efc730e652b630f4e1780683f280011aa5efa5b19bde6a460e714780`  
		Last Modified: Wed, 20 Dec 2023 20:23:54 GMT  
		Size: 15.2 MB (15241176 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89f31d35c33398400c2ec852c2ad44582913bdb07689fb4eb81725fc1a05446f`  
		Last Modified: Wed, 20 Dec 2023 20:23:53 GMT  
		Size: 132.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `perl:threaded-bookworm` - unknown; unknown

```console
$ docker pull perl@sha256:ee10103c250e3b03787b566bc07039e2ca93a311e8198891230ab3c9f5a587b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.8 KB (17773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db475a9585739accc5b65e147d7889ff2bf07d5539a9c7a819e88fffd12aef75`

```dockerfile
```

-	Layers:
	-	`sha256:f14060aaa294cff01612535d49abd3445b05677e359af26e1458b78e7e86397f`  
		Last Modified: Wed, 20 Dec 2023 20:23:53 GMT  
		Size: 17.8 KB (17773 bytes)  
		MIME: application/vnd.in-toto+json

### `perl:threaded-bookworm` - linux; mips64le

```console
$ docker pull perl@sha256:1f8001eaabd4851b864a2af1a5be4756a765b8b73acb714cfb49522889ad36d2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.7 MB (340746633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea60b0c3a7ad5956061b6551383d686c412c1c272572be2fb1dce1d15b9dad6b`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Tue, 19 Dec 2023 02:12:55 GMT
ADD file:87d7b313e4309f5e9ad824dfd7dc6f9a85458ccb7056f5001dc6066e964eabcb in / 
# Tue, 19 Dec 2023 02:13:00 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:50:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 02:52:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 02:57:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 07:27:47 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 19 Dec 2023 07:27:53 GMT
WORKDIR /usr/src/perl
# Tue, 19 Dec 2023 09:26:22 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 19 Dec 2023 09:26:28 GMT
WORKDIR /usr/src/app
# Tue, 19 Dec 2023 09:26:35 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:659946beb815c8c0157caa0571c5512c4508ff0fe3bbb59e9513e933c7023366`  
		Last Modified: Tue, 19 Dec 2023 02:23:53 GMT  
		Size: 49.5 MB (49548860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65baf0481eb7e4d5215eb36d70ba1c460bd80282806d1e361c83f4c442ed9adf`  
		Last Modified: Tue, 19 Dec 2023 03:18:48 GMT  
		Size: 23.6 MB (23630657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3c3175afa4d6bd28886bc3fbd23dcc38227468b970b9dc18e6730d47f29cd0`  
		Last Modified: Tue, 19 Dec 2023 03:19:43 GMT  
		Size: 63.0 MB (62963274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d627909a3ff9de03889850fa5e83ecd71d896b3c313a14fb5c6e9915cc9b62e6`  
		Last Modified: Tue, 19 Dec 2023 03:21:51 GMT  
		Size: 189.7 MB (189684223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6066747268953e308928cdae02af6f43c9d8f732748f29a0b6c99a64669512aa`  
		Last Modified: Tue, 19 Dec 2023 19:14:48 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b70312acf3fc1945245d555f06df1ac5e42bf296974a6dac35f757ffe199f0`  
		Last Modified: Tue, 19 Dec 2023 19:17:43 GMT  
		Size: 14.9 MB (14919353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f1836e3526201bcb0580ccfb0c7865aabb433e1b872606a31ad3c393fb29218`  
		Last Modified: Tue, 19 Dec 2023 19:17:30 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded-bookworm` - linux; ppc64le

```console
$ docker pull perl@sha256:b18d5999aefeecb06e5e1c0d62a04498af7ba2708a452b11338e0f06f4db24c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **378.7 MB (378710893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbdcf77051611cfc122107ee96e04859715d4bad9f7a1ca6bfb700c73761b472`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Thu, 30 Nov 2023 02:54:02 GMT
ADD file:1728d055717ccd4f036c355a84deb6451942dd6e2c7998ee9d9d4edb3c02f7f4 in / 
# Thu, 30 Nov 2023 02:54:02 GMT
CMD ["bash"]
# Thu, 30 Nov 2023 02:54:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 30 Nov 2023 02:54:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 30 Nov 2023 02:54:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 30 Nov 2023 02:54:02 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 30 Nov 2023 02:54:02 GMT
WORKDIR /usr/src/perl
# Thu, 30 Nov 2023 02:54:02 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version # buildkit
# Thu, 30 Nov 2023 02:54:02 GMT
WORKDIR /usr/src/app
# Thu, 30 Nov 2023 02:54:02 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:b5382b02d02e48b7676d14a370941b889916302c0c0a4ce6eed6a87ddd65e5a3`  
		Last Modified: Tue, 19 Dec 2023 01:25:50 GMT  
		Size: 53.6 MB (53557744 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:53bef292d6dca0f2e01dadfb6697f50846fd2abe37345bd28c4b40d155bd3efb`  
		Last Modified: Tue, 19 Dec 2023 12:22:47 GMT  
		Size: 25.7 MB (25696155 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:397f3d69bf2380c69602528735990cbdbea6905ab14ff27daaf1ccd8e0599ad3`  
		Last Modified: Tue, 19 Dec 2023 12:23:09 GMT  
		Size: 69.6 MB (69582346 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bb645d1c095a31790b781022ac255437ab2c1a39357d5785bef239f25436d0d0`  
		Last Modified: Tue, 19 Dec 2023 12:23:51 GMT  
		Size: 214.1 MB (214135090 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a107e404797090f23f9a06cad030167ab4a78bcdf8174e8ca6f5708f4225823c`  
		Last Modified: Wed, 20 Dec 2023 21:32:16 GMT  
		Size: 135.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:66365a79e65c7d9e4276523d2b98c6e8c997e27f6c9ac2008616d8d473459f99`  
		Last Modified: Wed, 20 Dec 2023 21:59:10 GMT  
		Size: 15.7 MB (15739291 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:618310d7d518b0420f7ae0b60ee82eb798d3b689e2c84f14b7090109bd357c1b`  
		Last Modified: Wed, 20 Dec 2023 21:59:09 GMT  
		Size: 132.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `perl:threaded-bookworm` - unknown; unknown

```console
$ docker pull perl@sha256:7621f2d727e45af0847450c763293ce08579cbd0f10bc88028105e4102af9e4b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13402185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c50bbaa45392bebb344782b1afcab6e899d5feb3998954bf4177948575782ab2`

```dockerfile
```

-	Layers:
	-	`sha256:55947c8ff30e4495391d2f909681e5603dd39cf4f27b1abaef258bcaf7ba58ab`  
		Last Modified: Wed, 20 Dec 2023 21:59:09 GMT  
		Size: 13.4 MB (13384727 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:98aef31405ee97493ad46b4261538646c1416392ea72dc9e7fb4d63215e396fc`  
		Last Modified: Wed, 20 Dec 2023 21:59:09 GMT  
		Size: 17.5 KB (17458 bytes)  
		MIME: application/vnd.in-toto+json

### `perl:threaded-bookworm` - linux; s390x

```console
$ docker pull perl@sha256:60a882bf16c78eeb0f5ae59a4cbe86d17317da3396da6b154c0b2e07fed33983
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.2 MB (334244484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d031f5e602006c63aa901c88334423052423723db437900e44f96c1ee14bce3`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Thu, 30 Nov 2023 02:54:02 GMT
ADD file:5e36efc0891837fbd669c10cc5082f41b4ad22190feb2d516f4f0efd4890e772 in / 
# Thu, 30 Nov 2023 02:54:02 GMT
CMD ["bash"]
# Thu, 30 Nov 2023 02:54:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 30 Nov 2023 02:54:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 30 Nov 2023 02:54:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 30 Nov 2023 02:54:02 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 30 Nov 2023 02:54:02 GMT
WORKDIR /usr/src/perl
# Thu, 30 Nov 2023 02:54:02 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version # buildkit
# Thu, 30 Nov 2023 02:54:02 GMT
WORKDIR /usr/src/app
# Thu, 30 Nov 2023 02:54:02 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:9ba06e3db941501f326f297f1b24643ce2b142581fc9f396effcbc7c63df4938`  
		Last Modified: Tue, 19 Dec 2023 01:47:24 GMT  
		Size: 47.9 MB (47917679 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e564b911d9e033f9a67fcf5b0ddaad82153cceb2c4f54b63054a3c41bee756a1`  
		Last Modified: Tue, 19 Dec 2023 07:53:32 GMT  
		Size: 24.0 MB (24042818 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4ea66ebaf962eb06e4d585525f721841b7431908eb06730bf77ec7484806f571`  
		Last Modified: Tue, 19 Dec 2023 07:53:47 GMT  
		Size: 63.1 MB (63127874 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:01b9f68d79b5fc3c0f18f46ec4248ca8b98056a74979f1bae5166066dd9f500c`  
		Last Modified: Tue, 19 Dec 2023 07:54:16 GMT  
		Size: 183.1 MB (183128239 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1d1bf3c27b6914285692e056c03df5a1d9ddfa0685529fe661761fb1d8da51f3`  
		Last Modified: Wed, 20 Dec 2023 21:37:45 GMT  
		Size: 136.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b996777233fc39d9dd5189e49b69b270ffb2663eb1283885128056afc90ba1a9`  
		Last Modified: Wed, 20 Dec 2023 22:04:41 GMT  
		Size: 16.0 MB (16027606 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:af1bbdc0fa74138190f800e7a7f5be1a38225d17c35b28fcac1b84b62090b9d1`  
		Last Modified: Wed, 20 Dec 2023 22:04:40 GMT  
		Size: 132.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `perl:threaded-bookworm` - unknown; unknown

```console
$ docker pull perl@sha256:2638af181d937ad1eb39d43dd92bfca6065d3446823b3c3894401d82aeda4abc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.3 MB (13256815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:563064bc9c4d305c780a662e665e526c3975cf23f358adb9632f5fa38423536d`

```dockerfile
```

-	Layers:
	-	`sha256:f7e5f5c75785a5b3aa917e8fc4ada7b90f47db5dac8651cb7d966ce3d0cc9825`  
		Last Modified: Wed, 20 Dec 2023 22:04:41 GMT  
		Size: 13.2 MB (13239431 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:18b341e05cd5fc4c4f41cb356e5f7deb265e260d89d51cead005c6b78880a43e`  
		Last Modified: Wed, 20 Dec 2023 22:04:40 GMT  
		Size: 17.4 KB (17384 bytes)  
		MIME: application/vnd.in-toto+json
