## `unit:go1.20`

```console
$ docker pull unit@sha256:bce58343c50d6ca14838992ad043b9d357811d632ac52d33dcc547ec1a054e87
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `unit:go1.20` - linux; amd64

```console
$ docker pull unit@sha256:54d2139d4b2e9a048c6f49114ea81c5e452617e232ee3bff09875e03b4b0a536
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **319.1 MB (319100025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1386af8dc3f689bec80bd4828c32619152a0f5f4f9a20ce708eaf6447a8ba38d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Thu, 19 Oct 2023 10:47:22 GMT
ADD file:d3a2f1f42338ba7066e352cea3b7bf4c7576e6b96fef785e8da763114f337c0e in / 
# Thu, 19 Oct 2023 10:47:22 GMT
CMD ["bash"]
# Thu, 19 Oct 2023 10:47:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Oct 2023 10:47:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 19 Oct 2023 10:47:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Oct 2023 10:47:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Oct 2023 10:47:22 GMT
ENV GOLANG_VERSION=1.20.12
# Thu, 19 Oct 2023 10:47:22 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.12.linux-amd64.tar.gz'; 			sha256='9c5d48c54dd8b0a3b2ef91b0f92a1190aa01f11d26e98033efa64c46a30bba7b'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.12.linux-armv6l.tar.gz'; 			sha256='bf4687cbbf0c44a82311d52e2dcccb263f3d9c3b512007e1fae569e03dc0a189'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.12.linux-arm64.tar.gz'; 			sha256='8afe8e3fb6972eaa2179ef0a71678c67f26509fab4f0f67c4b00f4cdfa92dc87'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.12.linux-386.tar.gz'; 			sha256='77db17c6350448b0c3afa5c4248426d8a445b5e8ac2411fff57463b47f8d7f80'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.12.linux-ppc64le.tar.gz'; 			sha256='2ae0ec3736216dfbd7b01ff679842dc1bed365e53a024d522645bcffd01c7328'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.12.linux-s390x.tar.gz'; 			sha256='ee48b23e1978a866cb60a8e8ddf0bd61cbbaf86bcfcdbf4f9509f34e9159ce45'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.12.src.tar.gz'; 		sha256='c5bf934751d31c315c1d0bb5fb02296545fa6d08923566f7a5afec81f2ed27d6'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Thu, 19 Oct 2023 10:47:22 GMT
ENV GOPATH=/go
# Thu, 19 Oct 2023 10:47:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Oct 2023 10:47:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 19 Oct 2023 10:47:22 GMT
WORKDIR /go
# Thu, 19 Oct 2023 10:47:22 GMT
LABEL org.opencontainers.image.title=Unit (go1.20)
# Thu, 19 Oct 2023 10:47:22 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Thu, 19 Oct 2023 10:47:22 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Thu, 19 Oct 2023 10:47:22 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Thu, 19 Oct 2023 10:47:22 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Thu, 19 Oct 2023 10:47:22 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Thu, 19 Oct 2023 10:47:22 GMT
LABEL org.opencontainers.image.version=1.31.1
# Thu, 19 Oct 2023 10:47:22 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.1-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure go --go-path=$GOPATH     && make -j $NCPU go-install-src libunit-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure go --go-path=$GOPATH     && make -j $NCPU go-install-src libunit-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log # buildkit
# Thu, 19 Oct 2023 10:47:22 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 19 Oct 2023 10:47:22 GMT
COPY welcome.* /usr/share/unit/welcome/ # buildkit
# Thu, 19 Oct 2023 10:47:22 GMT
STOPSIGNAL SIGTERM
# Thu, 19 Oct 2023 10:47:22 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 19 Oct 2023 10:47:22 GMT
EXPOSE map[80/tcp:{}]
# Thu, 19 Oct 2023 10:47:22 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
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
	-	`sha256:32e75cdbd7a06f7dcf0e2c0d7c5949d141e3cf6880a29f9f85b2aeef46b56a48`  
		Last Modified: Tue, 19 Dec 2023 18:53:35 GMT  
		Size: 86.1 MB (86085949 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b06b18eb9f8d9c08705e9e0b7bb2c535ea5e3368862f76ee3c5ec2d14ce0f0f5`  
		Last Modified: Tue, 19 Dec 2023 18:54:24 GMT  
		Size: 100.4 MB (100426509 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7fd6e3cabff1265fae4d43541621aa8727899c8f7f560c456dc7f537564ca00f`  
		Last Modified: Tue, 19 Dec 2023 18:54:12 GMT  
		Size: 156.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:11f7add38c7ed10208f4bf031c80079cb584cca186f0d0704904ea89eb73701e`  
		Last Modified: Wed, 20 Dec 2023 20:17:55 GMT  
		Size: 7.2 MB (7167095 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b6af610311532b1529ca6457fabd71dcd4d6666179bac2aebc5dbc974bd1ff0`  
		Last Modified: Wed, 20 Dec 2023 20:17:54 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5b5fb28b126c3e924e6223fdc2dabbab19dff70c0b9926a1551ebae8acda18b7`  
		Last Modified: Wed, 20 Dec 2023 20:17:55 GMT  
		Size: 1.5 KB (1453 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `unit:go1.20` - unknown; unknown

```console
$ docker pull unit@sha256:babe7236068d29fa75e3638d4f19b2e743d57ffb3008f28beef2b4b35bb62fdb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8809773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afe5eb6443e38f4733bf6343595719f659c80e0153faa54d87aaafd8ecf9c393`

```dockerfile
```

-	Layers:
	-	`sha256:3be51e52effbb08f6237e44b43ee7d2956261dd3ac8b17ec36b9b524e5deb7cb`  
		Last Modified: Wed, 20 Dec 2023 20:17:54 GMT  
		Size: 8.8 MB (8785168 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:2d501f4e8360ceedea9b758759bdb388f9f83268c04bdc2f55d98a94039366f7`  
		Last Modified: Wed, 20 Dec 2023 20:17:54 GMT  
		Size: 24.6 KB (24605 bytes)  
		MIME: application/vnd.in-toto+json

### `unit:go1.20` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:45d6c627619937908664308ffef3fb202a744e144b26c49ccb587cca019771fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.4 MB (308411696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0285f2f5f9e5fd915021f0e87eb2f090e0bfd038a0e947b207ec36c4b83081aa`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Thu, 19 Oct 2023 10:47:22 GMT
ADD file:06ba7e39a2f8e1a7bcbb929fa9d1e6fb1f8bdcf5096dc903576af8f7014e353b in / 
# Thu, 19 Oct 2023 10:47:22 GMT
CMD ["bash"]
# Thu, 19 Oct 2023 10:47:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Oct 2023 10:47:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 19 Oct 2023 10:47:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Oct 2023 10:47:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Oct 2023 10:47:22 GMT
ENV GOLANG_VERSION=1.20.12
# Thu, 19 Oct 2023 10:47:22 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.12.linux-amd64.tar.gz'; 			sha256='9c5d48c54dd8b0a3b2ef91b0f92a1190aa01f11d26e98033efa64c46a30bba7b'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.12.linux-armv6l.tar.gz'; 			sha256='bf4687cbbf0c44a82311d52e2dcccb263f3d9c3b512007e1fae569e03dc0a189'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.12.linux-arm64.tar.gz'; 			sha256='8afe8e3fb6972eaa2179ef0a71678c67f26509fab4f0f67c4b00f4cdfa92dc87'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.12.linux-386.tar.gz'; 			sha256='77db17c6350448b0c3afa5c4248426d8a445b5e8ac2411fff57463b47f8d7f80'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.12.linux-ppc64le.tar.gz'; 			sha256='2ae0ec3736216dfbd7b01ff679842dc1bed365e53a024d522645bcffd01c7328'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.12.linux-s390x.tar.gz'; 			sha256='ee48b23e1978a866cb60a8e8ddf0bd61cbbaf86bcfcdbf4f9509f34e9159ce45'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.12.src.tar.gz'; 		sha256='c5bf934751d31c315c1d0bb5fb02296545fa6d08923566f7a5afec81f2ed27d6'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Thu, 19 Oct 2023 10:47:22 GMT
ENV GOPATH=/go
# Thu, 19 Oct 2023 10:47:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Oct 2023 10:47:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 19 Oct 2023 10:47:22 GMT
WORKDIR /go
# Thu, 19 Oct 2023 10:47:22 GMT
LABEL org.opencontainers.image.title=Unit (go1.20)
# Thu, 19 Oct 2023 10:47:22 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Thu, 19 Oct 2023 10:47:22 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Thu, 19 Oct 2023 10:47:22 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Thu, 19 Oct 2023 10:47:22 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Thu, 19 Oct 2023 10:47:22 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Thu, 19 Oct 2023 10:47:22 GMT
LABEL org.opencontainers.image.version=1.31.1
# Thu, 19 Oct 2023 10:47:22 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.1-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure go --go-path=$GOPATH     && make -j $NCPU go-install-src libunit-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure go --go-path=$GOPATH     && make -j $NCPU go-install-src libunit-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log # buildkit
# Thu, 19 Oct 2023 10:47:22 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 19 Oct 2023 10:47:22 GMT
COPY welcome.* /usr/share/unit/welcome/ # buildkit
# Thu, 19 Oct 2023 10:47:22 GMT
STOPSIGNAL SIGTERM
# Thu, 19 Oct 2023 10:47:22 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 19 Oct 2023 10:47:22 GMT
EXPOSE map[80/tcp:{}]
# Thu, 19 Oct 2023 10:47:22 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
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
	-	`sha256:9aea5ee0f94d038f071199297175350bfa92e575e220b1f772fbf67b942202c9`  
		Last Modified: Tue, 19 Dec 2023 20:03:39 GMT  
		Size: 81.5 MB (81486689 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:13d23ae01c572d4a99e3e31dc6fa0c10b3f6a25e1600b98cf151455988948375`  
		Last Modified: Tue, 19 Dec 2023 20:04:24 GMT  
		Size: 95.7 MB (95742160 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:42bd42e09f9c45574015f8c993df1e8c6c1a5b2777158b2abeaadf58ddc514c9`  
		Last Modified: Tue, 19 Dec 2023 20:04:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:db64bf73d0dd5bea635bc9bd4b984d7a30951318b90a0b514db10f479d2a6541`  
		Last Modified: Thu, 21 Dec 2023 06:32:00 GMT  
		Size: 7.0 MB (7021699 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:342704ca501fbc404b0310ca09b9a6b11047e04ab5ff88930175250921c512e3`  
		Last Modified: Thu, 21 Dec 2023 06:32:01 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2b7ed60eed63c1b55871f4962fc25d8f9c69b370cb209ce538cd66a3e9e8d87e`  
		Last Modified: Thu, 21 Dec 2023 06:32:01 GMT  
		Size: 1.5 KB (1453 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `unit:go1.20` - unknown; unknown

```console
$ docker pull unit@sha256:bf602b4f407a70814027e4d7b56c196585ebed42b9c0c24491ecc921e143bc1d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8811468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5034a36e4799ee2147807b9ed625c443f6af71d69105c44adce2a46ca14b7bf`

```dockerfile
```

-	Layers:
	-	`sha256:f9a36c62478e3bca5264e2a021b8faafee2f02d8dd1d8a032cdbb4b88237f37e`  
		Last Modified: Thu, 21 Dec 2023 06:32:00 GMT  
		Size: 8.8 MB (8786862 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:4731cfc0ee73113efde2c0a6c173ce28d34221bc1f72f0f6ab160db726ef1084`  
		Last Modified: Thu, 21 Dec 2023 06:31:59 GMT  
		Size: 24.6 KB (24606 bytes)  
		MIME: application/vnd.in-toto+json
