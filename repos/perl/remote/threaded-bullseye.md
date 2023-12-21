## `perl:threaded-bullseye`

```console
$ docker pull perl@sha256:3ffb1c452c32a2b1e5ee246cdd2041f518776b2f67531dc2b1919686ec8ca078
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 16
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v5
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; mips64le
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `perl:threaded-bullseye` - linux; amd64

```console
$ docker pull perl@sha256:803a195dc9172460f48ccdfaf75819dd87927c335b406d0b8adcc00e7bb4d1bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.0 MB (337979716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f44a3993505fd9bfbaaa009e8c1444f73be024805366a60953c49e52508e55cd`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Thu, 30 Nov 2023 02:54:02 GMT
ADD file:d3a2f1f42338ba7066e352cea3b7bf4c7576e6b96fef785e8da763114f337c0e in / 
# Thu, 30 Nov 2023 02:54:02 GMT
CMD ["bash"]
# Thu, 30 Nov 2023 02:54:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
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
	-	`sha256:18f2c3b7ca52caba205d748b9ce41784eb010ca83ece9e84e2a09130a5ec3cbc`  
		Last Modified: Tue, 19 Dec 2023 01:25:17 GMT  
		Size: 55.1 MB (55057340 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8988ac7a69cc18b80883227d1cddd6babff98a5fce88b591500f8727dd26ff0d`  
		Last Modified: Tue, 19 Dec 2023 04:42:17 GMT  
		Size: 15.8 MB (15764812 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d8d278fc41a93b35689afe55f7bbeda81194c3ed9d7162d8adf2ed2af1e042ea`  
		Last Modified: Tue, 19 Dec 2023 04:42:32 GMT  
		Size: 54.6 MB (54595440 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d5e04794082b8082ce8c158a02cb11d1d737d6c0cd1542062514b3e2a93f6c70`  
		Last Modified: Tue, 19 Dec 2023 04:43:04 GMT  
		Size: 196.9 MB (196880584 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:155b7fcd1b4b66cb1ec8c3df405cd054fe676c9bf93b94583beb7b1d8a525d79`  
		Last Modified: Wed, 20 Dec 2023 20:16:04 GMT  
		Size: 135.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:156e9bb31d6f8e10cab446ec1b82f0d9238c50df4d7fbbc36ab543aba57bfc46`  
		Last Modified: Wed, 20 Dec 2023 20:16:04 GMT  
		Size: 15.7 MB (15681273 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:07aa65e184601c54c24919ecbe0ebbd7098a221455d546b1a34fd4b8a6e16ba9`  
		Last Modified: Wed, 20 Dec 2023 20:15:51 GMT  
		Size: 132.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `perl:threaded-bullseye` - unknown; unknown

```console
$ docker pull perl@sha256:14d55b5620253c0a82ec0b7f120a5b26e86875315e45019ff3ec70e6e69e20f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.0 MB (12969257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3116709c0a9811701e93921aa6eaff3ed9f94c01cc1951a9f107f4ef1af8b59`

```dockerfile
```

-	Layers:
	-	`sha256:7b72c2a72529e1754f6573b0a10fd6a7cbe3cbb0184b982e325422204fbc44b5`  
		Last Modified: Wed, 20 Dec 2023 20:16:04 GMT  
		Size: 13.0 MB (12952742 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:3340c2b1b720e7b11811e0a4294c11afd22ae52634fedcb1706952814b7f3b86`  
		Last Modified: Wed, 20 Dec 2023 20:16:04 GMT  
		Size: 16.5 KB (16515 bytes)  
		MIME: application/vnd.in-toto+json

### `perl:threaded-bullseye` - linux; arm variant v5

```console
$ docker pull perl@sha256:9ce6f7d2bdb2599b7a20721f7a5f24357159d491afe337b137d665a3833cb6b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.3 MB (310303689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46378f51fad387874f70160bca42ec30907e8cfaabd70340468bc946564159d1`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Thu, 30 Nov 2023 02:54:02 GMT
ADD file:10a67a16f03367965d9105db3d368f8cf27493769f1551c2bfdc274485bd7f6d in / 
# Thu, 30 Nov 2023 02:54:02 GMT
CMD ["bash"]
# Thu, 30 Nov 2023 02:54:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
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
	-	`sha256:476954b0dbc0bbf3e36983f98ae01dfefa01670a85ffcb7ed6916095b71bdd38`  
		Last Modified: Tue, 19 Dec 2023 01:58:55 GMT  
		Size: 52.6 MB (52562242 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c916e9180fcbf9c89ebfd7938abc54ad079641855f038c298e679cb1d772eec`  
		Last Modified: Tue, 19 Dec 2023 05:32:39 GMT  
		Size: 15.4 MB (15376057 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1d33e8d4b6c3b1604296a932879e7916cac6072efd2b9383ab5b5cad23e3a50f`  
		Last Modified: Tue, 19 Dec 2023 05:32:57 GMT  
		Size: 52.3 MB (52331706 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f4500a3ccfba84ad29d6a187a1df58375b465c6b72d771c80b4ba92087ef6a90`  
		Last Modified: Tue, 19 Dec 2023 05:33:31 GMT  
		Size: 175.1 MB (175098185 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ebb57add6a3aa653fe62bba7dad84ac512ccca3c1e667b837961ba607b93ce74`  
		Last Modified: Wed, 20 Dec 2023 20:56:06 GMT  
		Size: 136.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:53d7757d99a26be67ccc6a10cb1e6fbb12ee504170f9f4febda257d168099dc6`  
		Last Modified: Wed, 20 Dec 2023 21:34:05 GMT  
		Size: 14.9 MB (14935231 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ff54385d25f715308cf16869830c0d4c461a39b8c426cb829fa84eeeebe6be15`  
		Last Modified: Wed, 20 Dec 2023 21:34:04 GMT  
		Size: 132.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `perl:threaded-bullseye` - unknown; unknown

```console
$ docker pull perl@sha256:a54345e504c58c1ad90fa4059bfaccd46a2eacc74047e2d76b40b8ff3a3ad695
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 KB (15715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c49139682cad7ea9e2f94a93829c6bdadba3bfb6527a9933ed4009d18a7dc723`

```dockerfile
```

-	Layers:
	-	`sha256:037669b13d7f6ea1d5c12a313279d855bbeaf19e02de661ffd7c7351bf44ac98`  
		Last Modified: Wed, 20 Dec 2023 21:34:03 GMT  
		Size: 15.7 KB (15715 bytes)  
		MIME: application/vnd.in-toto+json

### `perl:threaded-bullseye` - linux; arm variant v7

```console
$ docker pull perl@sha256:8dd374505239756cebb01e476aa9091a47868a53cce9eea45b602f1db9578ca0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.5 MB (297532015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ca806b4354b486470a45e637d84ff6180e3250a90c430a9af52efc54e4de6c6`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Thu, 30 Nov 2023 02:54:02 GMT
ADD file:3b623bed8ec2536cb513edda1de6f79d2c8e06d6f82df2543202544dbba3ae3e in / 
# Thu, 30 Nov 2023 02:54:02 GMT
CMD ["bash"]
# Thu, 30 Nov 2023 02:54:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
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
	-	`sha256:1b42212018867046767b36eb95cf15c4b66bbb7b4fb552aab446d9822de5765c`  
		Last Modified: Tue, 19 Dec 2023 02:12:11 GMT  
		Size: 50.2 MB (50215775 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:344f6b88eeb188b9948991d7a318480a17a477fd684c6fbdc230ad9a217fed92`  
		Last Modified: Tue, 19 Dec 2023 08:07:28 GMT  
		Size: 14.9 MB (14880518 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a36372cf5bdff61f93cd6e14b66d2512eebf0c58b08179f661fbb89bdd34a5ca`  
		Last Modified: Tue, 19 Dec 2023 08:07:48 GMT  
		Size: 50.4 MB (50353358 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0a95e5981b0054b45d45e8a79f8a82867bfaae0efacc3cdf24f750d4ec2eb6bb`  
		Last Modified: Tue, 19 Dec 2023 08:08:18 GMT  
		Size: 167.4 MB (167352715 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:50c5350c4f82a703e90df58a3a890d7632efc4fcf6021032b584fe0222931f43`  
		Last Modified: Wed, 20 Dec 2023 23:38:37 GMT  
		Size: 135.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:028e27d051183acaa5581e06efe43db954bbd08bdb6f2e58c5092562d89afb02`  
		Last Modified: Thu, 21 Dec 2023 00:37:26 GMT  
		Size: 14.7 MB (14729381 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:90dcf838edce2686a08848ea48f63464dbb96c66595ab37d72a9c8571f16ae50`  
		Last Modified: Thu, 21 Dec 2023 00:37:25 GMT  
		Size: 133.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `perl:threaded-bullseye` - unknown; unknown

```console
$ docker pull perl@sha256:597d80d63d6fc8ef49e2d61208ccd8d551e46a2ad652c729b3223e5277a9d4b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.8 MB (12796327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd0a6bd2d1a784981f30862d18693a0883b316fd4c262c1b2f76ab5c5d0361e5`

```dockerfile
```

-	Layers:
	-	`sha256:38a5c01ba7f2a7abea5293c0198968f3e0939d8f16e9b1825ee37a64c581f35e`  
		Last Modified: Thu, 21 Dec 2023 00:37:26 GMT  
		Size: 12.8 MB (12780397 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:be62797e9db3dd19d7dce136046e255bee87b226fe7d1d6d612f11ff8b085ec9`  
		Last Modified: Thu, 21 Dec 2023 00:37:25 GMT  
		Size: 15.9 KB (15930 bytes)  
		MIME: application/vnd.in-toto+json

### `perl:threaded-bullseye` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:fc8aeb1e00c4fbc112a5d3ca31de835e200739ef1b47afc973f33d992735364b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.5 MB (329547787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a85fbeda314fc6d0523aa50329b7783d086ec503de5e75b3e87c084aa77e884`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Thu, 30 Nov 2023 02:54:02 GMT
ADD file:06ba7e39a2f8e1a7bcbb929fa9d1e6fb1f8bdcf5096dc903576af8f7014e353b in / 
# Thu, 30 Nov 2023 02:54:02 GMT
CMD ["bash"]
# Thu, 30 Nov 2023 02:54:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
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
	-	`sha256:396a672fee8bade1a7c9f228d919717447f110f39046d8b5ed21ad45ae13ab61`  
		Last Modified: Tue, 19 Dec 2023 01:44:57 GMT  
		Size: 53.7 MB (53708091 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:010797996cc86cf2cf7495aebc22e5be7d18a10bde1e11562dbe5283c226c0e9`  
		Last Modified: Tue, 19 Dec 2023 11:43:17 GMT  
		Size: 15.8 MB (15750308 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:70092c2a6b382a0cc0bd2adeb187b94d74c8bcf2ceb6f33bb8e4e4e9c6561141`  
		Last Modified: Tue, 19 Dec 2023 11:43:31 GMT  
		Size: 54.7 MB (54699871 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0cc4a505c38c38e8d9b219e6c3ed4fc061369233b452cca74b29876a248cfea2`  
		Last Modified: Tue, 19 Dec 2023 11:43:56 GMT  
		Size: 189.8 MB (189799678 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:617f85d36eb70fb3a5ae81fea2a0428e472dedc4658a7b93ffa8f9e0198e9a3b`  
		Last Modified: Wed, 20 Dec 2023 22:47:07 GMT  
		Size: 135.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8bb4c56983611d019a8779115aeaebf38f3401e68249446cc1578c671e3fc606`  
		Last Modified: Wed, 20 Dec 2023 23:52:44 GMT  
		Size: 15.6 MB (15589573 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a9ed9e0ce3962217757d444e8c885b488c0d9dc8abb111f3b04bc289472c14c6`  
		Last Modified: Wed, 20 Dec 2023 23:52:43 GMT  
		Size: 131.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `perl:threaded-bullseye` - unknown; unknown

```console
$ docker pull perl@sha256:7177c9b1f3cbae150f25ce6036679038112cf074d45d82cbd1a4e1a763a1434d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.0 MB (12970968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3c78e843b1d7324ab875f20cc23081c34fb048102a304100ab9b3ccdd0d4d43`

```dockerfile
```

-	Layers:
	-	`sha256:5ef2226246b3559bf9c7055c57880e12542fec97e6121695b4575533161f0d94`  
		Last Modified: Wed, 20 Dec 2023 23:52:45 GMT  
		Size: 13.0 MB (12955104 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:654cfca0d0af7d96c87bd596e40af56516af01b7c46eeb297168ac64a4b1437e`  
		Last Modified: Wed, 20 Dec 2023 23:52:43 GMT  
		Size: 15.9 KB (15864 bytes)  
		MIME: application/vnd.in-toto+json

### `perl:threaded-bullseye` - linux; 386

```console
$ docker pull perl@sha256:b054c61b1d565bfd9861149ecc73c03a613d8db1d0dee6b3bd81d22f2c47d83d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.3 MB (343261644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:696c0275aca251cc9d39b27c1e526b914d4714bfdd11a2cc4d4babebafcbd224`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Thu, 30 Nov 2023 02:54:02 GMT
ADD file:8a328fced7ae3a6fc868bbb95c23191103e595c9d22b2626c16f155bc48b51a8 in / 
# Thu, 30 Nov 2023 02:54:02 GMT
CMD ["bash"]
# Thu, 30 Nov 2023 02:54:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
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
	-	`sha256:a789657fd5416b1ccfd519597a8f5e57bd5a80d04d1b1b7b2770df4469f4dd44`  
		Last Modified: Tue, 19 Dec 2023 01:44:07 GMT  
		Size: 56.0 MB (56046336 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0386e6c873ad0aec679cfb967e1449dc2223a2543dd9923e9491c8d4dfe25ff9`  
		Last Modified: Tue, 19 Dec 2023 03:37:37 GMT  
		Size: 16.3 MB (16268921 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4a344c33a496f0c80e861246ac1b15db106b888d28c7bb89d17b87d06a5f1abc`  
		Last Modified: Tue, 19 Dec 2023 03:37:57 GMT  
		Size: 55.9 MB (55937182 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8fb89bdf92d460c8b83c3effc827149c832709e4d9e4e2262456e267a2e4decf`  
		Last Modified: Tue, 19 Dec 2023 03:38:42 GMT  
		Size: 199.8 MB (199796881 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4baf8853abdd078bceba2d0654c4943f0fb2ea9ce31e98cdd883cc1b237457a2`  
		Last Modified: Wed, 20 Dec 2023 20:17:00 GMT  
		Size: 136.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:321c0fe6070386e90977156ec7257085906e9056e810f9323c15f6c3bd2c580e`  
		Last Modified: Wed, 20 Dec 2023 20:17:01 GMT  
		Size: 15.2 MB (15212056 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0acd81b57ebf3beeff8ff71898cc4f5e9353c6068e71d4634ac852e6849721b2`  
		Last Modified: Wed, 20 Dec 2023 20:17:00 GMT  
		Size: 132.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `perl:threaded-bullseye` - unknown; unknown

```console
$ docker pull perl@sha256:8518968384c822353922679784533fa4da9f4529148f998f18051a4605b64b97
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 KB (16265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d4b85b83142430e47f1567e8916d13a61d3e0676fcfdbcd29cd559025cf8458`

```dockerfile
```

-	Layers:
	-	`sha256:00ca50b70f3ed559ab793dc19e543d0061daf4ef937c4fbd69847d89074b3db6`  
		Last Modified: Wed, 20 Dec 2023 20:17:00 GMT  
		Size: 16.3 KB (16265 bytes)  
		MIME: application/vnd.in-toto+json

### `perl:threaded-bullseye` - linux; mips64le

```console
$ docker pull perl@sha256:2470dbbf6c6abfaee11981a3228098ee08815e78f4f03dccf041665a6223c766
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.0 MB (316029006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ae09c71fd7f91245e8a8df91e7baf43185920c61a1053aa1c0c425fb2dd0080`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Thu, 30 Nov 2023 02:54:02 GMT
ADD file:95472c5be6ea30c4b6d715a3000e1bafb8e371897a96c9115040c4a7d2bb2c80 in / 
# Thu, 30 Nov 2023 02:54:02 GMT
CMD ["bash"]
# Thu, 30 Nov 2023 02:54:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
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
	-	`sha256:4d8f97806f78898e256ac429d0634dfcccbd6f6e81547afde1469a5968e33b18`  
		Last Modified: Tue, 19 Dec 2023 02:25:21 GMT  
		Size: 53.3 MB (53289008 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6729089c3e56fc6fa74aeb41283960af5e717a1e32232fb0de332e8b8393fc37`  
		Last Modified: Tue, 19 Dec 2023 03:22:13 GMT  
		Size: 15.5 MB (15530289 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a6e24f65044fa0f3a3c6a2bf5c15dd5d639173537bdcd52919cfc676d1bbd685`  
		Last Modified: Tue, 19 Dec 2023 03:22:58 GMT  
		Size: 53.3 MB (53302689 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b629433016e1325add5a9e6adac29d769012947b8e2ffaccf1a6796cf6312892`  
		Last Modified: Tue, 19 Dec 2023 03:24:56 GMT  
		Size: 179.0 MB (179003314 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dd7a51ed13ccec8991eca53ae8bf133ddf0b8286fee82de95621ee77eb943e01`  
		Last Modified: Thu, 21 Dec 2023 16:26:47 GMT  
		Size: 136.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:090d93377684d8e7e46d41389f5afe14d033f7670e21b4e5fe250cd93b40ecf6`  
		Last Modified: Thu, 21 Dec 2023 18:15:49 GMT  
		Size: 14.9 MB (14903438 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0712cef4fda6d70bd75121c51e48965154fd74514c7efebee3853ecd44d4b9bf`  
		Last Modified: Thu, 21 Dec 2023 18:15:48 GMT  
		Size: 132.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `perl:threaded-bullseye` - unknown; unknown

```console
$ docker pull perl@sha256:32540599debeef80eb7389128715725abc45a2a6e0bada1d4b4f33f05d0c19dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 KB (15703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d32ff85ac06fc6c738f6106ef0cc3d73b0f5094ea213f3e242d067d4ea99bb9`

```dockerfile
```

-	Layers:
	-	`sha256:f1f355f87e6813f11a02eeaef028ff16c1239f8416dc701f5e599b0cbb67e225`  
		Last Modified: Thu, 21 Dec 2023 18:15:47 GMT  
		Size: 15.7 KB (15703 bytes)  
		MIME: application/vnd.in-toto+json

### `perl:threaded-bullseye` - linux; ppc64le

```console
$ docker pull perl@sha256:339b3d8faee927876bd06ccaf96d5a5b209be463578a8ac139c2d5a585ce5a60
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.5 MB (346519596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d94115bb05838f59ce4b7dafebe5c65473c221662b52c0c0176a8e785cd6ba4`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Thu, 30 Nov 2023 02:54:02 GMT
ADD file:240a318dbc8a7ec4b3a6af5afec173d3579c94c27738b0f79750242acce5dd2f in / 
# Thu, 30 Nov 2023 02:54:02 GMT
CMD ["bash"]
# Thu, 30 Nov 2023 02:54:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
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
	-	`sha256:bdab4f9926bc1dc6c30480616baa760641ee4feeca1b5215d5c420b718c5a1a3`  
		Last Modified: Tue, 19 Dec 2023 01:26:44 GMT  
		Size: 58.9 MB (58929912 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5180a9882628ce87cf92f22142ff50ab10a6b9836f1ee8b3f4a4db8afab99f62`  
		Last Modified: Tue, 19 Dec 2023 12:24:04 GMT  
		Size: 16.8 MB (16766736 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:05ffb56ddbf3543b23b4a70af435c61ab9572ba994a4a98817b5efec8daf4084`  
		Last Modified: Tue, 19 Dec 2023 12:24:23 GMT  
		Size: 58.9 MB (58866991 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:034864951bd2e5c9836b63881b14af9f88ece461697ca805625708f42242232d`  
		Last Modified: Tue, 19 Dec 2023 12:25:01 GMT  
		Size: 196.2 MB (196248564 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9ac3b60d6b9d027c8018a98e6fc27e68bac17be9eb84fcfb11d57c2dd82c11de`  
		Last Modified: Wed, 20 Dec 2023 21:38:58 GMT  
		Size: 135.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2541b051ef0c91e3332d73f7d0e25da6baae78022287c2d6f24a152007b00267`  
		Last Modified: Wed, 20 Dec 2023 22:05:25 GMT  
		Size: 15.7 MB (15707126 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:085785e38ea7a4b4dad606e7ae73b7ed6a7feba35ea7aaab839fe43e80384261`  
		Last Modified: Wed, 20 Dec 2023 22:05:24 GMT  
		Size: 132.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `perl:threaded-bullseye` - unknown; unknown

```console
$ docker pull perl@sha256:9983362a36ca818982b3ad66afd5e864e66a94cb4efa9de7f4b04077246e2e2e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.9 MB (12943991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f75fd283f9d87dab9edfbd4088b4e3c361786608e41506eeac1f155654b6e8f`

```dockerfile
```

-	Layers:
	-	`sha256:6d53b6ec1a3d3b1ef1b8d000f439d5653f8246c4c32d11c42ec8dc3029c96dba`  
		Last Modified: Wed, 20 Dec 2023 22:05:25 GMT  
		Size: 12.9 MB (12928095 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:2a90b384cf625256afdcf914203b585ef74adc690dfa8733306def6f50452576`  
		Last Modified: Wed, 20 Dec 2023 22:05:24 GMT  
		Size: 15.9 KB (15896 bytes)  
		MIME: application/vnd.in-toto+json

### `perl:threaded-bullseye` - linux; s390x

```console
$ docker pull perl@sha256:9d2e02f3d72dc60dcece60e717cb1f5accb33c7345e55fee8391252745450523
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.9 MB (311924863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:490df0df4faef8e83e8a1bbe50e5fe0cce3f1e0defe7a6f1c621f11d0ae0452d`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Thu, 30 Nov 2023 02:54:02 GMT
ADD file:f3ff7311d9c8e7c83e0b7746d9402fed156fb05bd0c704d49535b4ece7f33177 in / 
# Thu, 30 Nov 2023 02:54:02 GMT
CMD ["bash"]
# Thu, 30 Nov 2023 02:54:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
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
	-	`sha256:a7334865824cce0a21e0af9d1f48eaee160e0ac01a54ca220a9814e8d2059646`  
		Last Modified: Tue, 19 Dec 2023 01:47:52 GMT  
		Size: 53.3 MB (53295959 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e096c63fd53eae4f8f314ef4db6a5af5579dae607952ecf51910447be347d0bf`  
		Last Modified: Tue, 19 Dec 2023 07:54:24 GMT  
		Size: 15.6 MB (15642144 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:008c491e9bc699339e05fa0f22fa74aacc65ae31563bf94ba464e87cb6d543a4`  
		Last Modified: Tue, 19 Dec 2023 07:54:39 GMT  
		Size: 54.1 MB (54065902 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fa1b9ec5b62c545680bff8a4afa9e19cfe778e934275d5fea6e0034382a87151`  
		Last Modified: Tue, 19 Dec 2023 07:55:05 GMT  
		Size: 172.9 MB (172895954 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8f0859d15132527668a50ed2ec2d6c81dde1a64fcf610f9c40b5f9579b461ee7`  
		Last Modified: Wed, 20 Dec 2023 21:44:15 GMT  
		Size: 136.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e691268ed8e195adcb0304ee05af24aa31e49f2ae400fa99b4a39866b11d869a`  
		Last Modified: Wed, 20 Dec 2023 22:11:33 GMT  
		Size: 16.0 MB (16024636 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3fac461c427925cb104f170207a2e5f9790e033723e2d9130ed51c205e0fcb90`  
		Last Modified: Wed, 20 Dec 2023 22:11:33 GMT  
		Size: 132.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `perl:threaded-bullseye` - unknown; unknown

```console
$ docker pull perl@sha256:e3211bfe8e6f16f0b88b7db0b6ae2de7ffa544404aba5d700890790140d593a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.8 MB (12812212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04a86b21ac31711130e2e3f27b9a4957a97cc7d7d88a6e223d5f9a6a7f560d42`

```dockerfile
```

-	Layers:
	-	`sha256:5f0dec4ecbb1dcb3dc797859f74277646ccbad90dd08b98eede28253e4ec2989`  
		Last Modified: Wed, 20 Dec 2023 22:11:33 GMT  
		Size: 12.8 MB (12796360 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:ffb9f29cee5577451d41f8f60a5643e2fe830a8ea3c48cb91ea3ac837094681e`  
		Last Modified: Wed, 20 Dec 2023 22:11:32 GMT  
		Size: 15.9 KB (15852 bytes)  
		MIME: application/vnd.in-toto+json
