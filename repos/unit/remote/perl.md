## `unit:perl`

```console
$ docker pull unit@sha256:b02a63f41a391d29e27b8450d9eb411e41576ca90f39f983f412f83b6ee069fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:perl` - linux; amd64

```console
$ docker pull unit@sha256:8fb0eec59177ca2b447bdceead1ae73dfa7e33cbdaed5eee9043c5b75cde330b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **345.1 MB (345141304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ff5d9adf48ca243a61dd9f52137c95d3ddc8e9f63693ac2a9f04fc97563a355`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:01 GMT
ADD file:144dff349a666134b5e98a9f1c6650fd9d6e4a88a6f98857f26eb84989360b91 in / 
# Thu, 07 Sep 2023 00:21:02 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:57:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:58:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:58:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 07:37:33 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 07 Sep 2023 07:37:34 GMT
WORKDIR /usr/src/perl
# Thu, 07 Sep 2023 07:42:51 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Thu, 07 Sep 2023 07:42:51 GMT
WORKDIR /usr/src/app
# Thu, 07 Sep 2023 07:42:51 GMT
CMD ["perl5.38.0" "-de0"]
# Thu, 07 Sep 2023 15:03:38 GMT
LABEL org.opencontainers.image.title=Unit (perl5.38)
# Thu, 07 Sep 2023 15:03:39 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Thu, 07 Sep 2023 15:03:39 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Thu, 07 Sep 2023 15:03:39 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Thu, 07 Sep 2023 15:03:39 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Thu, 07 Sep 2023 15:03:39 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Thu, 07 Sep 2023 15:03:39 GMT
LABEL org.opencontainers.image.version=1.31.0
# Thu, 07 Sep 2023 15:04:31 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure perl     && make -j $NCPU perl-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure perl     && make -j $NCPU perl-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Thu, 07 Sep 2023 15:04:31 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Thu, 07 Sep 2023 15:04:31 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Thu, 07 Sep 2023 15:04:31 GMT
STOPSIGNAL SIGTERM
# Thu, 07 Sep 2023 15:04:31 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 07 Sep 2023 15:04:31 GMT
EXPOSE 80
# Thu, 07 Sep 2023 15:04:31 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:5dea071bb9782209397443f024a630052ab7583e365894d414f1e39cd0f65025`  
		Last Modified: Thu, 07 Sep 2023 00:25:41 GMT  
		Size: 55.1 MB (55056245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d190df514e96e82a9048dff1406b65e853dbdfbfc0d8474b85ef6bf37bfea62a`  
		Last Modified: Thu, 07 Sep 2023 03:05:52 GMT  
		Size: 15.8 MB (15760386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b939be1a16917d966978485a9a71e7b85c49562a3c586f5e4a1f29a4e37eea`  
		Last Modified: Thu, 07 Sep 2023 03:06:08 GMT  
		Size: 54.6 MB (54584978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd599095290ceb230904c5a49548b19f4ae5255d7574371101ff5971495c7a5`  
		Last Modified: Thu, 07 Sep 2023 03:06:40 GMT  
		Size: 196.8 MB (196840917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94d04c2a3871c9d786508f8f64518b0f9bbd8bfd75516a2b85e257eba330d68e`  
		Last Modified: Thu, 07 Sep 2023 11:30:58 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3a9b5b1adb8cd5b35f8803a6a573c168da2fb7f84cf59fbd893863dee4f4856`  
		Last Modified: Thu, 07 Sep 2023 11:31:01 GMT  
		Size: 15.6 MB (15635052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce6a9446f645f3bdae58e1e2f6db85d428f43c5cae782c749de903277a0e140`  
		Last Modified: Thu, 07 Sep 2023 11:30:58 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062c6e5e5f877962c450ed74e8993336846116844c3924658ba5ad06a26f1a1c`  
		Last Modified: Thu, 07 Sep 2023 15:14:22 GMT  
		Size: 7.3 MB (7260663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:972165de2ea7437da65fed3789f1817c9cd35d5c586d8e221d212e53b21c6955`  
		Last Modified: Thu, 07 Sep 2023 15:14:21 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac961ee60f9d364429e987bb83f604301dc65dc6a6609bbed394de9b2b44432c`  
		Last Modified: Thu, 07 Sep 2023 15:14:20 GMT  
		Size: 1.5 KB (1466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:perl` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:12df8e95660c1e8a46634355ea7b6b3a4f7b71ddb90404dba04de2ba09cb39b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.6 MB (336612573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39c8cf739973a071e36c71cdb5c7dbf5fb290750e6b2b68992f18ea535f4a2e8`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:45 GMT
ADD file:6bc001e951ef1280f566a92e65fcff57aefb8a280aa3510b7cd4b4e0a54c5cff in / 
# Thu, 07 Sep 2023 00:39:46 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:52:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 06:52:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 06:53:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 11:29:53 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 07 Sep 2023 11:29:53 GMT
WORKDIR /usr/src/perl
# Thu, 07 Sep 2023 11:34:04 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Thu, 07 Sep 2023 11:34:04 GMT
WORKDIR /usr/src/app
# Thu, 07 Sep 2023 11:34:04 GMT
CMD ["perl5.38.0" "-de0"]
# Thu, 07 Sep 2023 22:19:51 GMT
LABEL org.opencontainers.image.title=Unit (perl5.38)
# Thu, 07 Sep 2023 22:19:51 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Thu, 07 Sep 2023 22:19:51 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Thu, 07 Sep 2023 22:19:51 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Thu, 07 Sep 2023 22:19:51 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Thu, 07 Sep 2023 22:19:51 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Thu, 07 Sep 2023 22:19:51 GMT
LABEL org.opencontainers.image.version=1.31.0
# Thu, 07 Sep 2023 22:20:31 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure perl     && make -j $NCPU perl-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure perl     && make -j $NCPU perl-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Thu, 07 Sep 2023 22:20:31 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Thu, 07 Sep 2023 22:20:32 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Thu, 07 Sep 2023 22:20:32 GMT
STOPSIGNAL SIGTERM
# Thu, 07 Sep 2023 22:20:32 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 07 Sep 2023 22:20:32 GMT
EXPOSE 80
# Thu, 07 Sep 2023 22:20:32 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:61c16b7975697b00760ff9536c09eed29b6a76923d4d98be38e9cdc749506417`  
		Last Modified: Thu, 07 Sep 2023 00:43:21 GMT  
		Size: 53.7 MB (53704716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b3f92a99188e47f7b0b8d38aff11fd0ad90510e0d26506aec007d24fe539b6`  
		Last Modified: Thu, 07 Sep 2023 07:00:19 GMT  
		Size: 15.7 MB (15746623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbbd1eb48e6c614e3e3767ae9ba92cd3104dc0df1c1cf83b5211c232c4962473`  
		Last Modified: Thu, 07 Sep 2023 07:00:33 GMT  
		Size: 54.7 MB (54676071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb15cc2af1f50b1422bbad6cc66af59be680a2861f9d9c17db2b115a1db0256`  
		Last Modified: Thu, 07 Sep 2023 07:00:59 GMT  
		Size: 189.8 MB (189776733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc874db75fa4d842ee082eb3093d9e6e82f507fef25a931bb9cb2abbda2d2f9a`  
		Last Modified: Thu, 07 Sep 2023 12:59:55 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe16acf0d1905624754ec7370daf0b96b328f98d898bed2f10ef9658ce37334`  
		Last Modified: Thu, 07 Sep 2023 12:59:58 GMT  
		Size: 15.6 MB (15569647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed299b2fca35b4fbfae52eaf5cc937e9a669587751d42299ec67705f27fdeda`  
		Last Modified: Thu, 07 Sep 2023 12:59:55 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a7d6ce02881517b809e1f0d737113f4ec32200033e98b291eb83288e339449`  
		Last Modified: Thu, 07 Sep 2023 22:24:19 GMT  
		Size: 7.1 MB (7135721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ab90c33b1e7d7f064804876b6712c0ac20cc0e5b442953b38a2df397a15270`  
		Last Modified: Thu, 07 Sep 2023 22:24:18 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852bda3524612429eaadf06cbc5eba4009bcf0dca33c2036a80caea1fa649595`  
		Last Modified: Thu, 07 Sep 2023 22:24:18 GMT  
		Size: 1.5 KB (1467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
