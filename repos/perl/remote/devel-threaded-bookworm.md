## `perl:devel-threaded-bookworm`

```console
$ docker pull perl@sha256:a772f8920a14eea04bd6d5011e01f255edda1eae1966a5e302ce9e1baf3b4c13
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

### `perl:devel-threaded-bookworm` - linux; amd64

```console
$ docker pull perl@sha256:30ff53a1af2333f5ea06ff8c3bab5964804288723f63787bfdda4c161f1ef9d4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **364.7 MB (364708907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6599935f030f8e6836f6cd59a42ed04f3cdc1c238c3082e9900b2bd15669321c`
-	Default Command: `["perl5.39.4","-de0"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:37 GMT
ADD file:3e9b6405f11dd24ce62105c033f1d8b931d9409298553f63b03af1b6dd1dda35 in / 
# Wed, 01 Nov 2023 00:20:38 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:52:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 00:52:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 00:53:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 07:39:38 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 01 Nov 2023 07:39:38 GMT
WORKDIR /usr/src/perl
# Wed, 01 Nov 2023 11:17:29 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.4.tar.xz -o perl-5.39.4.tar.xz     && echo '73c5e1eb3f125206e82c23e2d03df2c62184d1acc330f99ab7624a3ade19b587 *perl-5.39.4.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.4.tar.xz -C /usr/src/perl     && rm perl-5.39.4.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Wed, 01 Nov 2023 11:17:29 GMT
WORKDIR /usr/src/app
# Wed, 01 Nov 2023 11:17:29 GMT
CMD ["perl5.39.4" "-de0"]
```

-	Layers:
	-	`sha256:8457fd5474e70835e4482983a5662355d892d5f6f0f90a27a8e9f009997e8196`  
		Last Modified: Wed, 01 Nov 2023 00:25:05 GMT  
		Size: 49.6 MB (49582024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13baa2029dde87a21b87127168a0fb50a007c07da6b5adc8864e1fe1376c86ff`  
		Last Modified: Wed, 01 Nov 2023 01:02:01 GMT  
		Size: 24.0 MB (24049147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:325c5bf4c2f26c11380501bec4b6eef8a3ea35b554aa1b222cbcd1e1fe11ae1d`  
		Last Modified: Wed, 01 Nov 2023 01:02:20 GMT  
		Size: 64.1 MB (64130415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e18a660069fd7f87a7a6c49ddb701449bfb929c066811777601d36916c7f674`  
		Last Modified: Wed, 01 Nov 2023 01:02:55 GMT  
		Size: 211.1 MB (211064253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58d8121bfec9ed3499669eb2e520f15a8f7b63c54641b87207c4d340ad778da`  
		Last Modified: Wed, 01 Nov 2023 11:38:27 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d3bef691c2c1638904b76afc26ff4603a474c56523536f0e4061b0d478084e7`  
		Last Modified: Wed, 01 Nov 2023 11:48:58 GMT  
		Size: 15.9 MB (15882736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d62871b3fba3ead1959e5f3f5f0051866590cdfd1ae2162ae0458c132cd7cc9`  
		Last Modified: Wed, 01 Nov 2023 11:48:55 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-threaded-bookworm` - linux; arm variant v5

```console
$ docker pull perl@sha256:28a4202a599c28a0a17e414d4e630f75ec698bee86a2f5cfc669f2af6fd5ba90
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.2 MB (331177587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6729a2cbcfaceaad9163c1e08c156420b0912054e93e923df04ae593318d85a`
-	Default Command: `["perl5.39.5","-de0"]`

```dockerfile
# Wed, 01 Nov 2023 00:48:23 GMT
ADD file:963e26decfc65419428098047df29dcbf7865e13bcdd67abeb9849f99a7815e7 in / 
# Wed, 01 Nov 2023 00:48:23 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:56:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 03:27:56 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 01 Nov 2023 03:27:56 GMT
WORKDIR /usr/src/perl
# Tue, 21 Nov 2023 04:18:41 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.5.tar.xz -o perl-5.39.5.tar.xz     && echo '4048cf0065f347a03ec85e989631a64e03ba9c9ccbc8f2a35153cad07fe21930 *perl-5.39.5.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.5.tar.xz -C /usr/src/perl     && rm perl-5.39.5.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 21 Nov 2023 04:18:42 GMT
WORKDIR /usr/src/app
# Tue, 21 Nov 2023 04:18:42 GMT
CMD ["perl5.39.5" "-de0"]
```

-	Layers:
	-	`sha256:53c5547a993a8adb09a632a8ae34fbc336b27a456c6b3a670865cd8bedb5e6a9`  
		Last Modified: Wed, 01 Nov 2023 00:51:04 GMT  
		Size: 47.4 MB (47355649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752979e12aac8f84972cea68e4f8d9bb1b645e71b3fc64047af1ba792dd338d9`  
		Last Modified: Wed, 01 Nov 2023 03:04:53 GMT  
		Size: 22.7 MB (22727584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bad2403917aecfddc5d239a343aacd942aeb9c9e6d76c027cfdbb0d5479bcaa`  
		Last Modified: Wed, 01 Nov 2023 03:05:15 GMT  
		Size: 61.6 MB (61561816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f0dda98bbf4b74a7919e20bcc31a0ecda8fd013c63ef827f0316369707e6af`  
		Last Modified: Wed, 01 Nov 2023 03:05:53 GMT  
		Size: 184.4 MB (184383946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0566f74e8226e4b0930481cd96a9fee1a8aa43842c56551e236bd176aa1dd12b`  
		Last Modified: Wed, 01 Nov 2023 06:31:53 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee8d87c6a96073f655545734f2e4a78b7bcf1382c9f74a90bd1b343df8c2d0c`  
		Last Modified: Tue, 21 Nov 2023 04:41:31 GMT  
		Size: 15.1 MB (15148259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b49dcc534b1b1b3ed53b9b291ba1103e46d3a7c91fda6d972dbe0c347210a66`  
		Last Modified: Tue, 21 Nov 2023 04:41:27 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-threaded-bookworm` - linux; arm variant v7

```console
$ docker pull perl@sha256:b9ba41fdda7da9119f1bfc14675d6081858e147ee941df86a6e3edc9c9b33adf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.4 MB (316375974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4ea8a9acfde609c37eb09a2b5c8c0b330e39c55e6be15182bc8c872d8809b7b`
-	Default Command: `["perl5.39.4","-de0"]`

```dockerfile
# Wed, 01 Nov 2023 00:57:42 GMT
ADD file:3b2b4eda35d794b39d6b5567e81651625af51da3deb3f63b3ffdffa07720646e in / 
# Wed, 01 Nov 2023 00:57:42 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:30:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:30:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:31:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 03:20:51 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 01 Nov 2023 03:20:51 GMT
WORKDIR /usr/src/perl
# Wed, 01 Nov 2023 07:03:08 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.4.tar.xz -o perl-5.39.4.tar.xz     && echo '73c5e1eb3f125206e82c23e2d03df2c62184d1acc330f99ab7624a3ade19b587 *perl-5.39.4.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.4.tar.xz -C /usr/src/perl     && rm perl-5.39.4.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Wed, 01 Nov 2023 07:03:08 GMT
WORKDIR /usr/src/app
# Wed, 01 Nov 2023 07:03:08 GMT
CMD ["perl5.39.4" "-de0"]
```

-	Layers:
	-	`sha256:9bf855396a6f46c1cbac4e188af10f2c38474f989707b0b1b406b48c4b7284ef`  
		Last Modified: Wed, 01 Nov 2023 01:01:41 GMT  
		Size: 45.2 MB (45179410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6e59eca644b227cb755978679a3031e7b3f9a5c707057c293f2ba8732d8ef2`  
		Last Modified: Wed, 01 Nov 2023 02:41:40 GMT  
		Size: 22.0 MB (21951880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aefa016475f9e4925fd893a9d8cfcf375937aa4e637d337806176426509dfcd`  
		Last Modified: Wed, 01 Nov 2023 02:42:04 GMT  
		Size: 59.3 MB (59266468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d2c477968e94d61a34b16e774d58519d5e26175f92fbd0dfb90938103fab68`  
		Last Modified: Wed, 01 Nov 2023 02:42:47 GMT  
		Size: 175.0 MB (175048871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a9bb425339c559e25bddb409850a9f7250167f2b44cf3977aa3bf8dafb18a4`  
		Last Modified: Wed, 01 Nov 2023 07:23:50 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9999c2116199a7e2c8f36e2ab843334755f81ac6fd15c8ee8a7c0fcfe6cecf`  
		Last Modified: Wed, 01 Nov 2023 07:35:04 GMT  
		Size: 14.9 MB (14929012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd32783771725722c2415b678061ad594c0d08b917442f39a0de8ef51109080`  
		Last Modified: Wed, 01 Nov 2023 07:35:00 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-threaded-bookworm` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:b5817260c8de0779239f2977ee277902b87add6e95e8af32a123661709790a3f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.5 MB (355475000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e8fd8e70050ff1bb7dbaecb2869a77f4d3bb7836336886196bff9a194caf891`
-	Default Command: `["perl5.39.5","-de0"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:32 GMT
ADD file:c934ceb4c53a1cce6779198f1ea73d5c8aad9a035e750b343d49826120ecd0eb in / 
# Wed, 01 Nov 2023 00:39:33 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:04:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:04:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:05:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 04:42:32 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 01 Nov 2023 04:42:32 GMT
WORKDIR /usr/src/perl
# Tue, 21 Nov 2023 04:37:08 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.5.tar.xz -o perl-5.39.5.tar.xz     && echo '4048cf0065f347a03ec85e989631a64e03ba9c9ccbc8f2a35153cad07fe21930 *perl-5.39.5.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.5.tar.xz -C /usr/src/perl     && rm perl-5.39.5.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 21 Nov 2023 04:37:08 GMT
WORKDIR /usr/src/app
# Tue, 21 Nov 2023 04:37:08 GMT
CMD ["perl5.39.5" "-de0"]
```

-	Layers:
	-	`sha256:8024d4fb53b2455f66d49b7ee72eb3cad5074043578238b796a9879955946a88`  
		Last Modified: Wed, 01 Nov 2023 00:42:44 GMT  
		Size: 49.6 MB (49612653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d826ee8aa65e56e167f0e27fa65cfc065687a7ac6c360787d5940d8b51f0cf1`  
		Last Modified: Wed, 01 Nov 2023 02:13:39 GMT  
		Size: 23.6 MB (23584896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198068495d09b6865e75ce28d5d5d5de39897b8325ada63ba80eca884ad5666b`  
		Last Modified: Wed, 01 Nov 2023 02:13:57 GMT  
		Size: 64.0 MB (63994018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509db9a897ae5a94cad05bcf48605637fbf3f79733e8bf8c317b6babe3de1dbd`  
		Last Modified: Wed, 01 Nov 2023 02:14:29 GMT  
		Size: 202.5 MB (202450117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb6a49d688d31488c983bb97e298e4eb59898d39edb1647aba4ea1664776705`  
		Last Modified: Wed, 01 Nov 2023 07:57:35 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9761cf5ee19085f40081d5c3613fa99bcd359e9e54a650331020b726713901`  
		Last Modified: Tue, 21 Nov 2023 04:55:36 GMT  
		Size: 15.8 MB (15832985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230e213dfdd86a003f6f7d5ae8a960cc79cd416ff547df308bb564d1f78b3b41`  
		Last Modified: Tue, 21 Nov 2023 04:55:34 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-threaded-bookworm` - linux; 386

```console
$ docker pull perl@sha256:0975703aabcb7b15abfe0284181cb12ebcc596e0784a43822d6c656f7fb32762
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **366.9 MB (366889524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3dbc9c7a95ec160a3582eff5185db2b961478d5eaea5b1d4c04d38268e6e019`
-	Default Command: `["perl5.39.4","-de0"]`

```dockerfile
# Wed, 01 Nov 2023 00:38:46 GMT
ADD file:4043d711d8d7d1a995aed0a6998c96230765f55d4449167107955fe4af2a31db in / 
# Wed, 01 Nov 2023 00:38:47 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:44:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:44:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:45:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 18:34:46 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 01 Nov 2023 18:34:46 GMT
WORKDIR /usr/src/perl
# Wed, 01 Nov 2023 21:46:03 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.4.tar.xz -o perl-5.39.4.tar.xz     && echo '73c5e1eb3f125206e82c23e2d03df2c62184d1acc330f99ab7624a3ade19b587 *perl-5.39.4.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.4.tar.xz -C /usr/src/perl     && rm perl-5.39.4.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Wed, 01 Nov 2023 21:46:04 GMT
WORKDIR /usr/src/app
# Wed, 01 Nov 2023 21:46:04 GMT
CMD ["perl5.39.4" "-de0"]
```

-	Layers:
	-	`sha256:be8d77e28ff21732ba73253b6226e47e4e07ec2cedc803ffd62148df5d7a165b`  
		Last Modified: Wed, 01 Nov 2023 00:43:00 GMT  
		Size: 50.6 MB (50600049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cef920c8d790c11b84fa21c2204cca8ac6a84ec43e4a60bca3670e828748583`  
		Last Modified: Wed, 01 Nov 2023 13:55:45 GMT  
		Size: 24.9 MB (24885575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fee1ec8688f07e43b49247f3490035da93288449034600daee26c8ce0150a8c`  
		Last Modified: Wed, 01 Nov 2023 13:56:13 GMT  
		Size: 66.0 MB (65984300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6a893690e210e75c1236dc74079509b9f860409954240df3b2276364c416f8`  
		Last Modified: Wed, 01 Nov 2023 13:57:04 GMT  
		Size: 210.0 MB (209994372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b744d82a612e7fa24d556f4310f785ca97501f0607492a213a6a49b59cdca67`  
		Last Modified: Wed, 01 Nov 2023 21:58:00 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72afb8b0ec6c696e4bace3a6bbd63bfa8f663304ef16eb45871f8dca78a6c76a`  
		Last Modified: Wed, 01 Nov 2023 22:04:02 GMT  
		Size: 15.4 MB (15424894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44a898b8dea5771bb67fb3f966f4cb39f340ee89340426baace3b6143cff6e60`  
		Last Modified: Wed, 01 Nov 2023 22:03:56 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-threaded-bookworm` - linux; mips64le

```console
$ docker pull perl@sha256:eb88fbf6a2616933873e762421741ce3bd108969623d03a3318a4c60cecf7470
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.7 MB (340722811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8255801f4c570aa9d6366c4f926475520dd8f91523ff316f40ab167bc0ea558`
-	Default Command: `["perl5.39.4","-de0"]`

```dockerfile
# Wed, 01 Nov 2023 01:08:17 GMT
ADD file:b181441dc28bc6879e29cd086c569c653171c681525c124ffb6277bd71732bb1 in / 
# Wed, 01 Nov 2023 01:08:24 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 21:17:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 21:19:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 21:25:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Nov 2023 11:36:08 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 02 Nov 2023 11:36:14 GMT
WORKDIR /usr/src/perl
# Thu, 02 Nov 2023 16:45:02 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.4.tar.xz -o perl-5.39.4.tar.xz     && echo '73c5e1eb3f125206e82c23e2d03df2c62184d1acc330f99ab7624a3ade19b587 *perl-5.39.4.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.4.tar.xz -C /usr/src/perl     && rm perl-5.39.4.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Thu, 02 Nov 2023 16:45:09 GMT
WORKDIR /usr/src/app
# Thu, 02 Nov 2023 16:45:15 GMT
CMD ["perl5.39.4" "-de0"]
```

-	Layers:
	-	`sha256:0bfbf01892d22dd14fb9536e8675cc932ff41f415a415fbf8c6199106b01240d`  
		Last Modified: Wed, 01 Nov 2023 01:19:01 GMT  
		Size: 49.6 MB (49568811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9310598b7549f388c445368ea2a0a4077c57ddd45436efddb37e089d293f87fe`  
		Last Modified: Wed, 01 Nov 2023 21:53:41 GMT  
		Size: 23.4 MB (23438019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af2206444fab218d319700cbfcd93423bf4622bb8085adee11b684b7d3fd245`  
		Last Modified: Wed, 01 Nov 2023 21:54:35 GMT  
		Size: 63.0 MB (62962363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41601926009dec498023c4d0a7e1c4877fc9fe8372d6497206d1de026aeb215d`  
		Last Modified: Wed, 01 Nov 2023 21:57:00 GMT  
		Size: 189.7 MB (189652978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4240f3e68e4e91fb1ba3cbb190fa1c3e58235f385c11bbe1fb46e1041fe67281`  
		Last Modified: Thu, 02 Nov 2023 17:11:38 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68bd40d2dc8d10670ee8ec7d4a9148f6197c7ae71ba1e4b851bf4b4652b29a48`  
		Last Modified: Thu, 02 Nov 2023 17:18:20 GMT  
		Size: 15.1 MB (15100375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ce2782555d2f4ced72080c0af32b40b16aff3d5bc41ece4f716803edf69457`  
		Last Modified: Thu, 02 Nov 2023 17:18:06 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-threaded-bookworm` - linux; ppc64le

```console
$ docker pull perl@sha256:f8cb2214c67912713f4edb06461dc8813c655bb0bf94d2f5dd48d871229aa087
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **378.9 MB (378878534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d5aae238cac550f9f1fddf4e3ad49492f8e83317c95dbc9d9dccf5ade6fb128`
-	Default Command: `["perl5.39.4","-de0"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:25 GMT
ADD file:31b995b44eb1f532fd265be3fc0c3d3b55e28db0911c86a06c83de621418db94 in / 
# Wed, 01 Nov 2023 00:21:28 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:24:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:24:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:27:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 07:27:02 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 01 Nov 2023 07:27:02 GMT
WORKDIR /usr/src/perl
# Wed, 01 Nov 2023 10:11:26 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.4.tar.xz -o perl-5.39.4.tar.xz     && echo '73c5e1eb3f125206e82c23e2d03df2c62184d1acc330f99ab7624a3ade19b587 *perl-5.39.4.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.4.tar.xz -C /usr/src/perl     && rm perl-5.39.4.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Wed, 01 Nov 2023 10:11:28 GMT
WORKDIR /usr/src/app
# Wed, 01 Nov 2023 10:11:28 GMT
CMD ["perl5.39.4" "-de0"]
```

-	Layers:
	-	`sha256:071872f8f8cb44e883168d06195f8fbb330e259b415d1ab108c27bda84d6c060`  
		Last Modified: Wed, 01 Nov 2023 00:25:41 GMT  
		Size: 53.6 MB (53575361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9986fe7e71120fd78fcaad86d3a1d827f54f56f266364834bcb7c13eccf9ca0`  
		Last Modified: Wed, 01 Nov 2023 01:40:25 GMT  
		Size: 25.7 MB (25698676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7316c6cea433a21258a8af8686d8a74e964c21c6c563afd63f274e9346f8f7`  
		Last Modified: Wed, 01 Nov 2023 01:40:48 GMT  
		Size: 69.6 MB (69584512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d43d4f467d09dbebbdbbe77e08bdef659a411541528d2d0542c5a201a1e3953`  
		Last Modified: Wed, 01 Nov 2023 01:41:31 GMT  
		Size: 214.1 MB (214093588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5e6ec90e3e03f24ea5d734c845115c59b6341cb6741bdf6120dfbc3ce41f0d9`  
		Last Modified: Wed, 01 Nov 2023 10:31:59 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2aff409e5fca9682c22a41b8fd60f504688f2518450be9b26357187cf40bc2`  
		Last Modified: Wed, 01 Nov 2023 10:40:12 GMT  
		Size: 15.9 MB (15926064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdf0f849ff4d089cd2ee8d321f9409e16eb7a5383d43817b66b0ae44a8816c4`  
		Last Modified: Wed, 01 Nov 2023 10:40:08 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-threaded-bookworm` - linux; s390x

```console
$ docker pull perl@sha256:1147801a4c3498487a74826aa327ad604c64ccbb9cf61390a3d92d16a06e9440
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.4 MB (334441428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c439167ae835ecc15980872f495a09113ed3170025d9551e3852bf07e3b6222c`
-	Default Command: `["perl5.39.5","-de0"]`

```dockerfile
# Wed, 01 Nov 2023 00:42:15 GMT
ADD file:6d8ee60b2fe4604969d8feeeb7e0dc8b9619a778d1a905c8bfdde5ede5e1eb54 in / 
# Wed, 01 Nov 2023 00:42:19 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:54:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:55:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:56:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 03:28:47 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 01 Nov 2023 03:28:47 GMT
WORKDIR /usr/src/perl
# Tue, 21 Nov 2023 04:17:18 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.5.tar.xz -o perl-5.39.5.tar.xz     && echo '4048cf0065f347a03ec85e989631a64e03ba9c9ccbc8f2a35153cad07fe21930 *perl-5.39.5.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.5.tar.xz -C /usr/src/perl     && rm perl-5.39.5.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 21 Nov 2023 04:17:20 GMT
WORKDIR /usr/src/app
# Tue, 21 Nov 2023 04:17:20 GMT
CMD ["perl5.39.5" "-de0"]
```

-	Layers:
	-	`sha256:bca95e393f709ba301b35c2439a815fd4fe8134d7a466bd528563bc32fd754d8`  
		Last Modified: Wed, 01 Nov 2023 00:47:43 GMT  
		Size: 47.9 MB (47943171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e744d1ef2c8405f6352136656080d7e244e1a97362c21069b734a55b86c8d0a`  
		Last Modified: Wed, 01 Nov 2023 02:05:09 GMT  
		Size: 24.0 MB (24045096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de40af46a5373d0a49892fa9000736be09090b477719517fcec84887d847f94b`  
		Last Modified: Wed, 01 Nov 2023 02:05:25 GMT  
		Size: 63.1 MB (63132485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5d582ecd4430347fbaa4df40283ca084e7bf9c17c0ce600484712c9f61dbe3`  
		Last Modified: Wed, 01 Nov 2023 02:05:57 GMT  
		Size: 183.1 MB (183099418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fe505f6b647555398944ec5b4aa4379aeb5eb1cc9f105cebf6fa1ce0dc827e6`  
		Last Modified: Wed, 01 Nov 2023 06:51:12 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9728447746d97c02244c3192ecedc72b87211a8778b590eee29a54bc2c9fd39a`  
		Last Modified: Tue, 21 Nov 2023 04:42:18 GMT  
		Size: 16.2 MB (16220925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f778963bc6f4d311a1b1dcdc867dac8a54cce9704165156296de8b82511baddb`  
		Last Modified: Tue, 21 Nov 2023 04:42:15 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
