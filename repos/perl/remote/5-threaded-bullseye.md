## `perl:5-threaded-bullseye`

```console
$ docker pull perl@sha256:16732fc59dcbd35b2660b01ad9e955f1ac6f9bffc8487b48d0aadb8b86b561da
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

### `perl:5-threaded-bullseye` - linux; amd64

```console
$ docker pull perl@sha256:5196bbd4124795304d478b78f85fbd8150210bdae3f6b1a369f1f4c2c3b4df4d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.0 MB (337980028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c2a8a2b01889d80f3826bf1af95541ddbefee6b7c3d5cf1abe1405d17d55ce5`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:38 GMT
ADD file:d3a2f1f42338ba7066e352cea3b7bf4c7576e6b96fef785e8da763114f337c0e in / 
# Tue, 19 Dec 2023 01:20:38 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 04:33:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 04:33:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 04:34:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 08:24:27 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 19 Dec 2023 08:24:27 GMT
WORKDIR /usr/src/perl
# Tue, 19 Dec 2023 09:06:23 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 19 Dec 2023 09:06:23 GMT
WORKDIR /usr/src/app
# Tue, 19 Dec 2023 09:06:23 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:18f2c3b7ca52caba205d748b9ce41784eb010ca83ece9e84e2a09130a5ec3cbc`  
		Last Modified: Tue, 19 Dec 2023 01:25:17 GMT  
		Size: 55.1 MB (55057340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8988ac7a69cc18b80883227d1cddd6babff98a5fce88b591500f8727dd26ff0d`  
		Last Modified: Tue, 19 Dec 2023 04:42:17 GMT  
		Size: 15.8 MB (15764812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d278fc41a93b35689afe55f7bbeda81194c3ed9d7162d8adf2ed2af1e042ea`  
		Last Modified: Tue, 19 Dec 2023 04:42:32 GMT  
		Size: 54.6 MB (54595440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e04794082b8082ce8c158a02cb11d1d737d6c0cd1542062514b3e2a93f6c70`  
		Last Modified: Tue, 19 Dec 2023 04:43:04 GMT  
		Size: 196.9 MB (196880584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191dc0b607c4b76743dbc3453bf14b3dc7fa767b36f8ebbb85fa12d723986856`  
		Last Modified: Tue, 19 Dec 2023 12:23:46 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7248086677ce90e5ea5c429ac9dd2aae49f07bf5880b0f8f2e5846d886d71b4f`  
		Last Modified: Tue, 19 Dec 2023 12:25:56 GMT  
		Size: 15.7 MB (15681517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c61bf7b2f9dc350f064034daf792da01d3b9e2dfe3bc5c71ac39dd2de036be0`  
		Last Modified: Tue, 19 Dec 2023 12:25:53 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-threaded-bullseye` - linux; arm variant v5

```console
$ docker pull perl@sha256:6b71a9cdc8c5718c4e38f2c68d825a8449d336120be20720c0b81fec46d153d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.3 MB (310304161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45dd18a5f6f7b65a3caef83b53036d400b94be92e12fec7a2a1bdc3e95abfd9e`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Tue, 19 Dec 2023 01:55:29 GMT
ADD file:10a67a16f03367965d9105db3d368f8cf27493769f1551c2bfdc274485bd7f6d in / 
# Tue, 19 Dec 2023 01:55:30 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 05:23:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 05:24:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 05:25:32 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 05:44:54 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 19 Dec 2023 05:44:54 GMT
WORKDIR /usr/src/perl
# Tue, 19 Dec 2023 06:17:00 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 19 Dec 2023 06:17:01 GMT
WORKDIR /usr/src/app
# Tue, 19 Dec 2023 06:17:01 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:476954b0dbc0bbf3e36983f98ae01dfefa01670a85ffcb7ed6916095b71bdd38`  
		Last Modified: Tue, 19 Dec 2023 01:58:55 GMT  
		Size: 52.6 MB (52562242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c916e9180fcbf9c89ebfd7938abc54ad079641855f038c298e679cb1d772eec`  
		Last Modified: Tue, 19 Dec 2023 05:32:39 GMT  
		Size: 15.4 MB (15376057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d33e8d4b6c3b1604296a932879e7916cac6072efd2b9383ab5b5cad23e3a50f`  
		Last Modified: Tue, 19 Dec 2023 05:32:57 GMT  
		Size: 52.3 MB (52331706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4500a3ccfba84ad29d6a187a1df58375b465c6b72d771c80b4ba92087ef6a90`  
		Last Modified: Tue, 19 Dec 2023 05:33:31 GMT  
		Size: 175.1 MB (175098185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:425d8d6cc361fd3aa3c1c9bdcff4d0cd4cbd6bb694af8ed5ec4aa7252797d0eb`  
		Last Modified: Tue, 19 Dec 2023 08:36:58 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a456455718d7b68fcebfc07adeb15a8f6166ed2d8f95ea75ea2bbd238d98784`  
		Last Modified: Tue, 19 Dec 2023 08:38:45 GMT  
		Size: 14.9 MB (14935636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e5b14e5ec4025bf3571d71a6f3f0ce740e3ed43a7d4bb18b9e1524a3ccf6493`  
		Last Modified: Tue, 19 Dec 2023 08:38:40 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-threaded-bullseye` - linux; arm variant v7

```console
$ docker pull perl@sha256:7f2c609a92ce3921801248c18919661e9716756034a54e3bf54d34cd916f4fab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.5 MB (297527366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e31f013daae77a69de69c49c362580c5ec2f2e4abd8117885a628802b25291d`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Tue, 21 Nov 2023 03:57:54 GMT
ADD file:ed8d88d0476fad37879d872d61d05a8cffff35609566f080f78bb882d1bae26b in / 
# Tue, 21 Nov 2023 03:57:54 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 14:05:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 14:05:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 14:06:43 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 14:33:23 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 21 Nov 2023 14:33:23 GMT
WORKDIR /usr/src/perl
# Thu, 30 Nov 2023 19:41:42 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Thu, 30 Nov 2023 19:41:42 GMT
WORKDIR /usr/src/app
# Thu, 30 Nov 2023 19:41:43 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:1dac19092a737e476f9b096fe28463512ae21c4f596dd2f8b84d62530416dffe`  
		Last Modified: Tue, 21 Nov 2023 04:02:11 GMT  
		Size: 50.2 MB (50215653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98461d76c0d7c5e4d320986d659d56aba23d807280d398632ef50acd8a6e028d`  
		Last Modified: Tue, 21 Nov 2023 14:15:07 GMT  
		Size: 14.9 MB (14879655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8eecaf32e1cec433a3782e292748fa035da5e777baaf4ac1861fa6524865c86`  
		Last Modified: Tue, 21 Nov 2023 14:15:27 GMT  
		Size: 50.4 MB (50353119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f7849827a6023dc0eb89664b4bbcb1022abfed00e52a6656cf5c7d397bf3fc7`  
		Last Modified: Tue, 21 Nov 2023 14:15:57 GMT  
		Size: 167.4 MB (167351454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b5b53b581960cc4e1df929623657160935a1ff1535f8d1b2f8b7dd0b5bab05`  
		Last Modified: Tue, 21 Nov 2023 16:27:38 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1046baaf248cddea7c9cef1fe6c7b339a758471e7b1d08cfafbcacaf3f4ba4c3`  
		Last Modified: Thu, 30 Nov 2023 22:09:39 GMT  
		Size: 14.7 MB (14727150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b8bb9ae67d1c86f58ad2a3f3a586781aa90b829cf80aeb5a09415e64b3671c`  
		Last Modified: Thu, 30 Nov 2023 22:09:34 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-threaded-bullseye` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:aa201e18a3c61e93ea9d93419227ed3965563e0e2e8d42c729b75103d8c36978
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.5 MB (329547539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22fa5f459684999e280ace5448bf269afc06a35df2879d61e801a064644f1852`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:17 GMT
ADD file:06ba7e39a2f8e1a7bcbb929fa9d1e6fb1f8bdcf5096dc903576af8f7014e353b in / 
# Tue, 19 Dec 2023 01:41:18 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 11:35:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 11:35:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 11:36:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 14:34:57 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 19 Dec 2023 14:34:57 GMT
WORKDIR /usr/src/perl
# Tue, 19 Dec 2023 14:53:16 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 19 Dec 2023 14:53:17 GMT
WORKDIR /usr/src/app
# Tue, 19 Dec 2023 14:53:17 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:396a672fee8bade1a7c9f228d919717447f110f39046d8b5ed21ad45ae13ab61`  
		Last Modified: Tue, 19 Dec 2023 01:44:57 GMT  
		Size: 53.7 MB (53708091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:010797996cc86cf2cf7495aebc22e5be7d18a10bde1e11562dbe5283c226c0e9`  
		Last Modified: Tue, 19 Dec 2023 11:43:17 GMT  
		Size: 15.8 MB (15750308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70092c2a6b382a0cc0bd2adeb187b94d74c8bcf2ceb6f33bb8e4e4e9c6561141`  
		Last Modified: Tue, 19 Dec 2023 11:43:31 GMT  
		Size: 54.7 MB (54699871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc4a505c38c38e8d9b219e6c3ed4fc061369233b452cca74b29876a248cfea2`  
		Last Modified: Tue, 19 Dec 2023 11:43:56 GMT  
		Size: 189.8 MB (189799678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf22060d9596d7fbfc37987d7ea28ef11bb14112bbca0e29d0a2b994d489b09`  
		Last Modified: Tue, 19 Dec 2023 16:05:12 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a54a25171f72b5ae79026c8036bad0d5b8c57f1e2d3a6a15a3fe3da2e2e8945`  
		Last Modified: Tue, 19 Dec 2023 16:06:25 GMT  
		Size: 15.6 MB (15589258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa493f0c2ce2a9c6a60b925eb85f936df41fb4cbb1ad2108e69ddaf573c358b`  
		Last Modified: Tue, 19 Dec 2023 16:06:22 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-threaded-bullseye` - linux; 386

```console
$ docker pull perl@sha256:8db2a7895f21d7188bcc0aa51c216e47015145d4f25ddfb4bf2f6b8945459982
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.3 MB (343260513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bf90148fac84d2335ed63245cb5f0c5dd7be04f659c6b6ffce940c00cc136ca`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Tue, 21 Nov 2023 04:40:03 GMT
ADD file:54170328827ccc52692c964f0c45a65ed6efdf39897f2c226672fdf526f3c412 in / 
# Tue, 21 Nov 2023 04:40:04 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 15:25:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 15:25:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 15:26:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 01:42:07 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 22 Nov 2023 01:42:07 GMT
WORKDIR /usr/src/perl
# Thu, 30 Nov 2023 21:05:05 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Thu, 30 Nov 2023 21:05:06 GMT
WORKDIR /usr/src/app
# Thu, 30 Nov 2023 21:05:06 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:e33c1468a29e45636d4d9529b663048f7e8aa83ff428eb0681253bd4200e23ec`  
		Last Modified: Tue, 21 Nov 2023 04:44:57 GMT  
		Size: 56.0 MB (56046301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50bbecef785328ce3a55c9be635ad1af8cedfba6ce5c0e5911a249381a479d5`  
		Last Modified: Tue, 21 Nov 2023 15:35:51 GMT  
		Size: 16.3 MB (16268214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2046634e054ee805901e2887a46c4c265c5130e7c4ddbdee7cf0467f32976be5`  
		Last Modified: Tue, 21 Nov 2023 15:36:13 GMT  
		Size: 55.9 MB (55937176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce6bca4df8961023f4b46de892472cbf36d3b60e1a8d49e85e19b9568f17a6c`  
		Last Modified: Tue, 21 Nov 2023 15:37:04 GMT  
		Size: 199.8 MB (199796687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63afd47a39f36eeec03df68adb5cc425a83cb7d09d019dabdbfbf2aeb71a583`  
		Last Modified: Wed, 22 Nov 2023 05:02:23 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9ab7243751d8cc8def2668b1eb59e9a89b9723578056f461cbd58c81ca3512`  
		Last Modified: Fri, 01 Dec 2023 01:31:51 GMT  
		Size: 15.2 MB (15211802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b61bcc2877bfe924094f7e7cc5e6ac3d209282794dfe394a5741b6733a34879`  
		Last Modified: Fri, 01 Dec 2023 01:31:47 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-threaded-bullseye` - linux; mips64le

```console
$ docker pull perl@sha256:fc1d7cad60db75a4908d0ac62a891e0581fdef67ef9eec7f91c020a0dd6945d8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.0 MB (316022622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:145dc5468c553651cc49d48c49fbe4b69376ef62b268e7a4dbe0686e4b25136e`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Tue, 21 Nov 2023 04:10:25 GMT
ADD file:dbfc3d226166089c4db0c154fdcea8049b8758c6812f1c397dec1444985e8557 in / 
# Tue, 21 Nov 2023 04:10:31 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 12:31:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 12:33:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 12:38:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 10:57:18 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 22 Nov 2023 10:57:24 GMT
WORKDIR /usr/src/perl
# Thu, 30 Nov 2023 21:31:20 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Thu, 30 Nov 2023 21:31:27 GMT
WORKDIR /usr/src/app
# Thu, 30 Nov 2023 21:31:33 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:ca31218601e95f4aafae0dcadda7600aeb04db374e1e829d5c123f8033ba3472`  
		Last Modified: Tue, 21 Nov 2023 04:21:21 GMT  
		Size: 53.3 MB (53289162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4053cd5a6af26fb90d7c0467241aaec093f035fa809a6ca17aa5e69d24eebd58`  
		Last Modified: Tue, 21 Nov 2023 13:01:44 GMT  
		Size: 15.5 MB (15529758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:174e243a4b8e6e8f714c8eb9ebef84bfaab27bdf92fcd3f0a409c73f5247d976`  
		Last Modified: Tue, 21 Nov 2023 13:02:31 GMT  
		Size: 53.3 MB (53302699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf9a34314b28ef89fdecdef1e9a4eb98f9f43ac10964fce4c19fdb1e05fa10a`  
		Last Modified: Tue, 21 Nov 2023 13:04:28 GMT  
		Size: 179.0 MB (179003553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec67bd715feb126665a9b39e1a4bffd03997d9b8c25dab0b7a52bc0134cb30d`  
		Last Modified: Wed, 22 Nov 2023 16:09:58 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f622dbefde5893d6b6a20dd005b6d09882e2555d97e45a44c11f9ff6c10b6831`  
		Last Modified: Fri, 01 Dec 2023 03:25:53 GMT  
		Size: 14.9 MB (14897185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be1640e92d911cea0a9c587195b88263a54107562422eeb9de81fd8948ca1236`  
		Last Modified: Fri, 01 Dec 2023 03:25:41 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-threaded-bullseye` - linux; ppc64le

```console
$ docker pull perl@sha256:4fc711474fe4ce84a0804e2249ae293751d23852185bcfb6c1369776943721ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.5 MB (346516541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52876999a0179cf332a6b288ce8fd6376781b32b46b9e972491693d3dda2228f`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:26 GMT
ADD file:c21c2b6cb3f9bdf6cc3641e9ebf810a461174480c6cd1c25515cf9fce4aa2143 in / 
# Tue, 21 Nov 2023 04:24:30 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:56:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:57:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:58:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 16:55:04 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 21 Nov 2023 16:55:04 GMT
WORKDIR /usr/src/perl
# Thu, 30 Nov 2023 20:14:03 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Thu, 30 Nov 2023 20:14:18 GMT
WORKDIR /usr/src/app
# Thu, 30 Nov 2023 20:14:19 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:23ebe74b854f8f6e2671f4c8cc147a6925fb7d929ce5898f7ca2af9781bf7d38`  
		Last Modified: Tue, 21 Nov 2023 04:29:21 GMT  
		Size: 58.9 MB (58929678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1736e334b1e250eaca590180779f3cbbdea68af8d960e1795174a8524fe6517`  
		Last Modified: Tue, 21 Nov 2023 07:08:03 GMT  
		Size: 16.8 MB (16765413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdaf6761a16c321d5d91b3da652f34fb1b7bde7c3cd21ef5adab0f5622b5abf6`  
		Last Modified: Tue, 21 Nov 2023 07:08:22 GMT  
		Size: 58.9 MB (58866450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071a148a4e40b127789a1fa17ce9bddefefb7832718f122f278a3521df2a87d8`  
		Last Modified: Tue, 21 Nov 2023 07:08:59 GMT  
		Size: 196.2 MB (196245923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:017d2a71c3d0b46a002af0bde6639ef6585729bb09524fdf9b33b7ed620c0ccc`  
		Last Modified: Tue, 21 Nov 2023 19:40:17 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5189054c13a810448b0f6bf4fe7500538f148e909fb5dfa8ef8385867b229e34`  
		Last Modified: Thu, 30 Nov 2023 22:38:15 GMT  
		Size: 15.7 MB (15708744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced2b135df5f177cfea6fb7704e21955dbb63765e2805aa8359730e8ad1c63a9`  
		Last Modified: Thu, 30 Nov 2023 22:38:11 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-threaded-bullseye` - linux; s390x

```console
$ docker pull perl@sha256:567c9b038f788ae4eeb8f7849b1666f30c539e71541753ff6e3af3ec662222cf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.9 MB (311924598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0968ff8cc6d143c29c836848860cd6a1a72b76987a2e10651cb8fbdbff06ce18`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Tue, 19 Dec 2023 01:42:51 GMT
ADD file:f3ff7311d9c8e7c83e0b7746d9402fed156fb05bd0c704d49535b4ece7f33177 in / 
# Tue, 19 Dec 2023 01:42:55 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 07:45:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 07:45:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 07:46:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 13:01:39 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 19 Dec 2023 13:01:39 GMT
WORKDIR /usr/src/perl
# Tue, 19 Dec 2023 13:20:21 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 19 Dec 2023 13:20:22 GMT
WORKDIR /usr/src/app
# Tue, 19 Dec 2023 13:20:22 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:a7334865824cce0a21e0af9d1f48eaee160e0ac01a54ca220a9814e8d2059646`  
		Last Modified: Tue, 19 Dec 2023 01:47:52 GMT  
		Size: 53.3 MB (53295959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e096c63fd53eae4f8f314ef4db6a5af5579dae607952ecf51910447be347d0bf`  
		Last Modified: Tue, 19 Dec 2023 07:54:24 GMT  
		Size: 15.6 MB (15642144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008c491e9bc699339e05fa0f22fa74aacc65ae31563bf94ba464e87cb6d543a4`  
		Last Modified: Tue, 19 Dec 2023 07:54:39 GMT  
		Size: 54.1 MB (54065902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa1b9ec5b62c545680bff8a4afa9e19cfe778e934275d5fea6e0034382a87151`  
		Last Modified: Tue, 19 Dec 2023 07:55:05 GMT  
		Size: 172.9 MB (172895954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:137858c588eb124ec23005a54d51e2a289cc75eb4c21ef63a228959c09824a42`  
		Last Modified: Tue, 19 Dec 2023 14:25:30 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd154fe24ebcf422afa3ada4556f72cf97e65d2f3e0e94ce05d09e27e0b0c7d0`  
		Last Modified: Tue, 19 Dec 2023 14:26:10 GMT  
		Size: 16.0 MB (16024303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab57a6298360c50f04ccc9059e3726b1febdaecf78704a5ea00d2ab146ed9ce4`  
		Last Modified: Tue, 19 Dec 2023 14:26:06 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
