## `unit:go1.20`

```console
$ docker pull unit@sha256:992a9f93793cae1560838c2fa384f4c17dddbcad5ac5998de97307455644d9ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:go1.20` - linux; amd64

```console
$ docker pull unit@sha256:af885c464915857fc8f2c3ca6216784c525d76827a396d6af508f6ee44b2c1a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **319.3 MB (319256892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:135578047dbf673b847a2eab62d71e7ab3f9d5bf384594bb9648f7edc30b6b9b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:57 GMT
ADD file:20f89ff93bfbd6c9fb1a97058a1f3de4485a8974e8a83892072c511fbd2e4134 in / 
# Wed, 16 Aug 2023 00:59:58 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 06:59:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 06:59:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 00:50:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 00:50:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:13 GMT
ENV GOLANG_VERSION=1.20.8
# Wed, 06 Sep 2023 18:32:22 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.8.linux-amd64.tar.gz'; 			sha256='cc97c28d9c252fbf28f91950d830201aa403836cbed702a05932e63f7f0c7bc4'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.8.linux-armv6l.tar.gz'; 			sha256='6fd6b0bd7861d8ff69d6f25b879c69cd25ee33b2cc52b6ed3a6c0d26368e0dcb'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.8.linux-arm64.tar.gz'; 			sha256='15ab379c6a2b0d086fe3e74be4599420e66549edf7426a300ee0f3809500f89e'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.8.linux-386.tar.gz'; 			sha256='d6e526520cf519049a854d7344b0a5fbe9675a3f24e7f22c44e38d8387ef942c'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.8.linux-ppc64le.tar.gz'; 			sha256='a5034a9c7eac6c5bcc650c2605c5edb4039c7b6064e2a2ea43c415c8af91f5f6'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.8.linux-s390x.tar.gz'; 			sha256='28261a277f4a724d3a3c56b50ca892ea762778a4b64b5e16b2b8a81faf523394'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.8.src.tar.gz'; 		sha256='38d71714fa5279f97240451956d8e47e3c1b6a5de7cb84137949d62b5dd3182e'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Wed, 06 Sep 2023 18:32:23 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:32:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:32:24 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:56:06 GMT
LABEL org.opencontainers.image.title=Unit (go1.20)
# Wed, 06 Sep 2023 18:56:06 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Wed, 06 Sep 2023 18:56:06 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Wed, 06 Sep 2023 18:56:06 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Wed, 06 Sep 2023 18:56:06 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Wed, 06 Sep 2023 18:56:06 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 06 Sep 2023 18:56:07 GMT
LABEL org.opencontainers.image.version=1.31.0
# Wed, 06 Sep 2023 18:56:56 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure go --go-path=$GOPATH     && make -j $NCPU go-install-src libunit-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure go --go-path=$GOPATH     && make -j $NCPU go-install-src libunit-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Wed, 06 Sep 2023 18:56:56 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Wed, 06 Sep 2023 18:56:56 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Wed, 06 Sep 2023 18:56:57 GMT
STOPSIGNAL SIGTERM
# Wed, 06 Sep 2023 18:56:57 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Wed, 06 Sep 2023 18:56:57 GMT
EXPOSE 80
# Wed, 06 Sep 2023 18:56:57 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
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
	-	`sha256:d4960566fad88b3b3a13610f36e9daf0fb2073f86a8377c10517fbe4bd0742a5`  
		Last Modified: Thu, 17 Aug 2023 00:52:21 GMT  
		Size: 86.0 MB (86031202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9c175b52c4b5ac69ce27cac8b67abc22ddfa4cc4be224634d1cc4671be77f94`  
		Last Modified: Wed, 06 Sep 2023 18:38:44 GMT  
		Size: 100.4 MB (100432011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ce8ad560f044231e8fb7e4a2290a1a70f56a612ed3de485ab5565b9d5fcf1c`  
		Last Modified: Wed, 06 Sep 2023 18:38:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:508b61a4d3c46c161f4c1b44f73d487aa910824512c50d61f631febc1b6ba27f`  
		Last Modified: Wed, 06 Sep 2023 18:58:03 GMT  
		Size: 7.4 MB (7388855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bec3f0858f8a2692ac7c5b457b8411ae862b177a839b7f517f38bd75cf1f35c`  
		Last Modified: Wed, 06 Sep 2023 18:58:02 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed92ebab2775969599e9c2fc614c945b2944742b855b526958fa6cd8ad274531`  
		Last Modified: Wed, 06 Sep 2023 18:58:02 GMT  
		Size: 1.5 KB (1467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:go1.20` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:e43d5a1123756abbfecc21320c0c7fb924ff7018907239b23ede6982d214ce2f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.6 MB (308573322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f081fcd70caec6ca53477192976b585a631c4e81f933cf4f433b31248453e5cb`
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
# Thu, 07 Sep 2023 11:03:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 11:03:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 11:04:00 GMT
ENV GOLANG_VERSION=1.20.8
# Thu, 07 Sep 2023 11:04:11 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.8.linux-amd64.tar.gz'; 			sha256='cc97c28d9c252fbf28f91950d830201aa403836cbed702a05932e63f7f0c7bc4'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.8.linux-armv6l.tar.gz'; 			sha256='6fd6b0bd7861d8ff69d6f25b879c69cd25ee33b2cc52b6ed3a6c0d26368e0dcb'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.8.linux-arm64.tar.gz'; 			sha256='15ab379c6a2b0d086fe3e74be4599420e66549edf7426a300ee0f3809500f89e'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.8.linux-386.tar.gz'; 			sha256='d6e526520cf519049a854d7344b0a5fbe9675a3f24e7f22c44e38d8387ef942c'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.8.linux-ppc64le.tar.gz'; 			sha256='a5034a9c7eac6c5bcc650c2605c5edb4039c7b6064e2a2ea43c415c8af91f5f6'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.8.linux-s390x.tar.gz'; 			sha256='28261a277f4a724d3a3c56b50ca892ea762778a4b64b5e16b2b8a81faf523394'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.8.src.tar.gz'; 		sha256='38d71714fa5279f97240451956d8e47e3c1b6a5de7cb84137949d62b5dd3182e'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Thu, 07 Sep 2023 11:04:12 GMT
ENV GOPATH=/go
# Thu, 07 Sep 2023 11:04:12 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 11:04:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 07 Sep 2023 11:04:13 GMT
WORKDIR /go
# Thu, 07 Sep 2023 22:17:06 GMT
LABEL org.opencontainers.image.title=Unit (go1.20)
# Thu, 07 Sep 2023 22:17:06 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Thu, 07 Sep 2023 22:17:06 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Thu, 07 Sep 2023 22:17:06 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Thu, 07 Sep 2023 22:17:06 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Thu, 07 Sep 2023 22:17:06 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Thu, 07 Sep 2023 22:17:06 GMT
LABEL org.opencontainers.image.version=1.31.0
# Thu, 07 Sep 2023 22:17:46 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure go --go-path=$GOPATH     && make -j $NCPU go-install-src libunit-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure go --go-path=$GOPATH     && make -j $NCPU go-install-src libunit-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Thu, 07 Sep 2023 22:17:47 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Thu, 07 Sep 2023 22:17:47 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Thu, 07 Sep 2023 22:17:47 GMT
STOPSIGNAL SIGTERM
# Thu, 07 Sep 2023 22:17:47 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 07 Sep 2023 22:17:47 GMT
EXPOSE 80
# Thu, 07 Sep 2023 22:17:47 GMT
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
	-	`sha256:175d1e52cc5a8a81fc3d30dfcf02306c41190283476954572b7406bdb77774ae`  
		Last Modified: Thu, 07 Sep 2023 11:05:12 GMT  
		Size: 81.5 MB (81467810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f8b4ad7da681336876dc73afa3ed6d6d4fbbd202436aa332f8276dd5f4f69c`  
		Last Modified: Thu, 07 Sep 2023 11:05:55 GMT  
		Size: 95.7 MB (95733923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac679ac5013621c2067f60aa8c2061d87e6243cdf7b382a72e9dabf49de73394`  
		Last Modified: Thu, 07 Sep 2023 11:05:45 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a691a694a6cec8a83a19181275fad414bf5c9e732cb90f7ff74e8cd85817f84e`  
		Last Modified: Thu, 07 Sep 2023 22:23:45 GMT  
		Size: 7.2 MB (7241282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606772289809cbe7457839668788999fdba8f94c92da44c06f47135e06a1d130`  
		Last Modified: Thu, 07 Sep 2023 22:23:44 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4496cb479a313e5489f243d5dc92273f23f45694473c59867c9440c4417dffa2`  
		Last Modified: Thu, 07 Sep 2023 22:23:44 GMT  
		Size: 1.5 KB (1466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
