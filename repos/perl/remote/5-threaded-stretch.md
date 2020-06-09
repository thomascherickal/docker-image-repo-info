## `perl:5-threaded-stretch`

```console
$ docker pull perl@sha256:41f72ceec541fb441bccf2e454a8aae93126da4150d9ca6b2fae863b97c9afd5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `perl:5-threaded-stretch` - linux; amd64

```console
$ docker pull perl@sha256:bbdffac79a7417415aefa605d1ddde05d15011a8a08045dad12dabfcd9287bd2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.4 MB (339374497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:468e14e3ca7e2034b5a0031bbd82924946317b75df2ada36f792e67310ef5fda`
-	Default Command: `["perl5.30.3","-de0"]`

```dockerfile
# Fri, 15 May 2020 06:33:25 GMT
ADD file:13031623172f5c5857e27de93553adedf17d955fa370882f850bb6ed6fb8cee7 in / 
# Fri, 15 May 2020 06:33:25 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:43:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:43:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 17:44:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:45:23 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 21:24:49 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Fri, 15 May 2020 21:24:50 GMT
COPY file:15650064fd29deac721f0aa084ddb3d41db77b78e2907775e257bd67e116ade4 in /usr/src/perl/ 
# Fri, 15 May 2020 21:24:50 GMT
WORKDIR /usr/src/perl
# Fri, 05 Jun 2020 21:43:44 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.30.3.tar.xz -o perl-5.30.3.tar.xz     && echo '6967595f2e3f3a94544c35152f9a25e0cb8ea24ae45f4bf1882f2e33f4a400f4 *perl-5.30.3.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.30.3.tar.xz -C /usr/src/perl     && rm perl-5.30.3.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Fri, 05 Jun 2020 21:43:44 GMT
WORKDIR /
# Fri, 05 Jun 2020 21:43:44 GMT
CMD ["perl5.30.3" "-de0"]
```

-	Layers:
	-	`sha256:1c6172af85ee14a8db5a3a51d406b768dfa94d196c06d0d06d591507cf8199f0`  
		Last Modified: Fri, 15 May 2020 06:40:31 GMT  
		Size: 45.4 MB (45375207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b194b0e3c928807cfabf081055a117585ba5bf6697f65b2fede02225a5d73ad2`  
		Last Modified: Fri, 15 May 2020 17:55:27 GMT  
		Size: 10.8 MB (10797475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5ec00f35d5b2d1db6b8e925a3005c1a285365775028db0339903ddaeec4763`  
		Last Modified: Fri, 15 May 2020 17:55:29 GMT  
		Size: 4.3 MB (4340139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b1353672b6861da5f1b58b0eca02ec10373a25d2898bddafa1b4bae2271c55`  
		Last Modified: Fri, 15 May 2020 17:55:45 GMT  
		Size: 50.1 MB (50084198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7f38db3cca2c74df9a146d8419f5bf79d79b18de9eaee6351dccde16ab1f4a`  
		Last Modified: Fri, 15 May 2020 17:59:23 GMT  
		Size: 214.9 MB (214908492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a81840f6f0c19b68cf1a88abe2ead3de425086f4a21bf39fc81390c276a68e01`  
		Last Modified: Sat, 16 May 2020 01:55:58 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387d4f1f52cb362fd74a100eba3449018521253e289c888359cef97c49ef1fe0`  
		Last Modified: Sat, 06 Jun 2020 01:11:04 GMT  
		Size: 13.9 MB (13868573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-threaded-stretch` - linux; arm variant v7

```console
$ docker pull perl@sha256:f691ec13bd21fb0ab18b86969f511a98b32c1580647edae8f8d35728882ead17
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.4 MB (310439608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c54970dca8f9a48e252d5be0d5eb5a573de7c8ae1d8cb40d529e41caf004827`
-	Default Command: `["perl5.30.3","-de0"]`

```dockerfile
# Tue, 09 Jun 2020 01:06:07 GMT
ADD file:c0b9ed1244ec0acfc9054c7cb80c768878e3da99740f981ba3a82bdd854305db in / 
# Tue, 09 Jun 2020 01:06:09 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:02:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:02:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:03:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:06:20 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 05:44:01 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 09 Jun 2020 05:44:02 GMT
COPY file:15650064fd29deac721f0aa084ddb3d41db77b78e2907775e257bd67e116ade4 in /usr/src/perl/ 
# Tue, 09 Jun 2020 05:44:02 GMT
WORKDIR /usr/src/perl
# Tue, 09 Jun 2020 06:33:57 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.30.3.tar.xz -o perl-5.30.3.tar.xz     && echo '6967595f2e3f3a94544c35152f9a25e0cb8ea24ae45f4bf1882f2e33f4a400f4 *perl-5.30.3.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.30.3.tar.xz -C /usr/src/perl     && rm perl-5.30.3.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 09 Jun 2020 06:33:59 GMT
WORKDIR /
# Tue, 09 Jun 2020 06:33:59 GMT
CMD ["perl5.30.3" "-de0"]
```

-	Layers:
	-	`sha256:2566ca784846d2d0d4f9105084d94d68d8ea1a82a06a76c5bcd991ce5a10cda1`  
		Last Modified: Tue, 09 Jun 2020 01:13:35 GMT  
		Size: 42.1 MB (42102504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f976b5a12722f5e6e115157695654d36452b713c7fa64a860f8c9e14859402`  
		Last Modified: Tue, 09 Jun 2020 02:15:15 GMT  
		Size: 9.4 MB (9443335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35142ef6ea6c722cd0397799ab151e5da354eabc784b3acef29def7fa34e9bc`  
		Last Modified: Tue, 09 Jun 2020 02:15:13 GMT  
		Size: 3.9 MB (3918433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7773eda6b7a8801a6f09bd4ce443b7e88397ed16265ecd37f55af57db56c4658`  
		Last Modified: Tue, 09 Jun 2020 02:15:36 GMT  
		Size: 46.4 MB (46412697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf8c80047f39ca1669cf85bbab477a59e35f498d269e058afe91bf9850b7c52`  
		Last Modified: Tue, 09 Jun 2020 02:16:37 GMT  
		Size: 195.6 MB (195567505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba37951465e9aaaf097edf994c1cdf5a6b82037c6b33c960c8b8abaf7ab82281`  
		Last Modified: Tue, 09 Jun 2020 09:32:05 GMT  
		Size: 440.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce5101635bd8f17c838c50da5ca9f3ca63aea0f18e057d3b2cb173687ef49cb`  
		Last Modified: Tue, 09 Jun 2020 09:33:31 GMT  
		Size: 13.0 MB (12994694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-threaded-stretch` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:6a16146b4094596ee1539520b5b2472fced9a4823cc273cbd7a0b1375ee2b76e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.0 MB (320952767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ff950283347499df984c517242fff60c2181aaaf23c072c4d0dc00ee9bacffc`
-	Default Command: `["perl5.30.3","-de0"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:22 GMT
ADD file:5cbf00485aed776e940988cadfad6853c640c13635ae54fb2b00aafccfe81a73 in / 
# Tue, 09 Jun 2020 01:54:25 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:39:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:39:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:40:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:43:35 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 04:35:58 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 09 Jun 2020 04:35:59 GMT
COPY file:15650064fd29deac721f0aa084ddb3d41db77b78e2907775e257bd67e116ade4 in /usr/src/perl/ 
# Tue, 09 Jun 2020 04:36:01 GMT
WORKDIR /usr/src/perl
# Tue, 09 Jun 2020 05:26:37 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.30.3.tar.xz -o perl-5.30.3.tar.xz     && echo '6967595f2e3f3a94544c35152f9a25e0cb8ea24ae45f4bf1882f2e33f4a400f4 *perl-5.30.3.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.30.3.tar.xz -C /usr/src/perl     && rm perl-5.30.3.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 09 Jun 2020 05:26:39 GMT
WORKDIR /
# Tue, 09 Jun 2020 05:26:41 GMT
CMD ["perl5.30.3" "-de0"]
```

-	Layers:
	-	`sha256:4c4f692ec920eecb1f30d9ef8e50125217decc872d7ada6eeccc36c6dcb49e4d`  
		Last Modified: Tue, 09 Jun 2020 02:00:09 GMT  
		Size: 43.2 MB (43160923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0990c417a21ef9e268cc0822cd23968c4b17cded8170cce0c4d8f7e020e6fd`  
		Last Modified: Tue, 09 Jun 2020 02:50:17 GMT  
		Size: 9.7 MB (9699635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6b83fd41426d182f67fdac882a6bfcd3aad22d7226a653ae58d3046bd46b5e`  
		Last Modified: Tue, 09 Jun 2020 02:50:15 GMT  
		Size: 4.1 MB (4094104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2de3ad924e80f0d130d0bd9ed8ea866eefeb610874bce14fd8347d032772220`  
		Last Modified: Tue, 09 Jun 2020 02:50:36 GMT  
		Size: 48.0 MB (48034909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2720149da5321de7d3e31500696a088aae1c37ededd1680245aec1602c17c5`  
		Last Modified: Tue, 09 Jun 2020 02:51:32 GMT  
		Size: 202.3 MB (202283682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:712cbf624a5810fd6c123651738b7a1815db91e171d1e605ce172d7e61797178`  
		Last Modified: Tue, 09 Jun 2020 08:29:21 GMT  
		Size: 444.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9490c6338b86e91881fbf03ba4765ce24533ce7a1e15803c80ac4c049da6cef`  
		Last Modified: Tue, 09 Jun 2020 08:30:33 GMT  
		Size: 13.7 MB (13679070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-threaded-stretch` - linux; 386

```console
$ docker pull perl@sha256:882205238f9fa91993e944570e0e9962a6dc312d0c244c952aa692da1130b85b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.5 MB (346455563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3a748a65b93bc62c86d834fadee54de28be44eccb261ec7be2398a295296d9f`
-	Default Command: `["perl5.30.3","-de0"]`

```dockerfile
# Fri, 15 May 2020 07:12:19 GMT
ADD file:22284e8c6e684308a95b18c7ed63ef235582dbb1890d1d02c22213e41ae47192 in / 
# Fri, 15 May 2020 07:12:19 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:22:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:22:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 17:22:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:23:46 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 18:37:31 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Fri, 15 May 2020 18:37:31 GMT
COPY file:15650064fd29deac721f0aa084ddb3d41db77b78e2907775e257bd67e116ade4 in /usr/src/perl/ 
# Fri, 15 May 2020 18:37:31 GMT
WORKDIR /usr/src/perl
# Fri, 05 Jun 2020 20:45:17 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.30.3.tar.xz -o perl-5.30.3.tar.xz     && echo '6967595f2e3f3a94544c35152f9a25e0cb8ea24ae45f4bf1882f2e33f4a400f4 *perl-5.30.3.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.30.3.tar.xz -C /usr/src/perl     && rm perl-5.30.3.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Fri, 05 Jun 2020 20:45:17 GMT
WORKDIR /
# Fri, 05 Jun 2020 20:45:17 GMT
CMD ["perl5.30.3" "-de0"]
```

-	Layers:
	-	`sha256:ddf311fc69760572da5334a35e5a0e9fa15690ee1e40ed4b06e9a65213bc7223`  
		Last Modified: Fri, 15 May 2020 07:22:51 GMT  
		Size: 46.1 MB (46094205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b241dd4b1f1a808fb80049baea941ffeb595af14983b6e48560fc4d07b66cf54`  
		Last Modified: Fri, 15 May 2020 17:32:39 GMT  
		Size: 10.8 MB (10818399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a58f9666641b58144531065f83cb2bf8ae4fc7968332d0563612de804752c0`  
		Last Modified: Fri, 15 May 2020 17:32:36 GMT  
		Size: 4.6 MB (4561476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a5af2e44b2e93a8556c765c57f7a929c2e24ace22880ce91c76ebbdee145d4`  
		Last Modified: Fri, 15 May 2020 17:33:00 GMT  
		Size: 51.6 MB (51616873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9ee0073c51896ac0b635d1ff96911a7f31d4cf9d23a619c534f4c73fc4b703`  
		Last Modified: Fri, 15 May 2020 17:33:58 GMT  
		Size: 220.0 MB (219962263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31304dbbdaa281f3926d100984580b368b0f246b915a80b681576f8cc74fb599`  
		Last Modified: Fri, 15 May 2020 23:06:20 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a39a2eabf1fe14d2b907b3300d93bbce16a707bc23040fc5684a0352cb0152d`  
		Last Modified: Sat, 06 Jun 2020 00:47:59 GMT  
		Size: 13.4 MB (13401932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-threaded-stretch` - linux; ppc64le

```console
$ docker pull perl@sha256:f849f084e26fea69b5200437b8f9238f6b6750d2873678e87a6a044b6a095272
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.3 MB (334304476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8fd7141820c8e8a4398d2f5d3f4cfd5a71965fc0ea0f48404fd26134fc3b96c`
-	Default Command: `["perl5.30.3","-de0"]`

```dockerfile
# Wed, 13 May 2020 22:39:29 GMT
ADD file:fa4c7e3ca04f092e53cc791a32c929663412df3f68de2733bb867053577bf1d1 in / 
# Wed, 13 May 2020 22:39:34 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:08:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 00:08:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 14 May 2020 00:10:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 00:22:48 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 05 Jun 2020 21:26:03 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Fri, 05 Jun 2020 21:26:06 GMT
COPY file:15650064fd29deac721f0aa084ddb3d41db77b78e2907775e257bd67e116ade4 in /usr/src/perl/ 
# Fri, 05 Jun 2020 21:26:07 GMT
WORKDIR /usr/src/perl
# Fri, 05 Jun 2020 22:12:42 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.30.3.tar.xz -o perl-5.30.3.tar.xz     && echo '6967595f2e3f3a94544c35152f9a25e0cb8ea24ae45f4bf1882f2e33f4a400f4 *perl-5.30.3.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.30.3.tar.xz -C /usr/src/perl     && rm perl-5.30.3.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Fri, 05 Jun 2020 22:12:48 GMT
WORKDIR /
# Fri, 05 Jun 2020 22:12:49 GMT
CMD ["perl5.30.3" "-de0"]
```

-	Layers:
	-	`sha256:7732483b686efe14a1cf8add89a1568b83892e243798fba30808f1fc6287210b`  
		Last Modified: Wed, 13 May 2020 23:02:10 GMT  
		Size: 45.6 MB (45646193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df33ef5c6dd4781defd528815174987b67a617a4fbddd5e5241a2f67a34098cb`  
		Last Modified: Thu, 14 May 2020 00:37:47 GMT  
		Size: 10.0 MB (10002565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02507bd450f72bbb529f56f9579bb7169fc9be7900bc5b9b0587e4855e51ad8d`  
		Last Modified: Thu, 14 May 2020 00:37:41 GMT  
		Size: 4.3 MB (4296673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a5abe5a03ebb35ed027af57237427bf1650677f1d4c6a907f88cf889b5e403`  
		Last Modified: Thu, 14 May 2020 00:39:16 GMT  
		Size: 50.1 MB (50081278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e26879e4c99689db7dde317c0cef4c2586bcab4f29e2ca00e86e28101d2d88`  
		Last Modified: Thu, 14 May 2020 00:42:00 GMT  
		Size: 210.5 MB (210531113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea5c7bfee4d800e0d3257972895829da453872963450c966c775bda0ed8d263b`  
		Last Modified: Sat, 06 Jun 2020 00:37:14 GMT  
		Size: 441.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f07211ceff9be454bcf3ff2e1f2334996b6f7f6c8b21a13b6d540a21ea60c988`  
		Last Modified: Sat, 06 Jun 2020 00:38:58 GMT  
		Size: 13.7 MB (13746213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-threaded-stretch` - linux; s390x

```console
$ docker pull perl@sha256:25fe71b73a3db1a0732c891143feff2c56a7547ffcb269c851cf6ff4d1a46d07
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.6 MB (331621263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07d40b4054d3589a1ac4c97ecf84a72c54f7a309a164bff6c724e6ea571de786`
-	Default Command: `["perl5.30.3","-de0"]`

```dockerfile
# Tue, 09 Jun 2020 01:44:05 GMT
ADD file:ce4b8c76522cbe8599502985424901aee9d30d37296761d47dbcb9b0770f7aa2 in / 
# Tue, 09 Jun 2020 01:44:08 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:13:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:13:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:13:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:15:38 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 03:55:12 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 09 Jun 2020 03:55:12 GMT
COPY file:15650064fd29deac721f0aa084ddb3d41db77b78e2907775e257bd67e116ade4 in /usr/src/perl/ 
# Tue, 09 Jun 2020 03:55:12 GMT
WORKDIR /usr/src/perl
# Tue, 09 Jun 2020 04:19:51 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.30.3.tar.xz -o perl-5.30.3.tar.xz     && echo '6967595f2e3f3a94544c35152f9a25e0cb8ea24ae45f4bf1882f2e33f4a400f4 *perl-5.30.3.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.30.3.tar.xz -C /usr/src/perl     && rm perl-5.30.3.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 09 Jun 2020 04:19:53 GMT
WORKDIR /
# Tue, 09 Jun 2020 04:19:53 GMT
CMD ["perl5.30.3" "-de0"]
```

-	Layers:
	-	`sha256:cc8faf537ff83acc994f80bcea99d8e073aa05b5eb0dab5ce495510af0b6d1f6`  
		Last Modified: Tue, 09 Jun 2020 01:47:50 GMT  
		Size: 45.2 MB (45232505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9816eeae17f469b3b58481bdbae04cc1b7b69f8d8a6ef15f6972d91ba2f29ee8`  
		Last Modified: Tue, 09 Jun 2020 02:19:43 GMT  
		Size: 10.3 MB (10280522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a7344ca59dab92a8238f2df0ea3779840ec21afc295e24f39259558c3bfc05`  
		Last Modified: Tue, 09 Jun 2020 02:19:48 GMT  
		Size: 4.4 MB (4372414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a9332093631759dcfd58267f270de204b0c9388802581c972141e78700c0bb`  
		Last Modified: Tue, 09 Jun 2020 02:20:00 GMT  
		Size: 50.5 MB (50510977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6abb293160bb369db1a3815bce0f615b6d0d75a3a6f4152e6d68933bfa3653ee`  
		Last Modified: Tue, 09 Jun 2020 02:20:29 GMT  
		Size: 206.9 MB (206928247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b76dc7239124974cc0b25f3df650730be8ca9e8da5d1681f2e6088c616022d8`  
		Last Modified: Tue, 09 Jun 2020 05:47:27 GMT  
		Size: 437.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75531d48140fe8284d2006c3c3d0cd058b86020a0b540045fe283f811c554b8a`  
		Last Modified: Tue, 09 Jun 2020 05:48:17 GMT  
		Size: 14.3 MB (14296161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
