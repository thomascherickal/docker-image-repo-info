## `perl:threaded-bullseye`

```console
$ docker pull perl@sha256:b3f364824645be65c401c8f5c7750a3d2ff3c2667ae72bd65c061013f5712ec6
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

### `perl:threaded-bullseye` - linux; amd64

```console
$ docker pull perl@sha256:32bdecad03e56bbf43256bae3fa3dc57f5130e651dcaa2f58a618e53e873f0a3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.4 MB (336369875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:369b6bd6b7f13ce04ec4c1e55127f9e4e75f13cfaab2de283fde135fa935416e`
-	Default Command: `["perl5.34.0","-de0"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:07 GMT
ADD file:e777355768c63f735e5458c7e0ada7f556f27d0493b3af35dc7c34f9c4294ea9 in / 
# Thu, 02 Dec 2021 02:48:08 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:39:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:39:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 03:40:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:41:21 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 19:12:07 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 02 Dec 2021 19:12:07 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Thu, 02 Dec 2021 19:12:07 GMT
WORKDIR /usr/src/perl
# Thu, 02 Dec 2021 19:58:08 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.0.tar.xz -o perl-5.34.0.tar.xz     && echo '82c2e5e5c71b0e10487a80d79140469ab1f8056349ca8545140a224dbbed7ded *perl-5.34.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.0.tar.xz -C /usr/src/perl     && rm perl-5.34.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Thu, 02 Dec 2021 19:58:08 GMT
WORKDIR /
# Thu, 02 Dec 2021 19:58:08 GMT
CMD ["perl5.34.0" "-de0"]
```

-	Layers:
	-	`sha256:5e0b432e8ba9d9029a000e627840b98ffc1ed0c5172075b7d3e869be0df0fe9b`  
		Last Modified: Thu, 02 Dec 2021 02:53:18 GMT  
		Size: 54.9 MB (54932878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84cfd68b5cea612a8343c346bfa5bd6c486769010d12f7ec86b23c74887feb2`  
		Last Modified: Thu, 02 Dec 2021 03:49:22 GMT  
		Size: 5.2 MB (5153424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b8f2315954535f1e27cd13d777e73da4a787b0aebf4241d225beff3c91cbb1`  
		Last Modified: Thu, 02 Dec 2021 03:49:23 GMT  
		Size: 10.9 MB (10871995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0598fa43a7e793a76c198e8d45d8810394e1cfc943b2673d7fcf5a6fdc4f45b3`  
		Last Modified: Thu, 02 Dec 2021 03:49:46 GMT  
		Size: 54.6 MB (54567844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83098237b6d3febc7584c1f16076a32ac01def85b0d220ab46b6ebb2d6e7d4d4`  
		Last Modified: Thu, 02 Dec 2021 03:50:31 GMT  
		Size: 196.5 MB (196499409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46cd601fd47f014010b51abc8db1bc2f01b14d31602d6efa3f02e051ee00f041`  
		Last Modified: Thu, 02 Dec 2021 23:11:30 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b78e151d3c2495887650a4eda5e6ebeadebddd1f67c724d2c6643b35b9bf01`  
		Last Modified: Thu, 02 Dec 2021 23:13:11 GMT  
		Size: 14.3 MB (14344124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded-bullseye` - linux; arm variant v5

```console
$ docker pull perl@sha256:853d2f8743bc4dfcbf133d180480ba022586b2411adf420407455487649dc492
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.7 MB (308738338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58fb37823b077de9e4a48eb9b278a73ae398f1847fdbe6a24ec0fc7a11cfbbf4`
-	Default Command: `["perl5.34.0","-de0"]`

```dockerfile
# Thu, 02 Dec 2021 02:49:59 GMT
ADD file:7db27b7237be13d28b7ac71f50b332fc30b9988ea3b9a25dbf567e66ae9f3733 in / 
# Thu, 02 Dec 2021 02:50:00 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:34:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:35:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 03:36:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:39:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 19:47:45 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 02 Dec 2021 19:47:46 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Thu, 02 Dec 2021 19:47:46 GMT
WORKDIR /usr/src/perl
# Thu, 02 Dec 2021 20:51:48 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.0.tar.xz -o perl-5.34.0.tar.xz     && echo '82c2e5e5c71b0e10487a80d79140469ab1f8056349ca8545140a224dbbed7ded *perl-5.34.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.0.tar.xz -C /usr/src/perl     && rm perl-5.34.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Thu, 02 Dec 2021 20:51:49 GMT
WORKDIR /
# Thu, 02 Dec 2021 20:51:49 GMT
CMD ["perl5.34.0" "-de0"]
```

-	Layers:
	-	`sha256:7243911d8825e14c0a343985557fbeb75da8a3a059c3f67c83036cc217dac188`  
		Last Modified: Thu, 02 Dec 2021 03:08:41 GMT  
		Size: 52.5 MB (52467922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f91846e63508bbda03b74c487feabb599525b1c20c5b0e35d3ecb68b0791963`  
		Last Modified: Thu, 02 Dec 2021 04:00:12 GMT  
		Size: 5.1 MB (5063907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d446dad57642eb79a9cc56005f2d0bd04022a419a03076ed09503002b5f18f0`  
		Last Modified: Thu, 02 Dec 2021 04:00:13 GMT  
		Size: 10.6 MB (10571199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01c3e4ea3de2890a431db84174f2d19f5b0137f1d3ffa29e4afb1b24ca6404a`  
		Last Modified: Thu, 02 Dec 2021 04:00:51 GMT  
		Size: 52.3 MB (52323416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39fb04fcc8d78b399199145fc2f6a54663a334c390312b719f2aa7ee7a77968b`  
		Last Modified: Thu, 02 Dec 2021 04:02:07 GMT  
		Size: 174.7 MB (174690783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfcd44ce0c8fb5488329b13b591f32916bfc652aab1371c6791546b0483b4651`  
		Last Modified: Fri, 03 Dec 2021 00:59:36 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38af9120b2d4ed3d54ede72d5c190726a889b5e065d8b739f3316e1708c93ed`  
		Last Modified: Fri, 03 Dec 2021 01:02:29 GMT  
		Size: 13.6 MB (13620908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded-bullseye` - linux; arm variant v7

```console
$ docker pull perl@sha256:d8caf74932c772f4d093ab064e5d6bfb0b207c472483e6bc55b8b1c20b5ae386
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.0 MB (295975018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cddfa719c44c6e2b18467a52d1f2a2bbff1d930e1f05a007695445fd71f2bd97`
-	Default Command: `["perl5.34.0","-de0"]`

```dockerfile
# Thu, 02 Dec 2021 09:04:39 GMT
ADD file:f0d0256a657fcc82cba38ec9fe377ae4d30125de11e0003de81177370592b440 in / 
# Thu, 02 Dec 2021 09:04:40 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 11:38:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 11:38:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 11:39:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 11:41:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 18:30:52 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 02 Dec 2021 18:30:52 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Thu, 02 Dec 2021 18:30:53 GMT
WORKDIR /usr/src/perl
# Thu, 02 Dec 2021 19:30:20 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.0.tar.xz -o perl-5.34.0.tar.xz     && echo '82c2e5e5c71b0e10487a80d79140469ab1f8056349ca8545140a224dbbed7ded *perl-5.34.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.0.tar.xz -C /usr/src/perl     && rm perl-5.34.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Thu, 02 Dec 2021 19:30:21 GMT
WORKDIR /
# Thu, 02 Dec 2021 19:30:21 GMT
CMD ["perl5.34.0" "-de0"]
```

-	Layers:
	-	`sha256:e704987a22630df63d8518dd22b13ec2a4f460fd492ab42b97cdc6f971e7be31`  
		Last Modified: Thu, 02 Dec 2021 09:20:17 GMT  
		Size: 50.1 MB (50134315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfec4d15f2394da70fac9265e0e06909f3fc78eb919976d21b07ba0ba5214dba`  
		Last Modified: Thu, 02 Dec 2021 12:00:15 GMT  
		Size: 4.9 MB (4922713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5168f89db31fd7437013ced429c3e2fb7ef1d0e51dbd25bc65fdfde5ab4d5ca1`  
		Last Modified: Thu, 02 Dec 2021 12:00:17 GMT  
		Size: 10.2 MB (10216972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3a2d12df86190bd722a8220fd21e6b8978e175668c93e7678e898b6d6100e76`  
		Last Modified: Thu, 02 Dec 2021 12:01:06 GMT  
		Size: 50.3 MB (50327911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d64bd9959a5340020622e8677af3b688bbdc7e8184c4cf7f4eed670db88b4e9`  
		Last Modified: Thu, 02 Dec 2021 12:02:53 GMT  
		Size: 166.9 MB (166945379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ecad6e29437539b4ed91fcada4934f81770d63bd7a2bd7588ba56136bb28482`  
		Last Modified: Thu, 02 Dec 2021 23:21:41 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b44210e75e61db9cd6305da4eec22ba822528aaa7260f85a98f1af8a495e5a5`  
		Last Modified: Thu, 02 Dec 2021 23:24:36 GMT  
		Size: 13.4 MB (13427526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded-bullseye` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:449dc3ffb4211ea5864999f5af9af98b92feb56001df46b51e8ac5bd16531122
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.5 MB (327539938 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cb7e14c9faeb4b6122f3b0d56e20a781a537a4861596a213e2df1ed8c9a0315`
-	Default Command: `["perl5.34.0","-de0"]`

```dockerfile
# Thu, 02 Dec 2021 08:07:54 GMT
ADD file:998dc1c35eeeed1ddf46156aeb337fb9b8cbb4855caf994201167a1061f4ecbf in / 
# Thu, 02 Dec 2021 08:07:55 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 09:53:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 09:53:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 09:53:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 09:54:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 21:27:37 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 02 Dec 2021 21:27:38 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Thu, 02 Dec 2021 21:27:39 GMT
WORKDIR /usr/src/perl
# Thu, 02 Dec 2021 21:48:18 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.0.tar.xz -o perl-5.34.0.tar.xz     && echo '82c2e5e5c71b0e10487a80d79140469ab1f8056349ca8545140a224dbbed7ded *perl-5.34.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.0.tar.xz -C /usr/src/perl     && rm perl-5.34.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Thu, 02 Dec 2021 21:48:19 GMT
WORKDIR /
# Thu, 02 Dec 2021 21:48:20 GMT
CMD ["perl5.34.0" "-de0"]
```

-	Layers:
	-	`sha256:6476cb406b24c94f24348db05d154b814b14ee38860dea1625080e7e08295a80`  
		Last Modified: Thu, 02 Dec 2021 08:40:14 GMT  
		Size: 53.6 MB (53619027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96565d527970b1cc982493f96d6b317b1fbfdd7bf0ea6fd58d44942bb4f597c5`  
		Last Modified: Thu, 02 Dec 2021 10:02:24 GMT  
		Size: 4.9 MB (4937631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8c15f93136056df893ba8088992a38e90dc37210fd6ebb712413fd045c58de`  
		Last Modified: Thu, 02 Dec 2021 10:02:25 GMT  
		Size: 10.7 MB (10655914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee42e24e52cb2f9b50ab14328865298f5ae6ac159219db890afc6366ec641a46`  
		Last Modified: Thu, 02 Dec 2021 10:02:46 GMT  
		Size: 54.7 MB (54669690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac9532df0bb004dc05861cf06b71118340d756f7ce167e8394e1fd1137b0002`  
		Last Modified: Thu, 02 Dec 2021 10:03:24 GMT  
		Size: 189.4 MB (189384630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f8098fa93952bf1659cbb89101f55e8eb31e72f19b1b1a2d55736a07574aebc`  
		Last Modified: Thu, 02 Dec 2021 23:11:40 GMT  
		Size: 179.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b1f5d7d4c7d58b8111b072b74219b5cdd465b0942079d7dc1bac9b571a3e5a4`  
		Last Modified: Thu, 02 Dec 2021 23:13:27 GMT  
		Size: 14.3 MB (14272867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded-bullseye` - linux; 386

```console
$ docker pull perl@sha256:20f6e6d9cae5a99e01d800a36632362469d0e65187bfa2ec226ccd6d4f233933
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **341.7 MB (341662734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2693add2c721b4194f15ecc38e783fb2166b4a0bf822b73daac497cd3a2eb38`
-	Default Command: `["perl5.34.0","-de0"]`

```dockerfile
# Thu, 02 Dec 2021 02:39:37 GMT
ADD file:0fd00a1dc1745744d1e95964f1f6fc73e016055aeec062f1946440b6ba68411d in / 
# Thu, 02 Dec 2021 02:39:37 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:10:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:10:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 03:11:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:12:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 09:59:01 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 02 Dec 2021 09:59:01 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Thu, 02 Dec 2021 09:59:01 GMT
WORKDIR /usr/src/perl
# Thu, 02 Dec 2021 10:44:00 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.0.tar.xz -o perl-5.34.0.tar.xz     && echo '82c2e5e5c71b0e10487a80d79140469ab1f8056349ca8545140a224dbbed7ded *perl-5.34.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.0.tar.xz -C /usr/src/perl     && rm perl-5.34.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Thu, 02 Dec 2021 10:44:01 GMT
WORKDIR /
# Thu, 02 Dec 2021 10:44:01 GMT
CMD ["perl5.34.0" "-de0"]
```

-	Layers:
	-	`sha256:3dfa4acb9eec45f56cd836373cf9bf145fb45d1ae4cbc3181c21d4d01d14037d`  
		Last Modified: Thu, 02 Dec 2021 02:47:22 GMT  
		Size: 55.9 MB (55937571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3245a08f8d7007d55bcf225301e2ba4bcbd38d83c944f9a0fe4ca5811ac6bf9f`  
		Last Modified: Thu, 02 Dec 2021 03:20:35 GMT  
		Size: 5.3 MB (5283147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff3b7dd8fe63a0512b577941dbb20701dc02abfdca700e55006d84c44cfc0e1`  
		Last Modified: Thu, 02 Dec 2021 03:20:35 GMT  
		Size: 11.3 MB (11250671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:394078f1578cde892a871c190a95f65490ec769aa2c7aadf9d224b49f50f1a35`  
		Last Modified: Thu, 02 Dec 2021 03:21:05 GMT  
		Size: 55.9 MB (55917753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3da24b680b80bb8e49e7a6655ea0c6a18d872049c9addcb70c96f44bb69190c`  
		Last Modified: Thu, 02 Dec 2021 03:21:57 GMT  
		Size: 199.4 MB (199412590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e404fe4375a46f7de9c84a660e0568fd754beff00f2ac0568509c1d5c1a513b2`  
		Last Modified: Thu, 02 Dec 2021 14:18:48 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9c30961a2c3acf29e5c111f82ba60fd2722aed23a3c04387ed182e24b99376b`  
		Last Modified: Thu, 02 Dec 2021 14:21:14 GMT  
		Size: 13.9 MB (13860800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded-bullseye` - linux; mips64le

```console
$ docker pull perl@sha256:54ed3844edefb958f2467e28ce8dcc75607883dc19ab2f483d96e39cb6c5b776
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.7 MB (314699561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a714a88bd082a77c90051054fc5c47eaa8c33bd95d07d13d1205dbe8f63f1db`
-	Default Command: `["perl5.34.0","-de0"]`

```dockerfile
# Thu, 02 Dec 2021 03:08:44 GMT
ADD file:40dd380a63b1628d2ba96873bcf6a035d95f158325e90ad46ed46a6866f06c36 in / 
# Thu, 02 Dec 2021 03:08:45 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 04:09:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 04:10:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 04:11:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 04:14:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 04:15:12 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Fri, 03 Dec 2021 04:15:13 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Fri, 03 Dec 2021 04:15:13 GMT
WORKDIR /usr/src/perl
# Fri, 03 Dec 2021 05:52:11 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.0.tar.xz -o perl-5.34.0.tar.xz     && echo '82c2e5e5c71b0e10487a80d79140469ab1f8056349ca8545140a224dbbed7ded *perl-5.34.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.0.tar.xz -C /usr/src/perl     && rm perl-5.34.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Fri, 03 Dec 2021 05:52:11 GMT
WORKDIR /
# Fri, 03 Dec 2021 05:52:12 GMT
CMD ["perl5.34.0" "-de0"]
```

-	Layers:
	-	`sha256:0ddc107271364d08a7f7838aeeb4e5f1381785e292f448280a494b1e02dc4e1d`  
		Last Modified: Thu, 02 Dec 2021 03:17:13 GMT  
		Size: 53.2 MB (53183833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a316e34103c19d4dfaa32faac9aa612895a883b0b9ee9512437d61491e352a`  
		Last Modified: Thu, 02 Dec 2021 04:25:09 GMT  
		Size: 5.1 MB (5114991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581dfe9196165133ea6c0f84d927fcd80ddb219aadb032ae7e581cd0c8ff4c15`  
		Last Modified: Thu, 02 Dec 2021 04:25:12 GMT  
		Size: 10.9 MB (10873302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45f96d0b57eaaab4f2cadb251810c0fc66f400bc38f157386a5acaf3f22c9c4`  
		Last Modified: Thu, 02 Dec 2021 04:26:03 GMT  
		Size: 53.3 MB (53296541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d424348959b333b959194b5970da75eeb868bca9d31a1860f2e05905a57ba77c`  
		Last Modified: Thu, 02 Dec 2021 04:28:12 GMT  
		Size: 178.6 MB (178614868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:343947f4391f5a1e6b02cb658ae8093a13b0418f68bede1d057fb67666195978`  
		Last Modified: Fri, 03 Dec 2021 12:05:50 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baa33b2e711fc8f8e170485687ee25b7aa0ddb5749b4d62852a3a8a23227b118`  
		Last Modified: Fri, 03 Dec 2021 12:08:24 GMT  
		Size: 13.6 MB (13615850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded-bullseye` - linux; ppc64le

```console
$ docker pull perl@sha256:7d0178be2d498ae33a73ae871be5440c78f7cae64f183281056f1d5a953ba974
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.9 MB (344932649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a253d3a0bac7ab0e00efc7ace2d79ee1d6a39b4c914512a3168b4a7f2fa2c7e`
-	Default Command: `["perl5.34.0","-de0"]`

```dockerfile
# Thu, 02 Dec 2021 07:20:49 GMT
ADD file:781003f73ff5fb7313d2bd58dc99ae83adc49c419929d32a63c29a9d45b5a554 in / 
# Thu, 02 Dec 2021 07:20:54 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 12:05:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 12:06:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 12:08:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 12:18:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 22:01:32 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 02 Dec 2021 22:01:34 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Thu, 02 Dec 2021 22:01:35 GMT
WORKDIR /usr/src/perl
# Thu, 02 Dec 2021 22:42:09 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.0.tar.xz -o perl-5.34.0.tar.xz     && echo '82c2e5e5c71b0e10487a80d79140469ab1f8056349ca8545140a224dbbed7ded *perl-5.34.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.0.tar.xz -C /usr/src/perl     && rm perl-5.34.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Thu, 02 Dec 2021 22:42:11 GMT
WORKDIR /
# Thu, 02 Dec 2021 22:42:14 GMT
CMD ["perl5.34.0" "-de0"]
```

-	Layers:
	-	`sha256:6ae53eb717439cac2dd934aaff8829ad7eadd86024d1ea6efc5bcd9ad4291200`  
		Last Modified: Thu, 02 Dec 2021 07:31:08 GMT  
		Size: 58.8 MB (58819590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fac4014676b1c485dd93f21955848a174e2d21b407aa34ffef66c57f1322051`  
		Last Modified: Thu, 02 Dec 2021 12:54:45 GMT  
		Size: 5.4 MB (5402059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8244759ab55b45af369ca2cf554b0c1302663446bb7781aeb3b8dda967f75dcc`  
		Last Modified: Thu, 02 Dec 2021 12:54:46 GMT  
		Size: 11.6 MB (11626130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b784ac8d3e562c2d41fcab748557f1be3e0b77ebfafcb308f9f8cb79d966bb3e`  
		Last Modified: Thu, 02 Dec 2021 12:55:13 GMT  
		Size: 58.9 MB (58851432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:139235cf9b5e27744b11351cd34c96a2aa31fe6c93aaa3c3dca9e7f9a0edbfcf`  
		Last Modified: Thu, 02 Dec 2021 12:56:03 GMT  
		Size: 195.9 MB (195854133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1282fa112ca6fa068f68f1d30697fd7ef559c9890d94b73f94303fe390be68c0`  
		Last Modified: Fri, 03 Dec 2021 01:17:16 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c43a52ae7bd5cc9f71ea0b5fea05a2b37717bcfc94dfaac7f95c5b1d525f2fc`  
		Last Modified: Fri, 03 Dec 2021 01:19:15 GMT  
		Size: 14.4 MB (14379102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:threaded-bullseye` - linux; s390x

```console
$ docker pull perl@sha256:58c54f15773c03ba68c0a8babfef7055355afc7e7a7d137b94e662e58aca3bd3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.3 MB (310348586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71da573e8c691652aa9d2aca456b8c20c2613e36ba8af6573efc438bbd402352`
-	Default Command: `["perl5.34.0","-de0"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:08 GMT
ADD file:9bd51bb5b152533abeecc5a52ab1ef27b6fe2b3be150073d286b50d9c422cfb9 in / 
# Tue, 21 Dec 2021 01:42:11 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:08:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:08:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:09:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:10:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 03:39:41 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 21 Dec 2021 03:39:41 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 21 Dec 2021 03:39:42 GMT
WORKDIR /usr/src/perl
# Tue, 21 Dec 2021 04:03:28 GMT
RUN true     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.0.tar.xz -o perl-5.34.0.tar.xz     && echo '82c2e5e5c71b0e10487a80d79140469ab1f8056349ca8545140a224dbbed7ded *perl-5.34.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.0.tar.xz -C /usr/src/perl     && rm perl-5.34.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && true     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 21 Dec 2021 04:03:29 GMT
WORKDIR /
# Tue, 21 Dec 2021 04:03:29 GMT
CMD ["perl5.34.0" "-de0"]
```

-	Layers:
	-	`sha256:893d9e8a132ef3e4de94156342e290ae15179e3e749ae758ca27bd72cd67b6e1`  
		Last Modified: Tue, 21 Dec 2021 01:47:53 GMT  
		Size: 53.2 MB (53194655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f80509ff28f085f5b09954bf0136808ae6b2a37744ef3f8a0c6989c0ff40de21`  
		Last Modified: Tue, 21 Dec 2021 02:17:33 GMT  
		Size: 5.1 MB (5136685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc21e37a06fd996c6ae0abba5be8b2c09baba43d9a6119c4c9e905db2ffeb46`  
		Last Modified: Tue, 21 Dec 2021 02:17:34 GMT  
		Size: 10.8 MB (10761597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed2dbae5528b3a39c8ae6ebd7570ddfcda9993e4addda77f48e17061117c8d8`  
		Last Modified: Tue, 21 Dec 2021 02:17:49 GMT  
		Size: 54.0 MB (54041198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62b0e9760b5d084b8ebc8263ef8e0ed37bbdfc861b33cec6354fe4369287e57`  
		Last Modified: Tue, 21 Dec 2021 02:18:16 GMT  
		Size: 172.5 MB (172511504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f971b265ea7584e5d8b7d96c1d1c605123108202ff9da6e3bdfb9dac7b9b30`  
		Last Modified: Tue, 21 Dec 2021 05:41:46 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dddb0c7b523f5a7a3a797456ec96b707ae727dd6cbdb25f98f9982273b02012e`  
		Last Modified: Tue, 21 Dec 2021 05:42:53 GMT  
		Size: 14.7 MB (14702746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
