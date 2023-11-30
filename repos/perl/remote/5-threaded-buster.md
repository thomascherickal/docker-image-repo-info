## `perl:5-threaded-buster`

```console
$ docker pull perl@sha256:894987dec71162fe75fb4e1a9280b429e2deb9c59070ac2359f6d914c9f25ccd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `perl:5-threaded-buster` - linux; amd64

```console
$ docker pull perl@sha256:c43e4edebbe52787af3f326a1fdb8f61c42488c8d12c45a97e9db877b5f7eb9e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.6 MB (327576470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d9ad7fd9b444c803ff7a62e0f4f52c2077bc13fc1397da07e9cd5781d8e5975`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Tue, 21 Nov 2023 05:22:08 GMT
ADD file:4f8b7a35280160ec5a55323fa07ac91e294c86e2ea647ba212053983ef380bcf in / 
# Tue, 21 Nov 2023 05:22:08 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:55:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 09:56:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 09:57:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 21:10:47 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 21 Nov 2023 21:10:47 GMT
WORKDIR /usr/src/perl
# Thu, 30 Nov 2023 20:13:17 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Thu, 30 Nov 2023 20:13:17 GMT
WORKDIR /usr/src/app
# Thu, 30 Nov 2023 20:13:17 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:b32028968d56a86ac35eac062e7abba276c547ab175fb057973c469eb41db55b`  
		Last Modified: Tue, 21 Nov 2023 05:26:57 GMT  
		Size: 50.5 MB (50499471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24c059838ae87ccefc35d50177e4e280a9e6f2f54127456ad0eaa5be5ed5386`  
		Last Modified: Tue, 21 Nov 2023 10:03:28 GMT  
		Size: 17.6 MB (17583860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:819458a39dea8d30616a22068e79bcb7743745aa8b0d35fdb762ba69d98e3ec0`  
		Last Modified: Tue, 21 Nov 2023 10:03:45 GMT  
		Size: 51.9 MB (51874180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eedd23d9034d9de62653c3bb2a2ca71fb88a1c6d17f386c0bfe4ac5bf8163929`  
		Last Modified: Tue, 21 Nov 2023 10:04:21 GMT  
		Size: 191.9 MB (191910019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9514a4efc131041c374381c502f31e8c18421d24cf16e185c4adef05f63c4415`  
		Last Modified: Tue, 21 Nov 2023 22:56:07 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4fbbc2f9de1f49452efbb8004da63edd4c806b9c4a69249147c00c587dc1679`  
		Last Modified: Thu, 30 Nov 2023 22:33:52 GMT  
		Size: 15.7 MB (15708606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50f9db0b63c22b11c616b8258fc29ca1a408de3da15cab2e341b9e590d27a6d`  
		Last Modified: Thu, 30 Nov 2023 22:33:50 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-threaded-buster` - linux; arm variant v7

```console
$ docker pull perl@sha256:4887271ddc379deb0ab892bcbfe32f3c1e373921c1718533fd0de6a3a51b8631
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.5 MB (292486335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:777030c25047e94b4b6b263bfee48522c09f8e6a9aa44e2b014c01bccd65f25f`
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
# Thu, 30 Nov 2023 19:47:23 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Thu, 30 Nov 2023 19:47:23 GMT
WORKDIR /usr/src/app
# Thu, 30 Nov 2023 19:47:23 GMT
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
	-	`sha256:3d4d6577ee75096f3c62be446bba2576119ee62c2adc207cd314f36fd70d3f82`  
		Last Modified: Thu, 30 Nov 2023 22:09:59 GMT  
		Size: 14.8 MB (14786433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcdff1dfa7f7cdb813074a75364692c4c3e0fd7db79150539d01cd739c12d861`  
		Last Modified: Thu, 30 Nov 2023 22:09:54 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-threaded-buster` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:7e20283c1c0be37e2e233e18d7ca5494172e486985ee1b951d25014851dafe0c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.0 MB (318047026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faddc1bc790d2ebf9ecec05357625091b6af2ff8acae150a061bfccff75049e6`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:27 GMT
ADD file:ea38b381ee92d0c4b34697af5b78def83b881e6837b309e1f41a14bee2ff2b7e in / 
# Tue, 21 Nov 2023 06:27:27 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:00:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 08:00:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 08:01:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 10:42:22 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 21 Nov 2023 10:42:22 GMT
WORKDIR /usr/src/perl
# Thu, 30 Nov 2023 20:24:31 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Thu, 30 Nov 2023 20:24:31 GMT
WORKDIR /usr/src/app
# Thu, 30 Nov 2023 20:24:32 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:357c576c57e480da5e7eb018506db51d822da9f357c02a76f7c4da1ccaa61b33`  
		Last Modified: Tue, 21 Nov 2023 06:31:24 GMT  
		Size: 49.3 MB (49291145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9750a1d4e9cc8d118fb8f247658f2e931026ab641d4ebdc3c3806b3dd8ee4d0d`  
		Last Modified: Tue, 21 Nov 2023 08:07:51 GMT  
		Size: 17.5 MB (17454097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55295586deeb07a4153f5f4d0cd2723a2240e52697d6ad85612c498057c0d832`  
		Last Modified: Tue, 21 Nov 2023 08:08:06 GMT  
		Size: 52.2 MB (52207152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fb9e461a1bbc28daea6d98c6425175d5ec238091b9c6d22306c3d257de50cd`  
		Last Modified: Tue, 21 Nov 2023 08:08:31 GMT  
		Size: 183.5 MB (183476090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d54341bf7f75e572bf0f6212e9a7fdcda4c60b7cb560eaf4b9705f40c5fecce`  
		Last Modified: Tue, 21 Nov 2023 13:50:02 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f274807cbfbd8b88a68507cf57c2f013e3df447544d0c7dfd51d0c9bc29f813d`  
		Last Modified: Thu, 30 Nov 2023 22:19:25 GMT  
		Size: 15.6 MB (15618210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6697219cf82912be8ad92a8dfbdc4f7b2886fb98bf21dc42617ecf56902ffecb`  
		Last Modified: Thu, 30 Nov 2023 22:19:23 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-threaded-buster` - linux; 386

```console
$ docker pull perl@sha256:9ae463ac3692daec02427f7f4667df7e362a5e8721e5f1fdd2feb48949ad6257
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.6 MB (336554103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73b1b4d931a7b460b283b0b40caad5f8e5bb8da5475d52cf7ef5f104eb68a856`
-	Default Command: `["perl5.38.0","-de0"]`

```dockerfile
# Tue, 21 Nov 2023 04:40:26 GMT
ADD file:3a91c3eed04829ed9d8801ae9da9d5dfb67139d59f8b98f87943131fc8953b49 in / 
# Tue, 21 Nov 2023 04:40:27 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 15:26:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 15:27:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 15:28:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 01:51:46 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 22 Nov 2023 01:51:46 GMT
WORKDIR /usr/src/perl
# Wed, 22 Nov 2023 02:34:16 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Wed, 22 Nov 2023 02:34:17 GMT
WORKDIR /usr/src/app
# Wed, 22 Nov 2023 02:34:17 GMT
CMD ["perl5.38.0" "-de0"]
```

-	Layers:
	-	`sha256:d9ff368d73b50f922dcf47b179053552ad7a9257e80ae0ef12ba15c8ca86eb6f`  
		Last Modified: Tue, 21 Nov 2023 04:45:46 GMT  
		Size: 51.3 MB (51256132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0ce00719c35aa0a641fc47343cf212a84a6290329a87ab71b902fa3c9b2bf0`  
		Last Modified: Tue, 21 Nov 2023 15:37:17 GMT  
		Size: 18.1 MB (18099384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785b20146c034209432ec7edd0514388edc0b27de9f7d44d10f1f7731bc37f73`  
		Last Modified: Tue, 21 Nov 2023 15:37:38 GMT  
		Size: 53.5 MB (53487793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7935218a8b05cf08fff65eaad84714f7d517167e5d68209bbd2111c8c2708c`  
		Last Modified: Tue, 21 Nov 2023 15:38:32 GMT  
		Size: 198.4 MB (198445334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f264f76a07d1452aabefdab44016d076d7d80653afe4f030c7c901d7c7e544f`  
		Last Modified: Wed, 22 Nov 2023 05:02:38 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb10168990572542944a78afb3eef0d9cd61701563850319f270e5f83d653472`  
		Last Modified: Wed, 22 Nov 2023 05:03:57 GMT  
		Size: 15.3 MB (15265129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb92762f1c051ee186278e6a6f6bc15d28bc38d66e944761e85f66e4e59fe649`  
		Last Modified: Wed, 22 Nov 2023 05:03:52 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
