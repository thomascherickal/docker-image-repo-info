## `unit:go1.21`

```console
$ docker pull unit@sha256:ec98b35f34fb6ae82ef1a8aac1b47eabf501604fa136d2776d67e37cb1b88986
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 3
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8

### `unit:go1.21` - linux; amd64

```console
$ docker pull unit@sha256:cfd8b27e7b3bb2e07d7f67d031bbfa292fd9f53bc700bde4b757e64626cab107
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.7 MB (285656075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:284b23344860ec9ce899820b67fb23ad4293197a150c23172c563f6b7cdef505`
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
ENV GOLANG_VERSION=1.21.5
# Thu, 19 Oct 2023 10:47:22 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.5.linux-amd64.tar.gz'; 			sha256='e2bc0b3e4b64111ec117295c088bde5f00eeed1567999ff77bc859d7df70078e'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.5.linux-arm64.tar.gz'; 			sha256='841cced7ecda9b2014f139f5bab5ae31785f35399f236b8b3e75dff2a2978d96'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.5.linux-386.tar.gz'; 			sha256='8f4dba9cf5c61757bbd7e9ebdb93b6a30a1b03f4a636a1ba0cc2f27b907ab8e1'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.5.linux-mips64le.tar.gz'; 			sha256='0799ce6a33181d09d623551e108b8d48359ace39eef9dc935f3140618f844f12'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.5.linux-ppc64le.tar.gz'; 			sha256='907b8c6ec4be9b184952e5d3493be66b1746442394a8bc78556c56834cd7c38b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.5.linux-riscv64.tar.gz'; 			sha256='984d8f999f5019d15527a1a0e6b0c3ef879833e26dcd422ab0ef4d81ac486b96'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.5.linux-s390x.tar.gz'; 			sha256='9c4a81b72ebe44368813cd03684e1080a818bf915d84163abae2ed325a1b2dc0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		go version
# Thu, 19 Oct 2023 10:47:22 GMT
ENV GOTOOLCHAIN=local
# Thu, 19 Oct 2023 10:47:22 GMT
ENV GOPATH=/go
# Thu, 19 Oct 2023 10:47:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Oct 2023 10:47:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 19 Oct 2023 10:47:22 GMT
WORKDIR /go
# Thu, 19 Oct 2023 10:47:22 GMT
LABEL org.opencontainers.image.title=Unit (go1.21)
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
	-	`sha256:4445172115f2a9bb717578a2ef4e6197f05400bf770679bd8ba39acce10a0841`  
		Last Modified: Wed, 20 Dec 2023 20:26:08 GMT  
		Size: 67.0 MB (66982586 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e3ca2e15a2868f4118fbca9d8b94adacf9e5dfb007e81d9b2f39cec7d7c5c465`  
		Last Modified: Wed, 20 Dec 2023 20:25:57 GMT  
		Size: 154.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:74d4db59f2f198a30965d9d722c0b9f1f1c4527aff49042275bfc444639ebe32`  
		Last Modified: Wed, 20 Dec 2023 22:13:19 GMT  
		Size: 7.2 MB (7167072 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a68e94ec48d9d15d9391b3770a6d24977778bc58ee2a7106060350cefc806db1`  
		Last Modified: Wed, 20 Dec 2023 22:13:18 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eca9cc622ea9b7a8d6ffbd0e02a053cf02216d7fdae9bdefdd531ed179de74bf`  
		Last Modified: Wed, 20 Dec 2023 22:13:20 GMT  
		Size: 1.5 KB (1453 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `unit:go1.21` - unknown; unknown

```console
$ docker pull unit@sha256:0a699bebf7c6efd41d56001d3fba0669202d65111208188c7293e2ed4704749f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8809466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7752b70c4ebed67e584f0ecf81a505a0f5076c7356b927d5b2e173cfc02961e0`

```dockerfile
```

-	Layers:
	-	`sha256:785969f48e5b4c6fb00d2f8b7ebff0379037eed837a347806b30011ad0041b9a`  
		Last Modified: Wed, 20 Dec 2023 22:13:19 GMT  
		Size: 8.8 MB (8784273 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:235076435ba9a7f01af81708346c03d4147f75657d33f72620baeeb70206ffaa`  
		Last Modified: Wed, 20 Dec 2023 22:13:19 GMT  
		Size: 25.2 KB (25193 bytes)  
		MIME: application/vnd.in-toto+json

### `unit:go1.21` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:b124cd1c8dce7ed6e751fcc9dfa18b5d937f4a8d01f5a980bb807091444f3d26
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.0 MB (276966595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:745a16a9dec83e0fd623fb89b1ece5422b5146614f33af2debc8868dff05a1fe`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:17 GMT
ADD file:06ba7e39a2f8e1a7bcbb929fa9d1e6fb1f8bdcf5096dc903576af8f7014e353b in / 
# Tue, 19 Dec 2023 01:41:18 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 11:35:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 11:35:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 20:02:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 20:02:06 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 19 Dec 2023 20:02:06 GMT
ENV GOLANG_VERSION=1.21.5
# Wed, 20 Dec 2023 20:49:27 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.5.linux-amd64.tar.gz'; 			sha256='e2bc0b3e4b64111ec117295c088bde5f00eeed1567999ff77bc859d7df70078e'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.5.linux-arm64.tar.gz'; 			sha256='841cced7ecda9b2014f139f5bab5ae31785f35399f236b8b3e75dff2a2978d96'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.5.linux-386.tar.gz'; 			sha256='8f4dba9cf5c61757bbd7e9ebdb93b6a30a1b03f4a636a1ba0cc2f27b907ab8e1'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.5.linux-mips64le.tar.gz'; 			sha256='0799ce6a33181d09d623551e108b8d48359ace39eef9dc935f3140618f844f12'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.5.linux-ppc64le.tar.gz'; 			sha256='907b8c6ec4be9b184952e5d3493be66b1746442394a8bc78556c56834cd7c38b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.5.linux-riscv64.tar.gz'; 			sha256='984d8f999f5019d15527a1a0e6b0c3ef879833e26dcd422ab0ef4d81ac486b96'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.5.linux-s390x.tar.gz'; 			sha256='9c4a81b72ebe44368813cd03684e1080a818bf915d84163abae2ed325a1b2dc0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		go version
# Wed, 20 Dec 2023 20:49:28 GMT
ENV GOTOOLCHAIN=local
# Wed, 20 Dec 2023 20:49:28 GMT
ENV GOPATH=/go
# Wed, 20 Dec 2023 20:49:28 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Dec 2023 20:49:29 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 20 Dec 2023 20:49:29 GMT
WORKDIR /go
# Wed, 20 Dec 2023 21:18:02 GMT
LABEL org.opencontainers.image.title=Unit (go1.21)
# Wed, 20 Dec 2023 21:18:02 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Wed, 20 Dec 2023 21:18:02 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Wed, 20 Dec 2023 21:18:02 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Wed, 20 Dec 2023 21:18:02 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Wed, 20 Dec 2023 21:18:03 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 20 Dec 2023 21:18:03 GMT
LABEL org.opencontainers.image.version=1.31.1
# Wed, 20 Dec 2023 21:18:44 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.1-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure go --go-path=$GOPATH     && make -j $NCPU go-install-src libunit-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure go --go-path=$GOPATH     && make -j $NCPU go-install-src libunit-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Wed, 20 Dec 2023 21:18:44 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Wed, 20 Dec 2023 21:18:44 GMT
COPY multi:44b909b4ee0b15a0820a0f95f866a48ec9fbcb6e3c46d6d937842c09126ebe93 in /usr/share/unit/welcome/ 
# Wed, 20 Dec 2023 21:18:44 GMT
STOPSIGNAL SIGTERM
# Wed, 20 Dec 2023 21:18:45 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Wed, 20 Dec 2023 21:18:45 GMT
EXPOSE 80
# Wed, 20 Dec 2023 21:18:45 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
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
	-	`sha256:9aea5ee0f94d038f071199297175350bfa92e575e220b1f772fbf67b942202c9`  
		Last Modified: Tue, 19 Dec 2023 20:03:39 GMT  
		Size: 81.5 MB (81486689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b4c2556a812a669d93be0071f6ef4ed4f57545a3dac041872777d5a2d7f13b6`  
		Last Modified: Wed, 20 Dec 2023 20:52:15 GMT  
		Size: 64.1 MB (64072142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba193e4737ffb5f026c89050f401d39b37c071f72dbacdf683177bdd3944063`  
		Last Modified: Wed, 20 Dec 2023 20:52:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:175edc7d65a7f812551317d81e681b4af515a23b32936d1149eaeaf8df7bcfb9`  
		Last Modified: Wed, 20 Dec 2023 21:19:28 GMT  
		Size: 7.2 MB (7246590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6024bd03490ece0fb375abb9b4a28d371c5c0ebd7e1986d28a7eeb6701e9f9a3`  
		Last Modified: Wed, 20 Dec 2023 21:19:26 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d6653040e5218a268dd1dda9ae04fa2750de3a9f468cdceed14fa573a6604b0`  
		Last Modified: Wed, 20 Dec 2023 21:19:26 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
