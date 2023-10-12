<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `unit`

-	[`unit:1.31.0-go1.20`](#unit1310-go120)
-	[`unit:1.31.0-go1.21`](#unit1310-go121)
-	[`unit:1.31.0-jsc11`](#unit1310-jsc11)
-	[`unit:1.31.0-minimal`](#unit1310-minimal)
-	[`unit:1.31.0-node18`](#unit1310-node18)
-	[`unit:1.31.0-node20`](#unit1310-node20)
-	[`unit:1.31.0-perl5.36`](#unit1310-perl536)
-	[`unit:1.31.0-perl5.38`](#unit1310-perl538)
-	[`unit:1.31.0-php8.2`](#unit1310-php82)
-	[`unit:1.31.0-python3.11`](#unit1310-python311)
-	[`unit:1.31.0-ruby3.2`](#unit1310-ruby32)
-	[`unit:1.31.0-wasm`](#unit1310-wasm)
-	[`unit:go`](#unitgo)
-	[`unit:go1`](#unitgo1)
-	[`unit:go1.20`](#unitgo120)
-	[`unit:go1.21`](#unitgo121)
-	[`unit:jsc`](#unitjsc)
-	[`unit:jsc11`](#unitjsc11)
-	[`unit:latest`](#unitlatest)
-	[`unit:minimal`](#unitminimal)
-	[`unit:node`](#unitnode)
-	[`unit:node18`](#unitnode18)
-	[`unit:node20`](#unitnode20)
-	[`unit:perl`](#unitperl)
-	[`unit:perl5`](#unitperl5)
-	[`unit:perl5.36`](#unitperl536)
-	[`unit:perl5.38`](#unitperl538)
-	[`unit:php`](#unitphp)
-	[`unit:php8`](#unitphp8)
-	[`unit:php8.2`](#unitphp82)
-	[`unit:python`](#unitpython)
-	[`unit:python3`](#unitpython3)
-	[`unit:python3.11`](#unitpython311)
-	[`unit:ruby`](#unitruby)
-	[`unit:ruby3`](#unitruby3)
-	[`unit:ruby3.2`](#unitruby32)
-	[`unit:wasm`](#unitwasm)

## `unit:1.31.0-go1.20`

```console
$ docker pull unit@sha256:983ac481c876d9a3dbff95fefbffeb722e8c673f91fc6fdaea65f470cbda7227
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:1.31.0-go1.20` - linux; amd64

```console
$ docker pull unit@sha256:95eede34f128ca4a9c7e330a06d5b4b715d5db4efcdf34b09918aea5fdb99fd7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.3 MB (333278660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a816302fbfc02ecd48d477a933362a0443cb9952a0e46e29c844e409dbe2583`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 04:55:51 GMT
ADD file:85db4f4c5016f51f7112a5d09cb7d4620f565a1379ae4b8a03c5ffc23886a876 in / 
# Wed, 20 Sep 2023 04:55:51 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:22:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:22:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 03:29:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 03:29:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:20:57 GMT
ENV GOLANG_VERSION=1.20.10
# Tue, 10 Oct 2023 19:21:08 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.10.linux-amd64.tar.gz'; 			sha256='80d34f1fd74e382d86c2d6102e0e60d4318461a7c2f457ec1efc4042752d4248'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.10.linux-armv6l.tar.gz'; 			sha256='a2229772434dee3dde1e974ef5ae7936160a05a1b82c57cc5c64660479aa98cb'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.10.linux-arm64.tar.gz'; 			sha256='fb3c7e15fc4413c5b81eb9f26dbd7cd4faedd5c720b30fa8e2ff77457f74cab6'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.10.linux-386.tar.gz'; 			sha256='3c918225d22ef5731b63f0426e48614fc05d8da120fc23101639c81ab152e133'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.10.linux-ppc64le.tar.gz'; 			sha256='ebac6e713810174f9ffd7f48c17c373fbf359d50d8e6233b1dfbbdebd524fd1c'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.10.linux-s390x.tar.gz'; 			sha256='fa32588cbdd1e8adfd7e9f1b4ba3f7a8b424f60e90bf2cc4716650374eb459ae'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.10.src.tar.gz'; 		sha256='72d2f51805c47150066c103754c75fddb2c19d48c9219fa33d1e46696c841dbb'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 10 Oct 2023 19:21:09 GMT
ENV GOPATH=/go
# Tue, 10 Oct 2023 19:21:09 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:21:09 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 10 Oct 2023 19:21:09 GMT
WORKDIR /go
# Tue, 10 Oct 2023 19:46:10 GMT
LABEL org.opencontainers.image.title=Unit (go1.20)
# Tue, 10 Oct 2023 19:46:10 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Tue, 10 Oct 2023 19:46:10 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Tue, 10 Oct 2023 19:46:10 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Tue, 10 Oct 2023 19:46:10 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Tue, 10 Oct 2023 19:46:10 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 10 Oct 2023 19:46:10 GMT
LABEL org.opencontainers.image.version=1.31.0
# Tue, 10 Oct 2023 19:47:05 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure go --go-path=$GOPATH     && make -j $NCPU go-install-src libunit-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure go --go-path=$GOPATH     && make -j $NCPU go-install-src libunit-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Tue, 10 Oct 2023 19:47:06 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Tue, 10 Oct 2023 19:47:06 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Tue, 10 Oct 2023 19:47:06 GMT
STOPSIGNAL SIGTERM
# Tue, 10 Oct 2023 19:47:06 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 10 Oct 2023 19:47:06 GMT
EXPOSE 80
# Tue, 10 Oct 2023 19:47:06 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:ddf874abf16cc990e0fd75a154a34ca0a03ee310ad895a18fb62ae15bf4171fb`  
		Last Modified: Wed, 20 Sep 2023 05:00:41 GMT  
		Size: 55.1 MB (55056714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1459d3ab8b5e46ac1a0a00134fe2f7b693474eb6d75ace97ecbe811a6f5b0e`  
		Last Modified: Wed, 20 Sep 2023 09:31:06 GMT  
		Size: 15.8 MB (15760408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab00e7798a04602c3f6e2dc445a994d75e96c45533cd44701f58509982a8c5`  
		Last Modified: Wed, 20 Sep 2023 09:31:23 GMT  
		Size: 54.6 MB (54584790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9036a471a1c45233bf72245ae53bd00fd2b25cbdf75be2cafe1c6fd91309cdb7`  
		Last Modified: Thu, 21 Sep 2023 03:31:14 GMT  
		Size: 86.1 MB (86068436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f860905235a993930bdd0d7418c0d8e87db9d0182e1aefaec8e37c0787579b`  
		Last Modified: Tue, 10 Oct 2023 19:27:37 GMT  
		Size: 100.4 MB (100433184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512a1d11f639f8a1ba9b7b87e551e39cbe3f2824bf2ed122a68981d6815e1a14`  
		Last Modified: Tue, 10 Oct 2023 19:27:24 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16efabcc1bbb8acc14957b20306cfc6b40cef3c4d63ccebfb4a9f800ced9a0b3`  
		Last Modified: Tue, 10 Oct 2023 19:48:25 GMT  
		Size: 21.4 MB (21372238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8c3847df07c19e00cc8dc749aee71a4d25c04ddda1880dfe6360b4418e1414c`  
		Last Modified: Tue, 10 Oct 2023 19:48:22 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:829580fa0a5a52a282d59cef9ad292ea6a107820f172e25f062e3143bdf36e1c`  
		Last Modified: Tue, 10 Oct 2023 19:48:22 GMT  
		Size: 1.5 KB (1466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:1.31.0-go1.20` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:b2b4fe008079d4f71bc2b8b3512ef693dcae1bdd8e6e24425f83632e2d78093d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **320.9 MB (320912278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a492b7d2f297049e2304bdf15362502f4e27365895ff9aad1b92b7e4d852a2fe`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:20 GMT
ADD file:46dcdcde338d2c01fed5db3fac9041736d9305145d8fc2039dd5b3714d38ede8 in / 
# Wed, 20 Sep 2023 02:44:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:24:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:25:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 22:20:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 22:20:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:40:40 GMT
ENV GOLANG_VERSION=1.20.10
# Tue, 10 Oct 2023 19:40:48 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.10.linux-amd64.tar.gz'; 			sha256='80d34f1fd74e382d86c2d6102e0e60d4318461a7c2f457ec1efc4042752d4248'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.10.linux-armv6l.tar.gz'; 			sha256='a2229772434dee3dde1e974ef5ae7936160a05a1b82c57cc5c64660479aa98cb'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.10.linux-arm64.tar.gz'; 			sha256='fb3c7e15fc4413c5b81eb9f26dbd7cd4faedd5c720b30fa8e2ff77457f74cab6'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.10.linux-386.tar.gz'; 			sha256='3c918225d22ef5731b63f0426e48614fc05d8da120fc23101639c81ab152e133'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.10.linux-ppc64le.tar.gz'; 			sha256='ebac6e713810174f9ffd7f48c17c373fbf359d50d8e6233b1dfbbdebd524fd1c'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.10.linux-s390x.tar.gz'; 			sha256='fa32588cbdd1e8adfd7e9f1b4ba3f7a8b424f60e90bf2cc4716650374eb459ae'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.10.src.tar.gz'; 		sha256='72d2f51805c47150066c103754c75fddb2c19d48c9219fa33d1e46696c841dbb'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 10 Oct 2023 19:40:50 GMT
ENV GOPATH=/go
# Tue, 10 Oct 2023 19:40:50 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:40:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 10 Oct 2023 19:40:50 GMT
WORKDIR /go
# Tue, 10 Oct 2023 20:03:23 GMT
LABEL org.opencontainers.image.title=Unit (go1.20)
# Tue, 10 Oct 2023 20:03:23 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Tue, 10 Oct 2023 20:03:23 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Tue, 10 Oct 2023 20:03:23 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Tue, 10 Oct 2023 20:03:23 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Tue, 10 Oct 2023 20:03:23 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 10 Oct 2023 20:03:23 GMT
LABEL org.opencontainers.image.version=1.31.0
# Tue, 10 Oct 2023 20:04:09 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure go --go-path=$GOPATH     && make -j $NCPU go-install-src libunit-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure go --go-path=$GOPATH     && make -j $NCPU go-install-src libunit-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Tue, 10 Oct 2023 20:04:09 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Tue, 10 Oct 2023 20:04:09 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Tue, 10 Oct 2023 20:04:10 GMT
STOPSIGNAL SIGTERM
# Tue, 10 Oct 2023 20:04:10 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 10 Oct 2023 20:04:10 GMT
EXPOSE 80
# Tue, 10 Oct 2023 20:04:10 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:31f5dc1f52c865588c43d8ec718f14d430e149b28f0b28232da825da7ae28f76`  
		Last Modified: Wed, 20 Sep 2023 02:47:53 GMT  
		Size: 53.7 MB (53704892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb60045eb75c62e890b95d28e4893132a6c7d61ec9979104ee4ff6e86c4badee`  
		Last Modified: Wed, 20 Sep 2023 09:33:11 GMT  
		Size: 15.7 MB (15746671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292737ab468ef80c6f78bdde4896157b8953d1e5556e1e526f40aeadcb547573`  
		Last Modified: Wed, 20 Sep 2023 09:33:26 GMT  
		Size: 54.7 MB (54676309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486d7167072fd25b2d2370fbba8326b8059274be0fa615a14d3e975fe46f1b4f`  
		Last Modified: Wed, 20 Sep 2023 22:21:57 GMT  
		Size: 81.5 MB (81468116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3620a3068a7e100c04f3a92008ab8fb7b5657d5a6df928e4df656cd7dc0c68`  
		Last Modified: Tue, 10 Oct 2023 19:46:15 GMT  
		Size: 95.7 MB (95742099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9fd2acf33b2386df69b659928d770708cc4733475aeb32c8e4f7401ece635f`  
		Last Modified: Tue, 10 Oct 2023 19:46:06 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327f70c6c88438458daaa74f214545f1fd4c8444e75c852f0251f82ecd3c534f`  
		Last Modified: Tue, 10 Oct 2023 20:05:17 GMT  
		Size: 19.6 MB (19571295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abadc26450eb0c18e9a42145d965b482edc4c4f1e24326ca00b8d51123457fae`  
		Last Modified: Tue, 10 Oct 2023 20:05:15 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdd7b8611cb2380a77472b6ca3da0f6e4893829857f497f8d58313fded8fbdbd`  
		Last Modified: Tue, 10 Oct 2023 20:05:15 GMT  
		Size: 1.5 KB (1468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `unit:1.31.0-go1.21`

```console
$ docker pull unit@sha256:b9c9ddcce8c48adfce8f29648cdc7739cc01f07d86354fd751cb8728bc521186
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:1.31.0-go1.21` - linux; amd64

```console
$ docker pull unit@sha256:e25c525607700cb9afff5bf7ba2516c4af8a99eb8c374d614b52840ab4d2012a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.8 MB (299846746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0fba295b6f441f9cc6a84818fd1d58b0c3a5345fc0684fd72ab87fac731bc9f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 04:55:51 GMT
ADD file:85db4f4c5016f51f7112a5d09cb7d4620f565a1379ae4b8a03c5ffc23886a876 in / 
# Wed, 20 Sep 2023 04:55:51 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:22:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:22:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 03:29:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 03:29:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:19:57 GMT
ENV GOLANG_VERSION=1.21.3
# Tue, 10 Oct 2023 19:20:06 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.3.linux-mips64le.tar.gz'; 			sha256='a569ffbc88b4e14cf2682f65cec950460665e4392b0d78b8868b4718c979bda8'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 10 Oct 2023 19:20:07 GMT
ENV GOTOOLCHAIN=local
# Tue, 10 Oct 2023 19:20:07 GMT
ENV GOPATH=/go
# Tue, 10 Oct 2023 19:20:07 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:20:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 10 Oct 2023 19:20:07 GMT
WORKDIR /go
# Tue, 10 Oct 2023 19:45:00 GMT
LABEL org.opencontainers.image.title=Unit (go1.21)
# Tue, 10 Oct 2023 19:45:00 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Tue, 10 Oct 2023 19:45:00 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Tue, 10 Oct 2023 19:45:00 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Tue, 10 Oct 2023 19:45:00 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Tue, 10 Oct 2023 19:45:00 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 10 Oct 2023 19:45:00 GMT
LABEL org.opencontainers.image.version=1.31.0
# Tue, 10 Oct 2023 19:45:58 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure go --go-path=$GOPATH     && make -j $NCPU go-install-src libunit-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure go --go-path=$GOPATH     && make -j $NCPU go-install-src libunit-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Tue, 10 Oct 2023 19:45:59 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Tue, 10 Oct 2023 19:45:59 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Tue, 10 Oct 2023 19:45:59 GMT
STOPSIGNAL SIGTERM
# Tue, 10 Oct 2023 19:45:59 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 10 Oct 2023 19:45:59 GMT
EXPOSE 80
# Tue, 10 Oct 2023 19:45:59 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:ddf874abf16cc990e0fd75a154a34ca0a03ee310ad895a18fb62ae15bf4171fb`  
		Last Modified: Wed, 20 Sep 2023 05:00:41 GMT  
		Size: 55.1 MB (55056714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1459d3ab8b5e46ac1a0a00134fe2f7b693474eb6d75ace97ecbe811a6f5b0e`  
		Last Modified: Wed, 20 Sep 2023 09:31:06 GMT  
		Size: 15.8 MB (15760408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab00e7798a04602c3f6e2dc445a994d75e96c45533cd44701f58509982a8c5`  
		Last Modified: Wed, 20 Sep 2023 09:31:23 GMT  
		Size: 54.6 MB (54584790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9036a471a1c45233bf72245ae53bd00fd2b25cbdf75be2cafe1c6fd91309cdb7`  
		Last Modified: Thu, 21 Sep 2023 03:31:14 GMT  
		Size: 86.1 MB (86068436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a30056caa3534c4f704e37958c32100b96aa5535fff9af405b5bf4cd272e158`  
		Last Modified: Tue, 10 Oct 2023 19:25:53 GMT  
		Size: 67.0 MB (67001246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca402200ac32a0f6d38fdcae01d58d804e90543fabef314c0aaa4731ac3f9b6`  
		Last Modified: Tue, 10 Oct 2023 19:25:42 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62756cd2c6f084fd53a983f51ef7d6c5b3d9ef2f80d2fc122550940332ad324`  
		Last Modified: Tue, 10 Oct 2023 19:48:08 GMT  
		Size: 21.4 MB (21372254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13a00f1dc20f8f2006ac8c9b1c91c322d352fd41f2b3a41e00fb8bba12e3534`  
		Last Modified: Tue, 10 Oct 2023 19:48:05 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533fb155fbc122a1435f260e62b8f43d7de9a2c0675df5ecf4b5bc1a6f4d93ed`  
		Last Modified: Tue, 10 Oct 2023 19:48:05 GMT  
		Size: 1.5 KB (1470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:1.31.0-go1.21` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:8a3b8f2b9a104a7bab667ab4a73ad407817aab9ec14cb264a3e2df2814cf8b6a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289268520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9020087609178de15b4aea74b2bfc5530c392b2d08c4661713cdad84547c7415`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:20 GMT
ADD file:46dcdcde338d2c01fed5db3fac9041736d9305145d8fc2039dd5b3714d38ede8 in / 
# Wed, 20 Sep 2023 02:44:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:24:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:25:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 22:20:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 22:20:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:39:44 GMT
ENV GOLANG_VERSION=1.21.3
# Tue, 10 Oct 2023 19:39:52 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.3.linux-mips64le.tar.gz'; 			sha256='a569ffbc88b4e14cf2682f65cec950460665e4392b0d78b8868b4718c979bda8'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 10 Oct 2023 19:39:53 GMT
ENV GOTOOLCHAIN=local
# Tue, 10 Oct 2023 19:39:54 GMT
ENV GOPATH=/go
# Tue, 10 Oct 2023 19:39:54 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:39:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 10 Oct 2023 19:39:54 GMT
WORKDIR /go
# Tue, 10 Oct 2023 20:02:25 GMT
LABEL org.opencontainers.image.title=Unit (go1.21)
# Tue, 10 Oct 2023 20:02:25 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Tue, 10 Oct 2023 20:02:25 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Tue, 10 Oct 2023 20:02:25 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Tue, 10 Oct 2023 20:02:26 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Tue, 10 Oct 2023 20:02:26 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 10 Oct 2023 20:02:26 GMT
LABEL org.opencontainers.image.version=1.31.0
# Tue, 10 Oct 2023 20:03:13 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure go --go-path=$GOPATH     && make -j $NCPU go-install-src libunit-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure go --go-path=$GOPATH     && make -j $NCPU go-install-src libunit-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Tue, 10 Oct 2023 20:03:13 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Tue, 10 Oct 2023 20:03:13 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Tue, 10 Oct 2023 20:03:13 GMT
STOPSIGNAL SIGTERM
# Tue, 10 Oct 2023 20:03:13 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 10 Oct 2023 20:03:13 GMT
EXPOSE 80
# Tue, 10 Oct 2023 20:03:14 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:31f5dc1f52c865588c43d8ec718f14d430e149b28f0b28232da825da7ae28f76`  
		Last Modified: Wed, 20 Sep 2023 02:47:53 GMT  
		Size: 53.7 MB (53704892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb60045eb75c62e890b95d28e4893132a6c7d61ec9979104ee4ff6e86c4badee`  
		Last Modified: Wed, 20 Sep 2023 09:33:11 GMT  
		Size: 15.7 MB (15746671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292737ab468ef80c6f78bdde4896157b8953d1e5556e1e526f40aeadcb547573`  
		Last Modified: Wed, 20 Sep 2023 09:33:26 GMT  
		Size: 54.7 MB (54676309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486d7167072fd25b2d2370fbba8326b8059274be0fa615a14d3e975fe46f1b4f`  
		Last Modified: Wed, 20 Sep 2023 22:21:57 GMT  
		Size: 81.5 MB (81468116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1306584d039cecaec0b207b88108f8c03ec361f1cf8015ae4ba23ec3c9406f50`  
		Last Modified: Tue, 10 Oct 2023 19:44:41 GMT  
		Size: 64.1 MB (64098318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815863143577abf9b2b650b8a28f205bfc32287c17ee2b8c0e8a8155b2a75ca3`  
		Last Modified: Tue, 10 Oct 2023 19:44:28 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd1b8471a82b8fb80921156f2b1abe4b85e1db1756650baa8a63c94cdb72a9ac`  
		Last Modified: Tue, 10 Oct 2023 20:05:01 GMT  
		Size: 19.6 MB (19571320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e45a03b84b12daccf9bbc14746f689f1d235d2526a77c4fa8e26e9e97ca6ff0`  
		Last Modified: Tue, 10 Oct 2023 20:04:58 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc16a37f4406cdb2846b682b8e11e00ea46efd01c2826567faa97e87146f0f20`  
		Last Modified: Tue, 10 Oct 2023 20:04:58 GMT  
		Size: 1.5 KB (1467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `unit:1.31.0-jsc11`

```console
$ docker pull unit@sha256:e50d9d241fa875598b3297e8ec201d7dff76133c2175e38a250e5784be524c1b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:1.31.0-jsc11` - linux; amd64

```console
$ docker pull unit@sha256:6016dbebad214783b916db5de81e16e7d24981a202b3259f0597a06e447d8f56
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.6 MB (202620873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:381ecba965946dd28e8467f802d866b567b6ac1f78b91a8a7cdafc202dd5c9a1`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Mon, 25 Sep 2023 10:17:05 GMT
ARG RELEASE
# Mon, 25 Sep 2023 10:17:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 25 Sep 2023 10:17:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 25 Sep 2023 10:17:05 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 25 Sep 2023 10:17:07 GMT
ADD file:194c886b88876c1804cc5f80719669653c16a388b664147b7f22402105f533c4 in / 
# Mon, 25 Sep 2023 10:17:08 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 05:11:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 03 Oct 2023 05:11:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 05:11:45 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 03 Oct 2023 05:12:00 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 05:12:35 GMT
ENV JAVA_VERSION=jdk-11.0.20.1+1
# Tue, 03 Oct 2023 05:12:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69d39682c4a2fac294a9eaacbf62c26d3c8a2f9123f1b5d287498a5472c6b672';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        armhf|arm)          ESUM='e83674aee238ebb5f359b9395b3c5e3fad5b645846095494662802d2f0fd01c9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_arm_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='b806f4bb526161bf9b2ffb37be4e1b77f56b4e726dc4d52c7902130a79e7d710';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='a7efbe804a4616d38b6ac0def40cd9feacc04aee2bb89132191f4d33fc0a7c1e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='398a64bff002f0e3b0c01ecd24a1a32c83cb72a5255344219e9757d4ddd9f857';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_x64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 03 Oct 2023 05:12:46 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 03 Oct 2023 05:12:46 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Tue, 03 Oct 2023 05:12:46 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Tue, 03 Oct 2023 05:12:46 GMT
CMD ["jshell"]
# Tue, 03 Oct 2023 09:52:09 GMT
LABEL org.opencontainers.image.title=Unit (jsc11)
# Tue, 03 Oct 2023 09:52:09 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Tue, 03 Oct 2023 09:52:09 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Tue, 03 Oct 2023 09:52:10 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Tue, 03 Oct 2023 09:52:10 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Tue, 03 Oct 2023 09:52:10 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 03 Oct 2023 09:52:10 GMT
LABEL org.opencontainers.image.version=1.31.0
# Tue, 03 Oct 2023 09:54:28 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure java --jars=/usr/share/unit-jsc-common/     && make -j $NCPU java-shared-install java-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure java --jars=/usr/share/unit-jsc-common/     && make -j $NCPU java-shared-install java-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && rm -rf /root/.m2     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Tue, 03 Oct 2023 09:54:28 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Tue, 03 Oct 2023 09:54:28 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Tue, 03 Oct 2023 09:54:28 GMT
STOPSIGNAL SIGTERM
# Tue, 03 Oct 2023 09:54:28 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 03 Oct 2023 09:54:28 GMT
EXPOSE 80
# Tue, 03 Oct 2023 09:54:28 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:707e32e9fc569fee476af9e92ae3d1df8b8e6dca47f9cb31db9d2c922a6de952`  
		Last Modified: Mon, 25 Sep 2023 12:54:05 GMT  
		Size: 30.4 MB (30440869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320d7b4a8f0a0932d6c981aa21a5793fb50fc408278be946023a29cdbe81594b`  
		Last Modified: Tue, 03 Oct 2023 05:16:04 GMT  
		Size: 12.9 MB (12902712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1198a528604fdd5b16e909383ab8d985b7cbc003c05ba6d441388bae6d5c79ea`  
		Last Modified: Tue, 03 Oct 2023 05:16:58 GMT  
		Size: 144.8 MB (144836065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5d4fd9d99dab5a8bf810d560d314fd9b72f50c074b510bc3699f524f1cd9b2`  
		Last Modified: Tue, 03 Oct 2023 05:16:47 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50cc5b9dc759b6d18830d982e59eb599ec2af11c6fdd227f0bbbe3954b2357be`  
		Last Modified: Tue, 03 Oct 2023 05:16:47 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b5ff4a0275694dfa99bab3a081be450836129cd75e6637e0722a6f476a10aed`  
		Last Modified: Tue, 03 Oct 2023 09:55:15 GMT  
		Size: 14.4 MB (14437584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8073bea624df40f4799f22f93c9a7f1be90fba7f0cd4c457d49db820287f75f`  
		Last Modified: Tue, 03 Oct 2023 09:55:13 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72af9c810665ef90c9790f16cabe13c6b839bc15a10a80fb75403e5dda76934e`  
		Last Modified: Tue, 03 Oct 2023 09:55:13 GMT  
		Size: 1.5 KB (1468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:1.31.0-jsc11` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:ead51b31b9489fef27235b9da252b28ac0ff5f0e2502d384e4b698cb94b2edb1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.2 MB (197194795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ec37f60f6e40f250b3b060a062b9adb7f5522757c2d35b5e71a6b813761c883`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Mon, 25 Sep 2023 10:17:41 GMT
ARG RELEASE
# Mon, 25 Sep 2023 10:17:41 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 25 Sep 2023 10:17:41 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 25 Sep 2023 10:17:41 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 25 Sep 2023 10:17:44 GMT
ADD file:8540670760767f19eaf101fbce1da1881a2f24a7d65da6abdedc644b8fb00463 in / 
# Mon, 25 Sep 2023 10:17:45 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 06:06:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 03 Oct 2023 06:06:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 06:06:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 03 Oct 2023 06:07:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 06:07:36 GMT
ENV JAVA_VERSION=jdk-11.0.20.1+1
# Tue, 03 Oct 2023 06:07:45 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69d39682c4a2fac294a9eaacbf62c26d3c8a2f9123f1b5d287498a5472c6b672';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        armhf|arm)          ESUM='e83674aee238ebb5f359b9395b3c5e3fad5b645846095494662802d2f0fd01c9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_arm_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='b806f4bb526161bf9b2ffb37be4e1b77f56b4e726dc4d52c7902130a79e7d710';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='a7efbe804a4616d38b6ac0def40cd9feacc04aee2bb89132191f4d33fc0a7c1e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='398a64bff002f0e3b0c01ecd24a1a32c83cb72a5255344219e9757d4ddd9f857';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_x64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 03 Oct 2023 06:07:48 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 03 Oct 2023 06:07:48 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Tue, 03 Oct 2023 06:07:48 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Tue, 03 Oct 2023 06:07:48 GMT
CMD ["jshell"]
# Tue, 03 Oct 2023 07:15:07 GMT
LABEL org.opencontainers.image.title=Unit (jsc11)
# Tue, 03 Oct 2023 07:15:07 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Tue, 03 Oct 2023 07:15:07 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Tue, 03 Oct 2023 07:15:07 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Tue, 03 Oct 2023 07:15:07 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Tue, 03 Oct 2023 07:15:07 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 03 Oct 2023 07:15:07 GMT
LABEL org.opencontainers.image.version=1.31.0
# Tue, 03 Oct 2023 07:16:47 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure java --jars=/usr/share/unit-jsc-common/     && make -j $NCPU java-shared-install java-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure java --jars=/usr/share/unit-jsc-common/     && make -j $NCPU java-shared-install java-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && rm -rf /root/.m2     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Tue, 03 Oct 2023 07:16:47 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Tue, 03 Oct 2023 07:16:47 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Tue, 03 Oct 2023 07:16:47 GMT
STOPSIGNAL SIGTERM
# Tue, 03 Oct 2023 07:16:47 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 03 Oct 2023 07:16:47 GMT
EXPOSE 80
# Tue, 03 Oct 2023 07:16:47 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:6ea603f1df5e3d23206761eca19fba4cdf4e22d773256cb65b71b730aa5acced`  
		Last Modified: Mon, 25 Sep 2023 17:30:11 GMT  
		Size: 28.4 MB (28392073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db904450c39fc4ef39317a37a19b15df4a74bf6bb91100343e382470ce034d79`  
		Last Modified: Tue, 03 Oct 2023 06:10:10 GMT  
		Size: 12.8 MB (12843603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b47fc5d37efc4608b1cbe274678274c4b0b13ffba61a009da323e825c70dcd`  
		Last Modified: Tue, 03 Oct 2023 06:10:57 GMT  
		Size: 141.6 MB (141581350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de85af6ca814ebce4fe8e3c07e7d5e2099f636f57368a04174aa5b8b2f8bffb`  
		Last Modified: Tue, 03 Oct 2023 06:10:48 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c1a07105f3af8e80487db46085c03e9df93026a8e7f4c8a26654db2826a9d5e`  
		Last Modified: Tue, 03 Oct 2023 06:10:48 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2a175557d394fae17c79474734d29b5e49ff13dba8d6193c6bbb7d3779c82d`  
		Last Modified: Tue, 03 Oct 2023 07:17:38 GMT  
		Size: 14.4 MB (14374133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1960ccd711ddb8654be789e03ca9b87caa16611dafc565defef9b699e7758d`  
		Last Modified: Tue, 03 Oct 2023 07:17:36 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4bf78594cdc3a2cee6b96864eba53b2636f69f3354357a986b1fb1ff48fb75b`  
		Last Modified: Tue, 03 Oct 2023 07:17:36 GMT  
		Size: 1.5 KB (1466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `unit:1.31.0-minimal`

```console
$ docker pull unit@sha256:d3557fce352d557ecaa5fb542a4330875b55800b84f9999643b11f00ce7dec90
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:1.31.0-minimal` - linux; amd64

```console
$ docker pull unit@sha256:8a058f2ff2357725a0e2d43771b4b90127c7c34e70f8d4f4d82a7e4b4ab8eb56
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40261522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9594c8601a63442da9eafb2f3e26140881d6aaddcda8909fc46b77c5085f2805`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:56:57 GMT
LABEL org.opencontainers.image.title=Unit (minimal)
# Wed, 11 Oct 2023 19:56:57 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Wed, 11 Oct 2023 19:56:57 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Wed, 11 Oct 2023 19:56:58 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Wed, 11 Oct 2023 19:56:58 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Wed, 11 Oct 2023 19:56:58 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 11 Oct 2023 19:56:58 GMT
LABEL org.opencontainers.image.version=1.31.0
# Wed, 11 Oct 2023 19:58:10 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure      && make -j $NCPU version     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure      && make -j $NCPU version     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Wed, 11 Oct 2023 19:58:10 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Wed, 11 Oct 2023 19:58:10 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Wed, 11 Oct 2023 19:58:10 GMT
STOPSIGNAL SIGTERM
# Wed, 11 Oct 2023 19:58:10 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Wed, 11 Oct 2023 19:58:10 GMT
EXPOSE 80
# Wed, 11 Oct 2023 19:58:10 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5c7861ad106bab941590b1d57e5271280238a482a62fae3a844f35758d6cf7`  
		Last Modified: Wed, 11 Oct 2023 19:59:14 GMT  
		Size: 8.8 MB (8840929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab66ee2cb20cc896b833b4cac356f5b8e28033978c6cb561db3684ff1682aeab`  
		Last Modified: Wed, 11 Oct 2023 19:59:12 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d2941a2f57e962e97d0feb6ed0ba2e47520d777a33cddab81bdb2e23380087`  
		Last Modified: Wed, 11 Oct 2023 19:59:12 GMT  
		Size: 1.5 KB (1466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:1.31.0-minimal` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:ccb78488948a120aa107a189c9ec3141b59dbe074b90d58fff0722300f58d688
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38766827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5cfb5b45514db84628b66c8c7d11190d1b56b910be1b5ac53b473d3b093b1a0`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:06 GMT
ADD file:2c3e5451390c62f0b85f20139d2c88011cc54d649cdda5567084c050ad373372 in / 
# Wed, 11 Oct 2023 18:25:06 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:12:20 GMT
LABEL org.opencontainers.image.title=Unit (minimal)
# Wed, 11 Oct 2023 19:12:20 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Wed, 11 Oct 2023 19:12:20 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Wed, 11 Oct 2023 19:12:20 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Wed, 11 Oct 2023 19:12:20 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Wed, 11 Oct 2023 19:12:20 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 11 Oct 2023 19:12:20 GMT
LABEL org.opencontainers.image.version=1.31.0
# Wed, 11 Oct 2023 19:13:19 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure      && make -j $NCPU version     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure      && make -j $NCPU version     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Wed, 11 Oct 2023 19:13:19 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Wed, 11 Oct 2023 19:13:19 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Wed, 11 Oct 2023 19:13:19 GMT
STOPSIGNAL SIGTERM
# Wed, 11 Oct 2023 19:13:19 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Wed, 11 Oct 2023 19:13:19 GMT
EXPOSE 80
# Wed, 11 Oct 2023 19:13:19 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:85e50d2242ceaba78c3726e059dbd2fa06f5c18e265554bd43a482d19b256d20`  
		Last Modified: Wed, 11 Oct 2023 18:29:07 GMT  
		Size: 30.1 MB (30064086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd2be98a787512e0f31ff5098e023ab6f7741e004bd83a019f3338a55b88442`  
		Last Modified: Wed, 11 Oct 2023 19:14:15 GMT  
		Size: 8.7 MB (8700007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e73e3e6505fafe6a4bb27553af1b9d11b649958d6b791bf4262e079a5a2ac97`  
		Last Modified: Wed, 11 Oct 2023 19:14:14 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b9dcc88e7522a2402575f94c8416ef9bdf27633408d51eaee97dab9216e948`  
		Last Modified: Wed, 11 Oct 2023 19:14:14 GMT  
		Size: 1.5 KB (1469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `unit:1.31.0-node18`

```console
$ docker pull unit@sha256:e68a25b71a9114a0044cdaea34df4cadde567335b2787fa4b2d7da011256bcc4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:1.31.0-node18` - linux; amd64

```console
$ docker pull unit@sha256:fa50021bd72995919e871c6f1d02261d4692a610e7ac7c03915a37f8514dcedc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **395.6 MB (395574915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53d99c0dc02a1abd926ee6f0b175466990afae60a9bd60c3091a263668c02bb4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 04:55:51 GMT
ADD file:85db4f4c5016f51f7112a5d09cb7d4620f565a1379ae4b8a03c5ffc23886a876 in / 
# Wed, 20 Sep 2023 04:55:51 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:22:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:22:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:23:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 03:33:48 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Thu, 12 Oct 2023 00:11:34 GMT
ENV NODE_VERSION=18.18.1
# Thu, 12 Oct 2023 00:11:50 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     4ED778F539E3634C779C87C6D7062848A1AB005C     141F07595B7B3FFE74309A937405533BE57C7D57     74F12602B6F1C4E913FAA37AD3A89613643B6201     DD792F5973C6DE52C432CBDAC77ABFA00DDBF2B7     61FC681DFB92A079F1685E77973F295594EC4689     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4     C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     108F52B48DB57BB0CC439B2997B01419BD92F80A     A363A499291CBBC940DD62E41F10027AF002F8B0   ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Thu, 12 Oct 2023 00:11:51 GMT
ENV YARN_VERSION=1.22.19
# Thu, 12 Oct 2023 00:11:54 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Thu, 12 Oct 2023 00:11:54 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Thu, 12 Oct 2023 00:11:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 Oct 2023 00:11:54 GMT
CMD ["node"]
# Thu, 12 Oct 2023 05:51:37 GMT
LABEL org.opencontainers.image.title=Unit (node18)
# Thu, 12 Oct 2023 05:51:37 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Thu, 12 Oct 2023 05:51:37 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Thu, 12 Oct 2023 05:51:37 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Thu, 12 Oct 2023 05:51:37 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Thu, 12 Oct 2023 05:51:37 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Thu, 12 Oct 2023 05:51:37 GMT
LABEL org.opencontainers.image.version=1.31.0
# Thu, 12 Oct 2023 05:52:44 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && npm -g install node-gyp     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure nodejs --node-gyp=/usr/local/bin/node-gyp     && make -j $NCPU node node-install libunit-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure nodejs --node-gyp=/usr/local/bin/node-gyp     && make -j $NCPU node node-install libunit-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && rm -rf /root/.cache/ && rm -rf /root/.npm     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Thu, 12 Oct 2023 05:52:45 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Thu, 12 Oct 2023 05:52:45 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Thu, 12 Oct 2023 05:52:45 GMT
STOPSIGNAL SIGTERM
# Thu, 12 Oct 2023 05:52:45 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 12 Oct 2023 05:52:45 GMT
EXPOSE 80
# Thu, 12 Oct 2023 05:52:45 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:ddf874abf16cc990e0fd75a154a34ca0a03ee310ad895a18fb62ae15bf4171fb`  
		Last Modified: Wed, 20 Sep 2023 05:00:41 GMT  
		Size: 55.1 MB (55056714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1459d3ab8b5e46ac1a0a00134fe2f7b693474eb6d75ace97ecbe811a6f5b0e`  
		Last Modified: Wed, 20 Sep 2023 09:31:06 GMT  
		Size: 15.8 MB (15760408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab00e7798a04602c3f6e2dc445a994d75e96c45533cd44701f58509982a8c5`  
		Last Modified: Wed, 20 Sep 2023 09:31:23 GMT  
		Size: 54.6 MB (54584790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7883a473306cf6632abe7e913e0f1a21ac2fed038a4116473b25738b8b88b294`  
		Last Modified: Wed, 20 Sep 2023 09:31:55 GMT  
		Size: 196.8 MB (196842512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ea6a75eb435af25ba0b42343548bee2f6eb322326d98e39823aa45c2ff2b21`  
		Last Modified: Thu, 21 Sep 2023 03:37:33 GMT  
		Size: 4.2 KB (4201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bdebbc0d5036b999a378c1ca2357cf358ab6ecfdd8896372522f140f4cc843a`  
		Last Modified: Thu, 12 Oct 2023 00:18:24 GMT  
		Size: 45.9 MB (45920712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff7a673b7589fa8817b773a39cf9b4090edaed28fd18f6519b4ef530251d4c9`  
		Last Modified: Thu, 12 Oct 2023 00:18:17 GMT  
		Size: 2.3 MB (2282356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11925737d6f606c4cc192f42f33a4d08b7888d13dffc884c7d5d0acb4c84189f`  
		Last Modified: Thu, 12 Oct 2023 00:18:17 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1460cb765d966efc06550cd495ceab89c072bd5091310515f25f4e1daafd641`  
		Last Modified: Thu, 12 Oct 2023 05:55:04 GMT  
		Size: 25.1 MB (25120029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cbba6d81182e15ddd86af1b2c9855f06dff1725d982b28d8cb8b52dd8cb1aa3`  
		Last Modified: Thu, 12 Oct 2023 05:55:00 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:728963f3a996e7f4d5cd802fb3dc0e43ce45414eb200a37a594445342c1c7cf0`  
		Last Modified: Thu, 12 Oct 2023 05:55:00 GMT  
		Size: 1.5 KB (1468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:1.31.0-node18` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:45ac93d65b15ac754ec07e25f60788514fa0b08dd4f09df5994030f0c3fc7657
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **371.8 MB (371830804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07b42b9a686c23bf7326fceb8a9cecb28e2756776f609c8c0c364657995b3e52`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:20 GMT
ADD file:46dcdcde338d2c01fed5db3fac9041736d9305145d8fc2039dd5b3714d38ede8 in / 
# Wed, 20 Sep 2023 02:44:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:24:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:25:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:26:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 11:57:12 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Wed, 20 Sep 2023 12:00:25 GMT
ENV NODE_VERSION=18.18.0
# Wed, 20 Sep 2023 12:00:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     4ED778F539E3634C779C87C6D7062848A1AB005C     141F07595B7B3FFE74309A937405533BE57C7D57     74F12602B6F1C4E913FAA37AD3A89613643B6201     DD792F5973C6DE52C432CBDAC77ABFA00DDBF2B7     61FC681DFB92A079F1685E77973F295594EC4689     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4     C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     108F52B48DB57BB0CC439B2997B01419BD92F80A     A363A499291CBBC940DD62E41F10027AF002F8B0   ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Wed, 20 Sep 2023 12:00:41 GMT
ENV YARN_VERSION=1.22.19
# Wed, 20 Sep 2023 12:00:43 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Wed, 20 Sep 2023 12:00:44 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Wed, 20 Sep 2023 12:00:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Sep 2023 12:00:44 GMT
CMD ["node"]
# Wed, 20 Sep 2023 16:35:00 GMT
LABEL org.opencontainers.image.title=Unit (node18)
# Wed, 20 Sep 2023 16:35:00 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Wed, 20 Sep 2023 16:35:00 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Wed, 20 Sep 2023 16:35:00 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Wed, 20 Sep 2023 16:35:00 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Wed, 20 Sep 2023 16:35:00 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 20 Sep 2023 16:35:01 GMT
LABEL org.opencontainers.image.version=1.31.0
# Wed, 20 Sep 2023 16:35:48 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && npm -g install node-gyp     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure nodejs --node-gyp=/usr/local/bin/node-gyp     && make -j $NCPU node node-install libunit-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure nodejs --node-gyp=/usr/local/bin/node-gyp     && make -j $NCPU node node-install libunit-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && rm -rf /root/.cache/ && rm -rf /root/.npm     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Wed, 20 Sep 2023 16:35:49 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Wed, 20 Sep 2023 16:35:49 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Wed, 20 Sep 2023 16:35:49 GMT
STOPSIGNAL SIGTERM
# Wed, 20 Sep 2023 16:35:49 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Wed, 20 Sep 2023 16:35:49 GMT
EXPOSE 80
# Wed, 20 Sep 2023 16:35:49 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:31f5dc1f52c865588c43d8ec718f14d430e149b28f0b28232da825da7ae28f76`  
		Last Modified: Wed, 20 Sep 2023 02:47:53 GMT  
		Size: 53.7 MB (53704892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb60045eb75c62e890b95d28e4893132a6c7d61ec9979104ee4ff6e86c4badee`  
		Last Modified: Wed, 20 Sep 2023 09:33:11 GMT  
		Size: 15.7 MB (15746671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292737ab468ef80c6f78bdde4896157b8953d1e5556e1e526f40aeadcb547573`  
		Last Modified: Wed, 20 Sep 2023 09:33:26 GMT  
		Size: 54.7 MB (54676309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d93979d624211374be152eee1c99ed4ca9e6bae68694135fc440ab6c8fd2044`  
		Last Modified: Wed, 20 Sep 2023 09:33:51 GMT  
		Size: 189.8 MB (189778334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb09eadf5e4e66f30b34eb75eb93cef58634d965f2a8ac2e17dc33d89c4080f`  
		Last Modified: Wed, 20 Sep 2023 12:04:28 GMT  
		Size: 4.2 KB (4204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e4f179e1dbb42e377b9b3f6063a56f2c2123ebf49298a91892232927a0813a`  
		Last Modified: Wed, 20 Sep 2023 12:07:07 GMT  
		Size: 46.0 MB (46042536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9f5fbe4a6f071732862a0191dcefbe066c976172f11bdf45c6f480f6514e9f`  
		Last Modified: Wed, 20 Sep 2023 12:07:02 GMT  
		Size: 2.3 MB (2282453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6c3942de3b3640682578129a868919d480f825bbd409d9010c4205b8da3694`  
		Last Modified: Wed, 20 Sep 2023 12:07:01 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15348bc59ac653a1eca05468f9b80d95633effc2ecb5990010669d62125f1fdf`  
		Last Modified: Wed, 20 Sep 2023 16:47:35 GMT  
		Size: 9.6 MB (9592214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bae505592bea869518bd481ff8fc7683c43aa12820c7538593a449f458dcaba`  
		Last Modified: Wed, 20 Sep 2023 16:47:33 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b8b268e85b393e5d4752e8d08749afb692adf8611ad2b45034fea3e959ae88`  
		Last Modified: Wed, 20 Sep 2023 16:47:33 GMT  
		Size: 1.5 KB (1466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `unit:1.31.0-node20`

```console
$ docker pull unit@sha256:2e5fdd933383b2f8b36ddd1ff597467b8f7fb6082b30afcca4c574a3c79f24aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:1.31.0-node20` - linux; amd64

```console
$ docker pull unit@sha256:9a17e1115cff9de798eee7bb865e2e74f001de34c20b6fc2b44c868f94a45d83
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **382.2 MB (382169133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ce8f24e50447c2c131f7c2f7aa0edb8605448cae812158185bf76cd3dffa3fd`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 04:55:51 GMT
ADD file:85db4f4c5016f51f7112a5d09cb7d4620f565a1379ae4b8a03c5ffc23886a876 in / 
# Wed, 20 Sep 2023 04:55:51 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:22:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:22:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:23:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 03:33:48 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Fri, 29 Sep 2023 19:24:14 GMT
ENV NODE_VERSION=20.8.0
# Fri, 29 Sep 2023 19:24:30 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     4ED778F539E3634C779C87C6D7062848A1AB005C     141F07595B7B3FFE74309A937405533BE57C7D57     74F12602B6F1C4E913FAA37AD3A89613643B6201     DD792F5973C6DE52C432CBDAC77ABFA00DDBF2B7     61FC681DFB92A079F1685E77973F295594EC4689     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4     C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     108F52B48DB57BB0CC439B2997B01419BD92F80A     A363A499291CBBC940DD62E41F10027AF002F8B0   ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Fri, 29 Sep 2023 19:24:31 GMT
ENV YARN_VERSION=1.22.19
# Fri, 29 Sep 2023 19:24:34 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Fri, 29 Sep 2023 19:24:34 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 29 Sep 2023 19:24:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Sep 2023 19:24:34 GMT
CMD ["node"]
# Fri, 29 Sep 2023 20:10:13 GMT
LABEL org.opencontainers.image.title=Unit (node20)
# Fri, 29 Sep 2023 20:10:13 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Fri, 29 Sep 2023 20:10:14 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Fri, 29 Sep 2023 20:10:14 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Fri, 29 Sep 2023 20:10:14 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Fri, 29 Sep 2023 20:10:14 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Fri, 29 Sep 2023 20:10:14 GMT
LABEL org.opencontainers.image.version=1.31.0
# Fri, 29 Sep 2023 20:11:13 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && npm -g install node-gyp     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure nodejs --node-gyp=/usr/local/bin/node-gyp     && make -j $NCPU node node-install libunit-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure nodejs --node-gyp=/usr/local/bin/node-gyp     && make -j $NCPU node node-install libunit-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && rm -rf /root/.cache/ && rm -rf /root/.npm     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Fri, 29 Sep 2023 20:11:13 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Fri, 29 Sep 2023 20:11:13 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Fri, 29 Sep 2023 20:11:13 GMT
STOPSIGNAL SIGTERM
# Fri, 29 Sep 2023 20:11:13 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Fri, 29 Sep 2023 20:11:14 GMT
EXPOSE 80
# Fri, 29 Sep 2023 20:11:14 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:ddf874abf16cc990e0fd75a154a34ca0a03ee310ad895a18fb62ae15bf4171fb`  
		Last Modified: Wed, 20 Sep 2023 05:00:41 GMT  
		Size: 55.1 MB (55056714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1459d3ab8b5e46ac1a0a00134fe2f7b693474eb6d75ace97ecbe811a6f5b0e`  
		Last Modified: Wed, 20 Sep 2023 09:31:06 GMT  
		Size: 15.8 MB (15760408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab00e7798a04602c3f6e2dc445a994d75e96c45533cd44701f58509982a8c5`  
		Last Modified: Wed, 20 Sep 2023 09:31:23 GMT  
		Size: 54.6 MB (54584790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7883a473306cf6632abe7e913e0f1a21ac2fed038a4116473b25738b8b88b294`  
		Last Modified: Wed, 20 Sep 2023 09:31:55 GMT  
		Size: 196.8 MB (196842512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ea6a75eb435af25ba0b42343548bee2f6eb322326d98e39823aa45c2ff2b21`  
		Last Modified: Thu, 21 Sep 2023 03:37:33 GMT  
		Size: 4.2 KB (4201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4adcb3caaf61e057ad5e1d45646af5af38d7ed33278d2648d3673a3813a5ad0`  
		Last Modified: Fri, 29 Sep 2023 19:29:53 GMT  
		Size: 47.9 MB (47890750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074c9dbbb6a5fe5d4fbd49fd8130e8e295774aa9dfeb84f34aec191872569665`  
		Last Modified: Fri, 29 Sep 2023 19:29:46 GMT  
		Size: 2.3 MB (2280831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ab1c2aa4a9bd2cf26470d4a68b1adddc4ede0a127bc3e58c67675f9be39b2d`  
		Last Modified: Fri, 29 Sep 2023 19:29:46 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b1c647298a5806b069632bf26a9123073d2e6fe603aa7b55b83bcc3370f2970`  
		Last Modified: Fri, 29 Sep 2023 20:12:11 GMT  
		Size: 9.7 MB (9745734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29feecf70dcceefb09dc67128ccdd0ecebc069afc29c84c9853f0a9ba6ffdd73`  
		Last Modified: Fri, 29 Sep 2023 20:12:09 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbe243da98f864346f2177531540a62578a5cbd7f9f28eb535390ae195df6e9`  
		Last Modified: Fri, 29 Sep 2023 20:12:09 GMT  
		Size: 1.5 KB (1471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:1.31.0-node20` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:9a0f79ed710800179506279f8abf519d2212fb2442c58130e994abd08d09c541
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **373.7 MB (373674910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46fc524ca4f70502a07c6995aa6dfc61c0bd1fa20d500d61386f005d8139e836`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:20 GMT
ADD file:46dcdcde338d2c01fed5db3fac9041736d9305145d8fc2039dd5b3714d38ede8 in / 
# Wed, 20 Sep 2023 02:44:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:24:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:25:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:26:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 11:57:12 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Fri, 29 Sep 2023 20:33:52 GMT
ENV NODE_VERSION=20.8.0
# Fri, 29 Sep 2023 20:34:06 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     4ED778F539E3634C779C87C6D7062848A1AB005C     141F07595B7B3FFE74309A937405533BE57C7D57     74F12602B6F1C4E913FAA37AD3A89613643B6201     DD792F5973C6DE52C432CBDAC77ABFA00DDBF2B7     61FC681DFB92A079F1685E77973F295594EC4689     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4     C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     108F52B48DB57BB0CC439B2997B01419BD92F80A     A363A499291CBBC940DD62E41F10027AF002F8B0   ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Fri, 29 Sep 2023 20:34:07 GMT
ENV YARN_VERSION=1.22.19
# Fri, 29 Sep 2023 20:34:10 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Fri, 29 Sep 2023 20:34:10 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 29 Sep 2023 20:34:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Sep 2023 20:34:10 GMT
CMD ["node"]
# Fri, 29 Sep 2023 21:30:12 GMT
LABEL org.opencontainers.image.title=Unit (node20)
# Fri, 29 Sep 2023 21:30:12 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Fri, 29 Sep 2023 21:30:12 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Fri, 29 Sep 2023 21:30:12 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Fri, 29 Sep 2023 21:30:12 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Fri, 29 Sep 2023 21:30:13 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Fri, 29 Sep 2023 21:30:13 GMT
LABEL org.opencontainers.image.version=1.31.0
# Fri, 29 Sep 2023 21:31:03 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && npm -g install node-gyp     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure nodejs --node-gyp=/usr/local/bin/node-gyp     && make -j $NCPU node node-install libunit-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure nodejs --node-gyp=/usr/local/bin/node-gyp     && make -j $NCPU node node-install libunit-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && rm -rf /root/.cache/ && rm -rf /root/.npm     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Fri, 29 Sep 2023 21:31:03 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Fri, 29 Sep 2023 21:31:03 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Fri, 29 Sep 2023 21:31:03 GMT
STOPSIGNAL SIGTERM
# Fri, 29 Sep 2023 21:31:03 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Fri, 29 Sep 2023 21:31:03 GMT
EXPOSE 80
# Fri, 29 Sep 2023 21:31:03 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:31f5dc1f52c865588c43d8ec718f14d430e149b28f0b28232da825da7ae28f76`  
		Last Modified: Wed, 20 Sep 2023 02:47:53 GMT  
		Size: 53.7 MB (53704892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb60045eb75c62e890b95d28e4893132a6c7d61ec9979104ee4ff6e86c4badee`  
		Last Modified: Wed, 20 Sep 2023 09:33:11 GMT  
		Size: 15.7 MB (15746671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292737ab468ef80c6f78bdde4896157b8953d1e5556e1e526f40aeadcb547573`  
		Last Modified: Wed, 20 Sep 2023 09:33:26 GMT  
		Size: 54.7 MB (54676309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d93979d624211374be152eee1c99ed4ca9e6bae68694135fc440ab6c8fd2044`  
		Last Modified: Wed, 20 Sep 2023 09:33:51 GMT  
		Size: 189.8 MB (189778334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb09eadf5e4e66f30b34eb75eb93cef58634d965f2a8ac2e17dc33d89c4080f`  
		Last Modified: Wed, 20 Sep 2023 12:04:28 GMT  
		Size: 4.2 KB (4204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24debdbd9457a0eb10a03ae601118a956b98fa2398012c256f56bf86c85f3e82`  
		Last Modified: Fri, 29 Sep 2023 20:39:17 GMT  
		Size: 47.9 MB (47887557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0420cb46253f07a9a438ceb9fb754f50231810e402e5d0cc102c603ab7a81e63`  
		Last Modified: Fri, 29 Sep 2023 20:39:12 GMT  
		Size: 2.3 MB (2280989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5352f9acdfe7faf9aca15154311a32d6202f149fe040531018acccc56a009fc`  
		Last Modified: Fri, 29 Sep 2023 20:39:11 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c2ebc1082453fd2911237585674e39ca8703025029b63cfd45f948f78517be`  
		Last Modified: Fri, 29 Sep 2023 21:31:46 GMT  
		Size: 9.6 MB (9592758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e88f1e59c0db97a5a8f3b473c48187fb5c181f7e0466fe4e6b67abe6a0ba0ce`  
		Last Modified: Fri, 29 Sep 2023 21:31:45 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b45aeeecd92e7513ded27236a3f362b72a18420700fb28ca4e7bc6db3068b0`  
		Last Modified: Fri, 29 Sep 2023 21:31:45 GMT  
		Size: 1.5 KB (1468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `unit:1.31.0-perl5.36`

```console
$ docker pull unit@sha256:e0f01023f2b4a55743f179baa4df204e66de3b578d76c5751a8e23be8b77c589
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:1.31.0-perl5.36` - linux; amd64

```console
$ docker pull unit@sha256:ef50de0b9c58bbbd5847056f3c7e4729038d51221785c34997b5cc71aad4932b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.7 MB (344722709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ba2be77e69bbbc055fdbf3993f1f99d53ab5bb80978b32f5b6cda84becdd29b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 04:55:51 GMT
ADD file:85db4f4c5016f51f7112a5d09cb7d4620f565a1379ae4b8a03c5ffc23886a876 in / 
# Wed, 20 Sep 2023 04:55:51 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:22:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:22:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:23:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 12:31:20 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 20 Sep 2023 12:31:20 GMT
WORKDIR /usr/src/perl
# Wed, 20 Sep 2023 13:49:26 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.1.tar.xz -o perl-5.36.1.tar.xz     && echo 'bd91217ea8a8c8b81f21ebbb6cefdf0d13ae532013f944cdece2cd51aef4b6a7 *perl-5.36.1.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.1.tar.xz -C /usr/src/perl     && rm perl-5.36.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Wed, 20 Sep 2023 13:49:27 GMT
WORKDIR /usr/src/app
# Wed, 20 Sep 2023 13:49:27 GMT
CMD ["perl5.36.1" "-de0"]
# Wed, 20 Sep 2023 21:39:07 GMT
LABEL org.opencontainers.image.title=Unit (perl5.36)
# Wed, 20 Sep 2023 21:39:08 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Wed, 20 Sep 2023 21:39:08 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Wed, 20 Sep 2023 21:39:08 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Wed, 20 Sep 2023 21:39:08 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Wed, 20 Sep 2023 21:39:08 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 20 Sep 2023 21:39:08 GMT
LABEL org.opencontainers.image.version=1.31.0
# Wed, 20 Sep 2023 21:39:58 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure perl     && make -j $NCPU perl-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure perl     && make -j $NCPU perl-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Wed, 20 Sep 2023 21:39:58 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Wed, 20 Sep 2023 21:39:59 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Wed, 20 Sep 2023 21:39:59 GMT
STOPSIGNAL SIGTERM
# Wed, 20 Sep 2023 21:39:59 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Wed, 20 Sep 2023 21:39:59 GMT
EXPOSE 80
# Wed, 20 Sep 2023 21:39:59 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:ddf874abf16cc990e0fd75a154a34ca0a03ee310ad895a18fb62ae15bf4171fb`  
		Last Modified: Wed, 20 Sep 2023 05:00:41 GMT  
		Size: 55.1 MB (55056714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1459d3ab8b5e46ac1a0a00134fe2f7b693474eb6d75ace97ecbe811a6f5b0e`  
		Last Modified: Wed, 20 Sep 2023 09:31:06 GMT  
		Size: 15.8 MB (15760408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab00e7798a04602c3f6e2dc445a994d75e96c45533cd44701f58509982a8c5`  
		Last Modified: Wed, 20 Sep 2023 09:31:23 GMT  
		Size: 54.6 MB (54584790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7883a473306cf6632abe7e913e0f1a21ac2fed038a4116473b25738b8b88b294`  
		Last Modified: Wed, 20 Sep 2023 09:31:55 GMT  
		Size: 196.8 MB (196842512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52b3edeb95fa7a0041689ffc83f83c850c381908d41acdd82e901f87878cdfd`  
		Last Modified: Wed, 20 Sep 2023 16:26:00 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801fec7181e64cb33e9618fc12991ed305fdc90cb37ba97513a9814b7da3b14d`  
		Last Modified: Wed, 20 Sep 2023 16:30:09 GMT  
		Size: 15.2 MB (15226973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13355de3cf006b6d46c2682a3c1a7980543832e27a6814162bcf2c11c78f4bac`  
		Last Modified: Wed, 20 Sep 2023 16:30:06 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1fde6eb25125a7410bf2ba9789a64d9d0b9f3b2e6bcfdfbb463132c6ec08df4`  
		Last Modified: Wed, 20 Sep 2023 21:42:59 GMT  
		Size: 7.2 MB (7248249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0d21cdf1397df3869aba37cbca4e46d401c97eabf8dfab51c9a1f1d7257128`  
		Last Modified: Wed, 20 Sep 2023 21:42:57 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8684e4982998d379d595ff34fce63e1ee9a5364e73b2b00ffb4f0f1fe2aff25b`  
		Last Modified: Wed, 20 Sep 2023 21:42:57 GMT  
		Size: 1.5 KB (1467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:1.31.0-perl5.36` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:0765c0cce675be3ac6160eef54947c98d790882fac94ca2e62d7432f8a710267
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.2 MB (336198228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c76a0625c259cb3b83797c395eab3e7b7f3b7f827bdf5bc3264262653a723e0`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:20 GMT
ADD file:46dcdcde338d2c01fed5db3fac9041736d9305145d8fc2039dd5b3714d38ede8 in / 
# Wed, 20 Sep 2023 02:44:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:24:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:25:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:26:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 12:49:59 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 20 Sep 2023 12:49:59 GMT
WORKDIR /usr/src/perl
# Wed, 20 Sep 2023 13:52:05 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.1.tar.xz -o perl-5.36.1.tar.xz     && echo 'bd91217ea8a8c8b81f21ebbb6cefdf0d13ae532013f944cdece2cd51aef4b6a7 *perl-5.36.1.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.1.tar.xz -C /usr/src/perl     && rm perl-5.36.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Wed, 20 Sep 2023 13:52:06 GMT
WORKDIR /usr/src/app
# Wed, 20 Sep 2023 13:52:06 GMT
CMD ["perl5.36.1" "-de0"]
# Wed, 20 Sep 2023 16:36:46 GMT
LABEL org.opencontainers.image.title=Unit (perl5.36)
# Wed, 20 Sep 2023 16:36:46 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Wed, 20 Sep 2023 16:36:46 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Wed, 20 Sep 2023 16:36:46 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Wed, 20 Sep 2023 16:36:46 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Wed, 20 Sep 2023 16:36:46 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 20 Sep 2023 16:36:46 GMT
LABEL org.opencontainers.image.version=1.31.0
# Wed, 20 Sep 2023 16:37:27 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure perl     && make -j $NCPU perl-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure perl     && make -j $NCPU perl-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Wed, 20 Sep 2023 16:37:27 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Wed, 20 Sep 2023 16:37:27 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Wed, 20 Sep 2023 16:37:27 GMT
STOPSIGNAL SIGTERM
# Wed, 20 Sep 2023 16:37:27 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Wed, 20 Sep 2023 16:37:27 GMT
EXPOSE 80
# Wed, 20 Sep 2023 16:37:27 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:31f5dc1f52c865588c43d8ec718f14d430e149b28f0b28232da825da7ae28f76`  
		Last Modified: Wed, 20 Sep 2023 02:47:53 GMT  
		Size: 53.7 MB (53704892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb60045eb75c62e890b95d28e4893132a6c7d61ec9979104ee4ff6e86c4badee`  
		Last Modified: Wed, 20 Sep 2023 09:33:11 GMT  
		Size: 15.7 MB (15746671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292737ab468ef80c6f78bdde4896157b8953d1e5556e1e526f40aeadcb547573`  
		Last Modified: Wed, 20 Sep 2023 09:33:26 GMT  
		Size: 54.7 MB (54676309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d93979d624211374be152eee1c99ed4ca9e6bae68694135fc440ab6c8fd2044`  
		Last Modified: Wed, 20 Sep 2023 09:33:51 GMT  
		Size: 189.8 MB (189778334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1117f9029f2f12e3c0ea1a49d453513b6d3c4ec5a2cf433fd56be576e3c53290`  
		Last Modified: Wed, 20 Sep 2023 15:58:14 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8093c0fb05a13b2a87dc07b437542e7a922365faaa15cbce8f4d7384483a02e`  
		Last Modified: Wed, 20 Sep 2023 16:02:31 GMT  
		Size: 15.2 MB (15164956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f04ba44dcfc11add9e8950c97672f1d8fbd34378618fda92771d4fc1f7d89e61`  
		Last Modified: Wed, 20 Sep 2023 16:02:29 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6686249ee24f0cea74da9d6bd6af97ab214e86c31ddbf1a6240ceb6d85e58b9`  
		Last Modified: Wed, 20 Sep 2023 16:48:00 GMT  
		Size: 7.1 MB (7124001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0e3baba03795b87967e901297e79c21e3bc8e1575373ee369d36f0b78b8b35`  
		Last Modified: Wed, 20 Sep 2023 16:47:59 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f15f31f41115dc86198f9372e52e119c904149c9a09c4660c16f458d434c15a`  
		Last Modified: Wed, 20 Sep 2023 16:47:59 GMT  
		Size: 1.5 KB (1466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `unit:1.31.0-perl5.38`

```console
$ docker pull unit@sha256:3c8e1eace3473a976477d60002f38209ae5ed55cf67898083eb6e9c688ceca09
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:1.31.0-perl5.38` - linux; amd64

```console
$ docker pull unit@sha256:5c8da37c00d90a41311793367b010c025b198bca791f4a48c1917dd5972ac6aa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **345.1 MB (345143371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f90ea950a89663407724e0fadeea9c93e63be29cb6cbd80b2223e894425414b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 04:55:51 GMT
ADD file:85db4f4c5016f51f7112a5d09cb7d4620f565a1379ae4b8a03c5ffc23886a876 in / 
# Wed, 20 Sep 2023 04:55:51 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:22:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:22:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:23:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 12:31:20 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 20 Sep 2023 12:31:20 GMT
WORKDIR /usr/src/perl
# Wed, 20 Sep 2023 12:36:40 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Wed, 20 Sep 2023 12:36:40 GMT
WORKDIR /usr/src/app
# Wed, 20 Sep 2023 12:36:40 GMT
CMD ["perl5.38.0" "-de0"]
# Wed, 20 Sep 2023 21:38:09 GMT
LABEL org.opencontainers.image.title=Unit (perl5.38)
# Wed, 20 Sep 2023 21:38:09 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Wed, 20 Sep 2023 21:38:09 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Wed, 20 Sep 2023 21:38:09 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Wed, 20 Sep 2023 21:38:09 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Wed, 20 Sep 2023 21:38:09 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 20 Sep 2023 21:38:09 GMT
LABEL org.opencontainers.image.version=1.31.0
# Wed, 20 Sep 2023 21:39:01 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure perl     && make -j $NCPU perl-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure perl     && make -j $NCPU perl-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Wed, 20 Sep 2023 21:39:01 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Wed, 20 Sep 2023 21:39:01 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Wed, 20 Sep 2023 21:39:01 GMT
STOPSIGNAL SIGTERM
# Wed, 20 Sep 2023 21:39:01 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Wed, 20 Sep 2023 21:39:02 GMT
EXPOSE 80
# Wed, 20 Sep 2023 21:39:02 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:ddf874abf16cc990e0fd75a154a34ca0a03ee310ad895a18fb62ae15bf4171fb`  
		Last Modified: Wed, 20 Sep 2023 05:00:41 GMT  
		Size: 55.1 MB (55056714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1459d3ab8b5e46ac1a0a00134fe2f7b693474eb6d75ace97ecbe811a6f5b0e`  
		Last Modified: Wed, 20 Sep 2023 09:31:06 GMT  
		Size: 15.8 MB (15760408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab00e7798a04602c3f6e2dc445a994d75e96c45533cd44701f58509982a8c5`  
		Last Modified: Wed, 20 Sep 2023 09:31:23 GMT  
		Size: 54.6 MB (54584790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7883a473306cf6632abe7e913e0f1a21ac2fed038a4116473b25738b8b88b294`  
		Last Modified: Wed, 20 Sep 2023 09:31:55 GMT  
		Size: 196.8 MB (196842512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52b3edeb95fa7a0041689ffc83f83c850c381908d41acdd82e901f87878cdfd`  
		Last Modified: Wed, 20 Sep 2023 16:26:00 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024bd37d7f953a74bb38362b5317ae998d40ca2fee8b8a8dca43148a8a3f4cfb`  
		Last Modified: Wed, 20 Sep 2023 16:26:03 GMT  
		Size: 15.6 MB (15635163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587b5a52835c5daacc0e54325851e643a1154769e8db9e765060b7fc4b43493d`  
		Last Modified: Wed, 20 Sep 2023 16:26:00 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66dfb10c0b36ce058292ef115f82b9ac08a5475f9e99e422fce5aabd7c51ba1f`  
		Last Modified: Wed, 20 Sep 2023 21:42:45 GMT  
		Size: 7.3 MB (7260721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f52778a1e6d26c16c061d9f1f0ce15b47ae70e29ba231b39f9e8ec2efe2ba4`  
		Last Modified: Wed, 20 Sep 2023 21:42:43 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fb22967b16e13a68371214b23ec1abf149a140a54d40230ae032b26df9d492`  
		Last Modified: Wed, 20 Sep 2023 21:42:43 GMT  
		Size: 1.5 KB (1468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:1.31.0-perl5.38` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:215346afdcf662582d06311303dc561b27195a9cd91b6b832805b504ecf15d32
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.6 MB (336614710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72b2d67a5c47a9faffd0dfa45b15e7e137607ed5b61f6a4c5fa0ce4e1b7b6fef`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:20 GMT
ADD file:46dcdcde338d2c01fed5db3fac9041736d9305145d8fc2039dd5b3714d38ede8 in / 
# Wed, 20 Sep 2023 02:44:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:24:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:25:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:26:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 12:49:59 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 20 Sep 2023 12:49:59 GMT
WORKDIR /usr/src/perl
# Wed, 20 Sep 2023 12:54:12 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Wed, 20 Sep 2023 12:54:13 GMT
WORKDIR /usr/src/app
# Wed, 20 Sep 2023 12:54:13 GMT
CMD ["perl5.38.0" "-de0"]
# Wed, 20 Sep 2023 16:35:58 GMT
LABEL org.opencontainers.image.title=Unit (perl5.38)
# Wed, 20 Sep 2023 16:35:58 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Wed, 20 Sep 2023 16:35:58 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Wed, 20 Sep 2023 16:35:58 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Wed, 20 Sep 2023 16:35:58 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Wed, 20 Sep 2023 16:35:58 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 20 Sep 2023 16:35:58 GMT
LABEL org.opencontainers.image.version=1.31.0
# Wed, 20 Sep 2023 16:36:39 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure perl     && make -j $NCPU perl-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure perl     && make -j $NCPU perl-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Wed, 20 Sep 2023 16:36:39 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Wed, 20 Sep 2023 16:36:39 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Wed, 20 Sep 2023 16:36:39 GMT
STOPSIGNAL SIGTERM
# Wed, 20 Sep 2023 16:36:39 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Wed, 20 Sep 2023 16:36:39 GMT
EXPOSE 80
# Wed, 20 Sep 2023 16:36:39 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:31f5dc1f52c865588c43d8ec718f14d430e149b28f0b28232da825da7ae28f76`  
		Last Modified: Wed, 20 Sep 2023 02:47:53 GMT  
		Size: 53.7 MB (53704892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb60045eb75c62e890b95d28e4893132a6c7d61ec9979104ee4ff6e86c4badee`  
		Last Modified: Wed, 20 Sep 2023 09:33:11 GMT  
		Size: 15.7 MB (15746671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292737ab468ef80c6f78bdde4896157b8953d1e5556e1e526f40aeadcb547573`  
		Last Modified: Wed, 20 Sep 2023 09:33:26 GMT  
		Size: 54.7 MB (54676309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d93979d624211374be152eee1c99ed4ca9e6bae68694135fc440ab6c8fd2044`  
		Last Modified: Wed, 20 Sep 2023 09:33:51 GMT  
		Size: 189.8 MB (189778334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1117f9029f2f12e3c0ea1a49d453513b6d3c4ec5a2cf433fd56be576e3c53290`  
		Last Modified: Wed, 20 Sep 2023 15:58:14 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b317f1f02fe8dd016d19c93440ae1ccfd4b40693bf91614faefd972e49128e`  
		Last Modified: Wed, 20 Sep 2023 15:58:16 GMT  
		Size: 15.6 MB (15569671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4ff545690965c4c8230cb542b04cbb5df00908ce2f26782b952990cb2a2dcf`  
		Last Modified: Wed, 20 Sep 2023 15:58:14 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e086d049566a67139ff421c28ba34c3a886279adff787914ca7d2c24aaca14b`  
		Last Modified: Wed, 20 Sep 2023 16:47:45 GMT  
		Size: 7.1 MB (7135766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dfd51d8d916894d7797d4c9a60e0eac911429596844e9663d88aea528066cfc`  
		Last Modified: Wed, 20 Sep 2023 16:47:44 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b8a03d176384e4135d0956f78c091cced19e54a2a562bf63b3224dea0a2197`  
		Last Modified: Wed, 20 Sep 2023 16:47:44 GMT  
		Size: 1.5 KB (1471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `unit:1.31.0-php8.2`

```console
$ docker pull unit@sha256:98a08f025af091d8e63156d9913c2264b8bd2fe6f7fd76eac388713ffff7cd7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:1.31.0-php8.2` - linux; amd64

```console
$ docker pull unit@sha256:3489384ba2bdfa707d08431b335b0f776c206863e93e5998892199036d767468
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.3 MB (177316657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1376dc93023d0e476b2a7d5762eede2dc29c43a2ef48986784e2b83701098818`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:51:31 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 12 Oct 2023 03:51:31 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 12 Oct 2023 03:51:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:51:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 12 Oct 2023 03:51:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 12 Oct 2023 03:51:50 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 12 Oct 2023 03:51:50 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 12 Oct 2023 03:51:50 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 12 Oct 2023 04:20:25 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 12 Oct 2023 04:20:25 GMT
ENV PHP_VERSION=8.2.11
# Thu, 12 Oct 2023 04:20:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.11.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.11.tar.xz.asc
# Thu, 12 Oct 2023 04:20:25 GMT
ENV PHP_SHA256=29af82e4f7509831490552918aad502697453f0869a579ee1b80b08f9112c5b8
# Thu, 12 Oct 2023 04:20:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 12 Oct 2023 04:20:38 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 12 Oct 2023 04:23:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--enable-embed 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 12 Oct 2023 04:23:40 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 12 Oct 2023 04:23:40 GMT
RUN docker-php-ext-enable sodium
# Thu, 12 Oct 2023 04:23:41 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 12 Oct 2023 04:23:41 GMT
CMD ["php" "-a"]
# Thu, 12 Oct 2023 05:53:05 GMT
LABEL org.opencontainers.image.title=Unit (php8.2)
# Thu, 12 Oct 2023 05:53:05 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Thu, 12 Oct 2023 05:53:06 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Thu, 12 Oct 2023 05:53:06 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Thu, 12 Oct 2023 05:53:06 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Thu, 12 Oct 2023 05:53:06 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Thu, 12 Oct 2023 05:53:06 GMT
LABEL org.opencontainers.image.version=1.31.0
# Thu, 12 Oct 2023 05:54:04 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure php     && make -j $NCPU php-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure php     && make -j $NCPU php-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && ldconfig     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Thu, 12 Oct 2023 05:54:04 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Thu, 12 Oct 2023 05:54:05 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Thu, 12 Oct 2023 05:54:05 GMT
STOPSIGNAL SIGTERM
# Thu, 12 Oct 2023 05:54:05 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 12 Oct 2023 05:54:05 GMT
EXPOSE 80
# Thu, 12 Oct 2023 05:54:05 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a19ba793cb30aa4b42c5ad97548d55ae00fec0c4877c76126583715d708ce9`  
		Last Modified: Thu, 12 Oct 2023 05:32:53 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e4193503519ae06279df9269c22245e20b0acb785371e054e848264cb901c2`  
		Last Modified: Thu, 12 Oct 2023 05:33:06 GMT  
		Size: 91.6 MB (91635233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de997c28946e5c94cd3025094a7aee8f9df3ea9dedc8e2d250d1edd5786ca21`  
		Last Modified: Thu, 12 Oct 2023 05:32:53 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:873f439f47bcfe71f69387163cbdee5f5916f1a239621af82adeb6545c8ebc9e`  
		Last Modified: Thu, 12 Oct 2023 05:36:20 GMT  
		Size: 12.4 MB (12366685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f4856de7837698b7c3f763062a2517b23adf18b5f61951f75c45e4f2f44b48`  
		Last Modified: Thu, 12 Oct 2023 05:36:19 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732fb5749b825ba822de67840caf6e00fc3c04541a5fb4da950ef79484b9a212`  
		Last Modified: Thu, 12 Oct 2023 05:36:24 GMT  
		Size: 34.6 MB (34578752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b802f88bd6721adf7730d5d3d154ec4fb86d8a0ba9b5a68e8b21f0641788cc`  
		Last Modified: Thu, 12 Oct 2023 05:36:19 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc1bfbe94373cbbdf1f91bd9f7d1ce800915c9dff4534f9e480b565522cea63`  
		Last Modified: Thu, 12 Oct 2023 05:36:19 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c18b9d27728522e863897b864d23bab4ac72a317b907a4947385190fa8cd76`  
		Last Modified: Thu, 12 Oct 2023 05:55:17 GMT  
		Size: 7.3 MB (7311692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d399b38b2e7a680119855d6a3c02175a9fca6045029fe034007c7c35159138`  
		Last Modified: Thu, 12 Oct 2023 05:55:16 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdd7d3b6ce6a617dbb942596a3aaf0ed6d14fefa6f7c507122bb9988213382ca`  
		Last Modified: Thu, 12 Oct 2023 05:55:16 GMT  
		Size: 1.5 KB (1473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:1.31.0-php8.2` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:9437be31a41199971c8c97470dc6210d02940181cf88412da7418b328e6fb65e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.0 MB (171047539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80a74fa49a48de50ce64633c1cfc1d6e8319ebf8d0900de19dce27e35f4cc22c`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:28 GMT
ADD file:024479be439b4ecb37c939e68673adc72955f3345ca0e809bd13e897709e59e4 in / 
# Wed, 20 Sep 2023 02:44:28 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 03:08:10 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 03:08:10 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 03:08:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 03:08:28 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 03:08:28 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 03:08:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 03:08:29 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 03:08:29 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 03:34:37 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Sat, 30 Sep 2023 02:00:47 GMT
ENV PHP_VERSION=8.2.11
# Sat, 30 Sep 2023 02:00:47 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.11.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.11.tar.xz.asc
# Sat, 30 Sep 2023 02:00:47 GMT
ENV PHP_SHA256=29af82e4f7509831490552918aad502697453f0869a579ee1b80b08f9112c5b8
# Sat, 30 Sep 2023 02:00:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 30 Sep 2023 02:00:57 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 30 Sep 2023 02:03:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--enable-embed 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 30 Sep 2023 02:03:41 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Sat, 30 Sep 2023 02:03:42 GMT
RUN docker-php-ext-enable sodium
# Sat, 30 Sep 2023 02:03:42 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 30 Sep 2023 02:03:42 GMT
CMD ["php" "-a"]
# Sat, 30 Sep 2023 06:58:25 GMT
LABEL org.opencontainers.image.title=Unit (php8.2)
# Sat, 30 Sep 2023 06:58:25 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Sat, 30 Sep 2023 06:58:25 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Sat, 30 Sep 2023 06:58:25 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Sat, 30 Sep 2023 06:58:25 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Sat, 30 Sep 2023 06:58:25 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Sat, 30 Sep 2023 06:58:26 GMT
LABEL org.opencontainers.image.version=1.31.0
# Sat, 30 Sep 2023 06:59:14 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure php     && make -j $NCPU php-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure php     && make -j $NCPU php-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && ldconfig     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Sat, 30 Sep 2023 06:59:14 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Sat, 30 Sep 2023 06:59:15 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Sat, 30 Sep 2023 06:59:15 GMT
STOPSIGNAL SIGTERM
# Sat, 30 Sep 2023 06:59:15 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Sat, 30 Sep 2023 06:59:15 GMT
EXPOSE 80
# Sat, 30 Sep 2023 06:59:15 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:fc521c5b98350f6fd8c72ace1e48558bb7b53cb3db201a2a3b42095401cd02f1`  
		Last Modified: Wed, 20 Sep 2023 02:48:13 GMT  
		Size: 30.1 MB (30062869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011d119a94c0f59e8eabde01f2b7a4da9d92360102426dcaad9d1d0be4b4092c`  
		Last Modified: Wed, 20 Sep 2023 06:01:09 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c2e7320620034b78e6c4122bdaf225b766ba582397845df17e1ca60098d29c`  
		Last Modified: Wed, 20 Sep 2023 06:01:20 GMT  
		Size: 86.9 MB (86929113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aff55be7dadd795271386506373641b927cc6f05b8efda3e6ff839f8419b6b1`  
		Last Modified: Wed, 20 Sep 2023 06:01:09 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454bbb352bd352bcfb21a488d3c30d4c5bd361cc4d710c6c074ee2b2a195c427`  
		Last Modified: Sat, 30 Sep 2023 03:44:41 GMT  
		Size: 12.4 MB (12364849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ed8e7b4178686ac6d44751dfb2df41c828db70441a966b5e9990ced097a483`  
		Last Modified: Sat, 30 Sep 2023 03:44:39 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe154f23538ad101fbd710d1152a33004c79ccdc6e535141f45e8338ea0d95d`  
		Last Modified: Sat, 30 Sep 2023 03:44:43 GMT  
		Size: 34.5 MB (34500324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4112cbf9310ae8cf8dd3cafe076e961454810770e4d6754f569e84f41eefb654`  
		Last Modified: Sat, 30 Sep 2023 03:44:39 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c11bd2118fe41faeb02374298f96d20fd1856d59a76c721cf384b44839e6582`  
		Last Modified: Sat, 30 Sep 2023 03:44:39 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050dd55155fdfd13168a12283c20639e5417b26741fd7b2176631945880a03f4`  
		Last Modified: Sat, 30 Sep 2023 07:00:01 GMT  
		Size: 7.2 MB (7183962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb54f4b569069290b7de89ebf3fb8ad666b51d307f3a23d3bd934fe26b1438d`  
		Last Modified: Sat, 30 Sep 2023 07:00:00 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fba378c9872d4d6a4444ea03d8a49f1eca4fc97928ac5aa68c747896ec36daf`  
		Last Modified: Sat, 30 Sep 2023 07:00:00 GMT  
		Size: 1.5 KB (1468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `unit:1.31.0-python3.11`

```console
$ docker pull unit@sha256:97f7574d4ce36f8eca74f25555dce4835dfc479d033acb68e20d19dec141e112
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:1.31.0-python3.11` - linux; amd64

```console
$ docker pull unit@sha256:7e930385f350c30f67fb9d8af68e500c684c6a7037a887fb28e8e9bb17f21a63
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.2 MB (359180856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f539861a71c1bdb6090a4ad0d937ad8e88c23b4e00971e8aee44a140ca84439`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 04:55:51 GMT
ADD file:85db4f4c5016f51f7112a5d09cb7d4620f565a1379ae4b8a03c5ffc23886a876 in / 
# Wed, 20 Sep 2023 04:55:51 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:22:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:22:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:23:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 02 Oct 2023 16:48:26 GMT
ENV LANG=C.UTF-8
# Mon, 02 Oct 2023 16:48:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 02 Oct 2023 16:48:26 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_VERSION=3.11.6
# Mon, 02 Oct 2023 16:48:26 GMT
RUN set -eux; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		bin="$(readlink -ve /usr/local/bin/python3)"; 	dir="$(dirname "$bin")"; 	mkdir -p "/usr/share/gdb/auto-load/$dir"; 	cp -vL Tools/gdb/libpython.py "/usr/share/gdb/auto-load/$bin-gdb.py"; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		python3 --version # buildkit
# Mon, 02 Oct 2023 16:48:26 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_PIP_VERSION=23.2.1
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/9af82b715db434abb94a0a6f3569f43e72157346/public/get-pip.py
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_GET_PIP_SHA256=45a2bb8bf2bb5eff16fdd00faef6f29731831c7c59bd9fc2bf1f3bed511ff1fe
# Mon, 02 Oct 2023 16:48:26 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Mon, 02 Oct 2023 16:48:26 GMT
CMD ["python3"]
# Tue, 03 Oct 2023 04:27:32 GMT
LABEL org.opencontainers.image.title=Unit (python3.11)
# Tue, 03 Oct 2023 04:27:32 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Tue, 03 Oct 2023 04:27:32 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Tue, 03 Oct 2023 04:27:32 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Tue, 03 Oct 2023 04:27:32 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Tue, 03 Oct 2023 04:27:32 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 03 Oct 2023 04:27:33 GMT
LABEL org.opencontainers.image.version=1.31.0
# Tue, 03 Oct 2023 04:28:23 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure python --config=/usr/local/bin/python3-config     && make -j $NCPU python3-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure python --config=/usr/local/bin/python3-config     && make -j $NCPU python3-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Tue, 03 Oct 2023 04:28:23 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Tue, 03 Oct 2023 04:28:23 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Tue, 03 Oct 2023 04:28:24 GMT
STOPSIGNAL SIGTERM
# Tue, 03 Oct 2023 04:28:24 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 03 Oct 2023 04:28:24 GMT
EXPOSE 80
# Tue, 03 Oct 2023 04:28:24 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:ddf874abf16cc990e0fd75a154a34ca0a03ee310ad895a18fb62ae15bf4171fb`  
		Last Modified: Wed, 20 Sep 2023 05:00:41 GMT  
		Size: 55.1 MB (55056714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1459d3ab8b5e46ac1a0a00134fe2f7b693474eb6d75ace97ecbe811a6f5b0e`  
		Last Modified: Wed, 20 Sep 2023 09:31:06 GMT  
		Size: 15.8 MB (15760408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab00e7798a04602c3f6e2dc445a994d75e96c45533cd44701f58509982a8c5`  
		Last Modified: Wed, 20 Sep 2023 09:31:23 GMT  
		Size: 54.6 MB (54584790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7883a473306cf6632abe7e913e0f1a21ac2fed038a4116473b25738b8b88b294`  
		Last Modified: Wed, 20 Sep 2023 09:31:55 GMT  
		Size: 196.8 MB (196842512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ab175b762c07a73f43bc078229d225d45a4810a8f4e8cb19602122986eadb5`  
		Last Modified: Wed, 20 Sep 2023 12:17:10 GMT  
		Size: 6.3 MB (6291084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19164320e566edd82bea237a00344772e5cdaceb1c0581eab62ea66b8a812d5c`  
		Last Modified: Tue, 03 Oct 2023 03:58:29 GMT  
		Size: 20.1 MB (20053476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccfa8e20789038925a7a0ac61d49b8337c2ff7f1b923e8190271a936e206413e`  
		Last Modified: Tue, 03 Oct 2023 03:58:26 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a5bfb4de08e5dbf05e323300db82d3423385e2e4a87ff92c93574cfe940306`  
		Last Modified: Tue, 03 Oct 2023 03:58:26 GMT  
		Size: 3.1 MB (3109666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2853480534c9003652abee52b8564d53ec16ae60da13fdca042d57b323bab888`  
		Last Modified: Tue, 03 Oct 2023 04:29:10 GMT  
		Size: 7.5 MB (7479231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d411f454564bf8a14d13d91dcef8dec6c34ec244c7580c88c8a1d529f08b848`  
		Last Modified: Tue, 03 Oct 2023 04:29:08 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14417cd73e58663a678f0c5a0fce443306ffd56f455e0d42c0264ef51dfadc2a`  
		Last Modified: Tue, 03 Oct 2023 04:29:08 GMT  
		Size: 1.5 KB (1464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:1.31.0-python3.11` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:6fed15916314569b43402551b06ad9ecde8957e827a4628b195d31304271e3ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.7 MB (350717878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:705609da8fdf387160dd80f7413f642a4b06072f958b38bbd8c0137df5d6db1b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:20 GMT
ADD file:46dcdcde338d2c01fed5db3fac9041736d9305145d8fc2039dd5b3714d38ede8 in / 
# Wed, 20 Sep 2023 02:44:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:24:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:25:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:26:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 02 Oct 2023 16:48:26 GMT
ENV LANG=C.UTF-8
# Mon, 02 Oct 2023 16:48:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 02 Oct 2023 16:48:26 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_VERSION=3.11.6
# Mon, 02 Oct 2023 16:48:26 GMT
RUN set -eux; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		bin="$(readlink -ve /usr/local/bin/python3)"; 	dir="$(dirname "$bin")"; 	mkdir -p "/usr/share/gdb/auto-load/$dir"; 	cp -vL Tools/gdb/libpython.py "/usr/share/gdb/auto-load/$bin-gdb.py"; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		python3 --version # buildkit
# Mon, 02 Oct 2023 16:48:26 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_PIP_VERSION=23.2.1
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/9af82b715db434abb94a0a6f3569f43e72157346/public/get-pip.py
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_GET_PIP_SHA256=45a2bb8bf2bb5eff16fdd00faef6f29731831c7c59bd9fc2bf1f3bed511ff1fe
# Mon, 02 Oct 2023 16:48:26 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Mon, 02 Oct 2023 16:48:26 GMT
CMD ["python3"]
# Tue, 03 Oct 2023 04:37:55 GMT
LABEL org.opencontainers.image.title=Unit (python3.11)
# Tue, 03 Oct 2023 04:37:55 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Tue, 03 Oct 2023 04:37:55 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Tue, 03 Oct 2023 04:37:55 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Tue, 03 Oct 2023 04:37:55 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Tue, 03 Oct 2023 04:37:56 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 03 Oct 2023 04:37:56 GMT
LABEL org.opencontainers.image.version=1.31.0
# Tue, 03 Oct 2023 04:38:36 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure python --config=/usr/local/bin/python3-config     && make -j $NCPU python3-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure python --config=/usr/local/bin/python3-config     && make -j $NCPU python3-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Tue, 03 Oct 2023 04:38:36 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Tue, 03 Oct 2023 04:38:36 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Tue, 03 Oct 2023 04:38:36 GMT
STOPSIGNAL SIGTERM
# Tue, 03 Oct 2023 04:38:37 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 03 Oct 2023 04:38:37 GMT
EXPOSE 80
# Tue, 03 Oct 2023 04:38:37 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:31f5dc1f52c865588c43d8ec718f14d430e149b28f0b28232da825da7ae28f76`  
		Last Modified: Wed, 20 Sep 2023 02:47:53 GMT  
		Size: 53.7 MB (53704892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb60045eb75c62e890b95d28e4893132a6c7d61ec9979104ee4ff6e86c4badee`  
		Last Modified: Wed, 20 Sep 2023 09:33:11 GMT  
		Size: 15.7 MB (15746671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292737ab468ef80c6f78bdde4896157b8953d1e5556e1e526f40aeadcb547573`  
		Last Modified: Wed, 20 Sep 2023 09:33:26 GMT  
		Size: 54.7 MB (54676309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d93979d624211374be152eee1c99ed4ca9e6bae68694135fc440ab6c8fd2044`  
		Last Modified: Wed, 20 Sep 2023 09:33:51 GMT  
		Size: 189.8 MB (189778334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a9f8670f1b8c5bf3a5389568c9f40d95526c380daa5b707640ce7a9be9076c4`  
		Last Modified: Wed, 20 Sep 2023 21:58:21 GMT  
		Size: 6.4 MB (6405066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4ee3feee6bb07e1e690530f4073cefe52850fc7ce215c60cde9f743293dd97`  
		Last Modified: Tue, 03 Oct 2023 04:12:56 GMT  
		Size: 19.9 MB (19937158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4091e9efdd6b4028377199af2b8bac46c9f271309e560152e21888f5d7f4ad0b`  
		Last Modified: Tue, 03 Oct 2023 04:12:53 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306fc013432d7365870d985fbeb02a5ea64cd70a0ff047dae8f958b3fa1b944e`  
		Last Modified: Tue, 03 Oct 2023 04:12:54 GMT  
		Size: 3.1 MB (3109607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e94fb5ebc22b2c1377eb006509be69bc493b269685b3dac417cdfbbe99501a`  
		Last Modified: Tue, 03 Oct 2023 04:39:18 GMT  
		Size: 7.4 MB (7356865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1c327971a0e691baac3b8e16245c90d68517bdd5ebd62c8672c393b21007ab`  
		Last Modified: Tue, 03 Oct 2023 04:39:16 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36b452cc0eb4a32a12308190469a5a96a527d292337bf035d0bdd865341fa34`  
		Last Modified: Tue, 03 Oct 2023 04:39:17 GMT  
		Size: 1.5 KB (1468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `unit:1.31.0-ruby3.2`

```console
$ docker pull unit@sha256:a5e6024510f124beb927b8856bbb21d3b41fc416478cf5a804c07f113e842f60
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:1.31.0-ruby3.2` - linux; amd64

```console
$ docker pull unit@sha256:956602c398b9f70c86add7421abf3c9cc2d2d2a5cff956bb5e88e8fd7302d344
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **364.3 MB (364275696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3213b761cda6d5ab61d82cffa6ccb864a779fd8d19fe7dd1c5e2b75e19fb987d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 04:55:51 GMT
ADD file:85db4f4c5016f51f7112a5d09cb7d4620f565a1379ae4b8a03c5ffc23886a876 in / 
# Wed, 20 Sep 2023 04:55:51 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:22:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:22:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:23:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 04:11:30 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 21 Sep 2023 04:11:30 GMT
ENV LANG=C.UTF-8
# Thu, 21 Sep 2023 04:18:56 GMT
ENV RUBY_MAJOR=3.2
# Thu, 21 Sep 2023 04:18:56 GMT
ENV RUBY_VERSION=3.2.2
# Thu, 21 Sep 2023 04:18:56 GMT
ENV RUBY_DOWNLOAD_SHA256=4b352d0f7ec384e332e3e44cdbfdcd5ff2d594af3c8296b5636c710975149e23
# Thu, 21 Sep 2023 04:21:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		rustArch=; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		'amd64') rustArch='x86_64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/x86_64-unknown-linux-gnu/rustup-init'; rustupSha256='5cc9ffd1026e82e7fb2eec2121ad71f4b0f044e88bca39207b3f6b769aaa799c' ;; 		'arm64') rustArch='aarch64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/aarch64-unknown-linux-gnu/rustup-init'; rustupSha256='e189948e396d47254103a49c987e7fb0e5dd8e34b200aa4481ecc4b8e41fb929' ;; 	esac; 		if [ -n "$rustArch" ]; then 		mkdir -p /tmp/rust; 				wget -O /tmp/rust/rustup-init "$rustupUrl"; 		echo "$rustupSha256 */tmp/rust/rustup-init" | sha256sum --check --strict; 		chmod +x /tmp/rust/rustup-init; 				export RUSTUP_HOME='/tmp/rust/rustup' CARGO_HOME='/tmp/rust/cargo'; 		export PATH="$CARGO_HOME/bin:$PATH"; 		/tmp/rust/rustup-init -y --no-modify-path --profile minimal --default-toolchain '1.66.0' --default-host "$rustArch"; 				rustc --version; 		cargo --version; 	fi; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 		${rustArch:+--enable-yjit} 	; 	make -j "$(nproc)"; 	make install; 		rm -rf /tmp/rust; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 21 Sep 2023 04:21:13 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 21 Sep 2023 04:21:13 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 21 Sep 2023 04:21:13 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 21 Sep 2023 04:21:13 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 21 Sep 2023 04:21:14 GMT
CMD ["irb"]
# Thu, 21 Sep 2023 09:01:40 GMT
LABEL org.opencontainers.image.title=Unit (ruby3.2)
# Thu, 21 Sep 2023 09:01:40 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Thu, 21 Sep 2023 09:01:40 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Thu, 21 Sep 2023 09:01:40 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Thu, 21 Sep 2023 09:01:40 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Thu, 21 Sep 2023 09:01:41 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Thu, 21 Sep 2023 09:01:41 GMT
LABEL org.opencontainers.image.version=1.31.0
# Thu, 21 Sep 2023 09:02:33 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure ruby     && make -j $NCPU ruby-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure ruby     && make -j $NCPU ruby-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && gem install rack && rm -rf /root/.local     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Thu, 21 Sep 2023 09:02:33 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Thu, 21 Sep 2023 09:02:33 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Thu, 21 Sep 2023 09:02:33 GMT
STOPSIGNAL SIGTERM
# Thu, 21 Sep 2023 09:02:33 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 21 Sep 2023 09:02:34 GMT
EXPOSE 80
# Thu, 21 Sep 2023 09:02:34 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:ddf874abf16cc990e0fd75a154a34ca0a03ee310ad895a18fb62ae15bf4171fb`  
		Last Modified: Wed, 20 Sep 2023 05:00:41 GMT  
		Size: 55.1 MB (55056714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1459d3ab8b5e46ac1a0a00134fe2f7b693474eb6d75ace97ecbe811a6f5b0e`  
		Last Modified: Wed, 20 Sep 2023 09:31:06 GMT  
		Size: 15.8 MB (15760408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab00e7798a04602c3f6e2dc445a994d75e96c45533cd44701f58509982a8c5`  
		Last Modified: Wed, 20 Sep 2023 09:31:23 GMT  
		Size: 54.6 MB (54584790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7883a473306cf6632abe7e913e0f1a21ac2fed038a4116473b25738b8b88b294`  
		Last Modified: Wed, 20 Sep 2023 09:31:55 GMT  
		Size: 196.8 MB (196842512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fdcd138618aab34068d5f25a76b9f52fd31968b0ac18bb7d07712e2dfb218da`  
		Last Modified: Thu, 21 Sep 2023 04:31:31 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a1c513a65f8aa3521e033b2594828b7458e09a64b409ae0c845fa78f54dbee`  
		Last Modified: Thu, 21 Sep 2023 04:32:15 GMT  
		Size: 34.6 MB (34555434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef736a5e310922df2e0ec8fea9b8cb6e82f6e05b6728246464e80cbd3323463`  
		Last Modified: Thu, 21 Sep 2023 04:32:12 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852f8560c08590962b1223b1b4098e276106212ed51b79cce0f8c8cc3c7ecf03`  
		Last Modified: Thu, 21 Sep 2023 09:03:59 GMT  
		Size: 7.5 MB (7472725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:355dd321857fb6ccef83d972ba26481615db92cda9272569c448f690bd3caaba`  
		Last Modified: Thu, 21 Sep 2023 09:03:57 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539417e59f1725542c24856f19c2f2a3348df4e315ef3336ff577fa9e163a913`  
		Last Modified: Thu, 21 Sep 2023 09:03:57 GMT  
		Size: 1.5 KB (1464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:1.31.0-ruby3.2` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:dffefd84552257cf59dee4bbe3e0bb6c1d278ea4149b15d4e9839dddd4e1dd05
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.7 MB (355686533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d01d684dd22e47a20187d814ce3077e56cffccc53f1a3681e112e1e6dd9c68e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:20 GMT
ADD file:46dcdcde338d2c01fed5db3fac9041736d9305145d8fc2039dd5b3714d38ede8 in / 
# Wed, 20 Sep 2023 02:44:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:24:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:25:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:26:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 17:00:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 20 Sep 2023 17:00:09 GMT
ENV LANG=C.UTF-8
# Wed, 20 Sep 2023 17:12:43 GMT
ENV RUBY_MAJOR=3.2
# Wed, 20 Sep 2023 17:12:43 GMT
ENV RUBY_VERSION=3.2.2
# Wed, 20 Sep 2023 17:12:43 GMT
ENV RUBY_DOWNLOAD_SHA256=4b352d0f7ec384e332e3e44cdbfdcd5ff2d594af3c8296b5636c710975149e23
# Wed, 20 Sep 2023 17:14:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		rustArch=; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		'amd64') rustArch='x86_64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/x86_64-unknown-linux-gnu/rustup-init'; rustupSha256='5cc9ffd1026e82e7fb2eec2121ad71f4b0f044e88bca39207b3f6b769aaa799c' ;; 		'arm64') rustArch='aarch64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/aarch64-unknown-linux-gnu/rustup-init'; rustupSha256='e189948e396d47254103a49c987e7fb0e5dd8e34b200aa4481ecc4b8e41fb929' ;; 	esac; 		if [ -n "$rustArch" ]; then 		mkdir -p /tmp/rust; 				wget -O /tmp/rust/rustup-init "$rustupUrl"; 		echo "$rustupSha256 */tmp/rust/rustup-init" | sha256sum --check --strict; 		chmod +x /tmp/rust/rustup-init; 				export RUSTUP_HOME='/tmp/rust/rustup' CARGO_HOME='/tmp/rust/cargo'; 		export PATH="$CARGO_HOME/bin:$PATH"; 		/tmp/rust/rustup-init -y --no-modify-path --profile minimal --default-toolchain '1.66.0' --default-host "$rustArch"; 				rustc --version; 		cargo --version; 	fi; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 		${rustArch:+--enable-yjit} 	; 	make -j "$(nproc)"; 	make install; 		rm -rf /tmp/rust; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 20 Sep 2023 17:14:28 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 20 Sep 2023 17:14:28 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 20 Sep 2023 17:14:28 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Sep 2023 17:14:28 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Wed, 20 Sep 2023 17:14:29 GMT
CMD ["irb"]
# Thu, 21 Sep 2023 03:27:09 GMT
LABEL org.opencontainers.image.title=Unit (ruby3.2)
# Thu, 21 Sep 2023 03:27:09 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Thu, 21 Sep 2023 03:27:09 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Thu, 21 Sep 2023 03:27:09 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Thu, 21 Sep 2023 03:27:09 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Thu, 21 Sep 2023 03:27:09 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Thu, 21 Sep 2023 03:27:10 GMT
LABEL org.opencontainers.image.version=1.31.0
# Thu, 21 Sep 2023 03:27:51 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure ruby     && make -j $NCPU ruby-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure ruby     && make -j $NCPU ruby-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && gem install rack && rm -rf /root/.local     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Thu, 21 Sep 2023 03:27:51 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Thu, 21 Sep 2023 03:27:51 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Thu, 21 Sep 2023 03:27:51 GMT
STOPSIGNAL SIGTERM
# Thu, 21 Sep 2023 03:27:51 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 21 Sep 2023 03:27:51 GMT
EXPOSE 80
# Thu, 21 Sep 2023 03:27:51 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:31f5dc1f52c865588c43d8ec718f14d430e149b28f0b28232da825da7ae28f76`  
		Last Modified: Wed, 20 Sep 2023 02:47:53 GMT  
		Size: 53.7 MB (53704892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb60045eb75c62e890b95d28e4893132a6c7d61ec9979104ee4ff6e86c4badee`  
		Last Modified: Wed, 20 Sep 2023 09:33:11 GMT  
		Size: 15.7 MB (15746671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292737ab468ef80c6f78bdde4896157b8953d1e5556e1e526f40aeadcb547573`  
		Last Modified: Wed, 20 Sep 2023 09:33:26 GMT  
		Size: 54.7 MB (54676309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d93979d624211374be152eee1c99ed4ca9e6bae68694135fc440ab6c8fd2044`  
		Last Modified: Wed, 20 Sep 2023 09:33:51 GMT  
		Size: 189.8 MB (189778334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b301519822ecf9e91a1d73928dcd311c4bca39d7dc3c8312271a3a87192b6fad`  
		Last Modified: Wed, 20 Sep 2023 17:32:40 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83bd254efa556fb8118a65fd122dfaebb9beb925b07e4bce5dab0753adfe612b`  
		Last Modified: Wed, 20 Sep 2023 17:33:59 GMT  
		Size: 34.4 MB (34432616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf0bf0364fef8b7d14832a31609b05b197fc4cd485098cba635e2dcc48c3a18`  
		Last Modified: Wed, 20 Sep 2023 17:33:56 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddcc516d1030a5cfc66d59f54ada76bc9df6bbc565d4b0e7d2f5f0b7dfcdc755`  
		Last Modified: Thu, 21 Sep 2023 03:29:08 GMT  
		Size: 7.3 MB (7344596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3698a78d8a3fbcff7cc1793bf3bae553dfb607bc4135436e5699d758d6b3b7`  
		Last Modified: Thu, 21 Sep 2023 03:29:07 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7a2e346b9c5a6b73c465209726bfa46af845b73807df32c3a5ac350195ab35`  
		Last Modified: Thu, 21 Sep 2023 03:29:07 GMT  
		Size: 1.5 KB (1469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `unit:1.31.0-wasm`

```console
$ docker pull unit@sha256:d2890c56bd6ed1c9cf1aca41dbca04209c01a40d85a244061b4ebb9a920c9953
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:1.31.0-wasm` - linux; amd64

```console
$ docker pull unit@sha256:7845aa107eff2617b276695e1df86a4761833df366dc4bb223ba13933d9bfd60
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.6 MB (46636244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc633f872efe837e4e06cf567ac808a1e1112294f079c42992cb2c64228fbb2c`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:53:19 GMT
LABEL org.opencontainers.image.title=Unit (wasm)
# Wed, 11 Oct 2023 19:53:19 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Wed, 11 Oct 2023 19:53:19 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Wed, 11 Oct 2023 19:53:19 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Wed, 11 Oct 2023 19:53:19 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Wed, 11 Oct 2023 19:53:19 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 11 Oct 2023 19:53:19 GMT
LABEL org.opencontainers.image.version=1.31.0
# Wed, 11 Oct 2023 19:56:46 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && export RUST_VERSION=1.71.0     && export RUSTUP_HOME=/usr/src/unit/rustup     && export CARGO_HOME=/usr/src/unit/cargo     && export PATH=/usr/src/unit/cargo/bin:$PATH     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in        amd64) rustArch="x86_64-unknown-linux-gnu"; rustupSha256="0b2f6c8f85a3d02fde2efc0ced4657869d73fccfce59defb4e8d29233116e6db" ;;        arm64) rustArch="aarch64-unknown-linux-gnu"; rustupSha256="673e336c81c65e6b16dcdede33f4cc9ed0f08bde1dbe7a935f113605292dc800" ;;        *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac     && url="https://static.rust-lang.org/rustup/archive/1.26.0/${rustArch}/rustup-init"     && curl -L -O "$url"     && echo "${rustupSha256} *rustup-init" | sha256sum -c -     && chmod +x rustup-init     && ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch}     && rm rustup-init     && rustup --version     && cargo --version     && rustc --version     && make -C pkg/contrib .wasmtime     && install -pm 755 pkg/contrib/wasmtime/target/release/libwasmtime.so /usr/lib/$(dpkg-architecture -q DEB_HOST_MULTIARCH)/     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure wasm --include-path=`pwd`/pkg/contrib/wasmtime/crates/c-api/include --lib-path=/usr/lib/$(dpkg-architecture -q DEB_HOST_MULTIARCH)/     && make -j $NCPU wasm-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure wasm --include-path=`pwd`/pkg/contrib/wasmtime/crates/c-api/include --lib-path=/usr/lib/$(dpkg-architecture -q DEB_HOST_MULTIARCH)/     && make -j $NCPU wasm-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Wed, 11 Oct 2023 19:56:47 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Wed, 11 Oct 2023 19:56:47 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Wed, 11 Oct 2023 19:56:47 GMT
STOPSIGNAL SIGTERM
# Wed, 11 Oct 2023 19:56:47 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Wed, 11 Oct 2023 19:56:47 GMT
EXPOSE 80
# Wed, 11 Oct 2023 19:56:47 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9141e09d044816697e52a2955dde172af5396e3c8c1b71153d67f668fa2454`  
		Last Modified: Wed, 11 Oct 2023 19:59:04 GMT  
		Size: 15.2 MB (15215650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5496485089c9075d6a558dcb20d3f86e3c90425b983f76abe65188304e9d4de2`  
		Last Modified: Wed, 11 Oct 2023 19:59:02 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc28d01cbfd6ee3775e414c61a1ae5f000333baff83a6a33eeae1c6bd4ae127`  
		Last Modified: Wed, 11 Oct 2023 19:59:01 GMT  
		Size: 1.5 KB (1469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:1.31.0-wasm` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:9102091e8f914725b06d7bf804d4ec19ac5aff70fe98b70bbbee6b756d9311fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (45044027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe1be587ad1f9b09ad9fbacb9c77ad16d6790b59be9d324f0613bb128f684bb1`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:06 GMT
ADD file:2c3e5451390c62f0b85f20139d2c88011cc54d649cdda5567084c050ad373372 in / 
# Wed, 11 Oct 2023 18:25:06 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:09:12 GMT
LABEL org.opencontainers.image.title=Unit (wasm)
# Wed, 11 Oct 2023 19:09:12 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Wed, 11 Oct 2023 19:09:12 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Wed, 11 Oct 2023 19:09:12 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Wed, 11 Oct 2023 19:09:12 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Wed, 11 Oct 2023 19:09:12 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 11 Oct 2023 19:09:12 GMT
LABEL org.opencontainers.image.version=1.31.0
# Wed, 11 Oct 2023 19:12:13 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && export RUST_VERSION=1.71.0     && export RUSTUP_HOME=/usr/src/unit/rustup     && export CARGO_HOME=/usr/src/unit/cargo     && export PATH=/usr/src/unit/cargo/bin:$PATH     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in        amd64) rustArch="x86_64-unknown-linux-gnu"; rustupSha256="0b2f6c8f85a3d02fde2efc0ced4657869d73fccfce59defb4e8d29233116e6db" ;;        arm64) rustArch="aarch64-unknown-linux-gnu"; rustupSha256="673e336c81c65e6b16dcdede33f4cc9ed0f08bde1dbe7a935f113605292dc800" ;;        *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac     && url="https://static.rust-lang.org/rustup/archive/1.26.0/${rustArch}/rustup-init"     && curl -L -O "$url"     && echo "${rustupSha256} *rustup-init" | sha256sum -c -     && chmod +x rustup-init     && ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch}     && rm rustup-init     && rustup --version     && cargo --version     && rustc --version     && make -C pkg/contrib .wasmtime     && install -pm 755 pkg/contrib/wasmtime/target/release/libwasmtime.so /usr/lib/$(dpkg-architecture -q DEB_HOST_MULTIARCH)/     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure wasm --include-path=`pwd`/pkg/contrib/wasmtime/crates/c-api/include --lib-path=/usr/lib/$(dpkg-architecture -q DEB_HOST_MULTIARCH)/     && make -j $NCPU wasm-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure wasm --include-path=`pwd`/pkg/contrib/wasmtime/crates/c-api/include --lib-path=/usr/lib/$(dpkg-architecture -q DEB_HOST_MULTIARCH)/     && make -j $NCPU wasm-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Wed, 11 Oct 2023 19:12:13 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Wed, 11 Oct 2023 19:12:13 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Wed, 11 Oct 2023 19:12:13 GMT
STOPSIGNAL SIGTERM
# Wed, 11 Oct 2023 19:12:13 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Wed, 11 Oct 2023 19:12:13 GMT
EXPOSE 80
# Wed, 11 Oct 2023 19:12:13 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:85e50d2242ceaba78c3726e059dbd2fa06f5c18e265554bd43a482d19b256d20`  
		Last Modified: Wed, 11 Oct 2023 18:29:07 GMT  
		Size: 30.1 MB (30064086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45870802cfcb84d8f28e525b07f1ab49e3705abd7690bd264c17e773986e6f2d`  
		Last Modified: Wed, 11 Oct 2023 19:14:06 GMT  
		Size: 15.0 MB (14977210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956d6f6dc5a165b604bdd1af481715ae8e2c40783e5ef4dfaf6780a8c91d0d45`  
		Last Modified: Wed, 11 Oct 2023 19:14:04 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51670beaa1ab175b4fc1b8b985cf32289b45e63df30ec8f98eae0f51506a3c3`  
		Last Modified: Wed, 11 Oct 2023 19:14:04 GMT  
		Size: 1.5 KB (1470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `unit:go`

```console
$ docker pull unit@sha256:b9c9ddcce8c48adfce8f29648cdc7739cc01f07d86354fd751cb8728bc521186
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:go` - linux; amd64

```console
$ docker pull unit@sha256:e25c525607700cb9afff5bf7ba2516c4af8a99eb8c374d614b52840ab4d2012a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.8 MB (299846746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0fba295b6f441f9cc6a84818fd1d58b0c3a5345fc0684fd72ab87fac731bc9f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 04:55:51 GMT
ADD file:85db4f4c5016f51f7112a5d09cb7d4620f565a1379ae4b8a03c5ffc23886a876 in / 
# Wed, 20 Sep 2023 04:55:51 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:22:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:22:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 03:29:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 03:29:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:19:57 GMT
ENV GOLANG_VERSION=1.21.3
# Tue, 10 Oct 2023 19:20:06 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.3.linux-mips64le.tar.gz'; 			sha256='a569ffbc88b4e14cf2682f65cec950460665e4392b0d78b8868b4718c979bda8'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 10 Oct 2023 19:20:07 GMT
ENV GOTOOLCHAIN=local
# Tue, 10 Oct 2023 19:20:07 GMT
ENV GOPATH=/go
# Tue, 10 Oct 2023 19:20:07 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:20:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 10 Oct 2023 19:20:07 GMT
WORKDIR /go
# Tue, 10 Oct 2023 19:45:00 GMT
LABEL org.opencontainers.image.title=Unit (go1.21)
# Tue, 10 Oct 2023 19:45:00 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Tue, 10 Oct 2023 19:45:00 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Tue, 10 Oct 2023 19:45:00 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Tue, 10 Oct 2023 19:45:00 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Tue, 10 Oct 2023 19:45:00 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 10 Oct 2023 19:45:00 GMT
LABEL org.opencontainers.image.version=1.31.0
# Tue, 10 Oct 2023 19:45:58 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure go --go-path=$GOPATH     && make -j $NCPU go-install-src libunit-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure go --go-path=$GOPATH     && make -j $NCPU go-install-src libunit-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Tue, 10 Oct 2023 19:45:59 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Tue, 10 Oct 2023 19:45:59 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Tue, 10 Oct 2023 19:45:59 GMT
STOPSIGNAL SIGTERM
# Tue, 10 Oct 2023 19:45:59 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 10 Oct 2023 19:45:59 GMT
EXPOSE 80
# Tue, 10 Oct 2023 19:45:59 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:ddf874abf16cc990e0fd75a154a34ca0a03ee310ad895a18fb62ae15bf4171fb`  
		Last Modified: Wed, 20 Sep 2023 05:00:41 GMT  
		Size: 55.1 MB (55056714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1459d3ab8b5e46ac1a0a00134fe2f7b693474eb6d75ace97ecbe811a6f5b0e`  
		Last Modified: Wed, 20 Sep 2023 09:31:06 GMT  
		Size: 15.8 MB (15760408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab00e7798a04602c3f6e2dc445a994d75e96c45533cd44701f58509982a8c5`  
		Last Modified: Wed, 20 Sep 2023 09:31:23 GMT  
		Size: 54.6 MB (54584790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9036a471a1c45233bf72245ae53bd00fd2b25cbdf75be2cafe1c6fd91309cdb7`  
		Last Modified: Thu, 21 Sep 2023 03:31:14 GMT  
		Size: 86.1 MB (86068436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a30056caa3534c4f704e37958c32100b96aa5535fff9af405b5bf4cd272e158`  
		Last Modified: Tue, 10 Oct 2023 19:25:53 GMT  
		Size: 67.0 MB (67001246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca402200ac32a0f6d38fdcae01d58d804e90543fabef314c0aaa4731ac3f9b6`  
		Last Modified: Tue, 10 Oct 2023 19:25:42 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62756cd2c6f084fd53a983f51ef7d6c5b3d9ef2f80d2fc122550940332ad324`  
		Last Modified: Tue, 10 Oct 2023 19:48:08 GMT  
		Size: 21.4 MB (21372254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13a00f1dc20f8f2006ac8c9b1c91c322d352fd41f2b3a41e00fb8bba12e3534`  
		Last Modified: Tue, 10 Oct 2023 19:48:05 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533fb155fbc122a1435f260e62b8f43d7de9a2c0675df5ecf4b5bc1a6f4d93ed`  
		Last Modified: Tue, 10 Oct 2023 19:48:05 GMT  
		Size: 1.5 KB (1470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:go` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:8a3b8f2b9a104a7bab667ab4a73ad407817aab9ec14cb264a3e2df2814cf8b6a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289268520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9020087609178de15b4aea74b2bfc5530c392b2d08c4661713cdad84547c7415`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:20 GMT
ADD file:46dcdcde338d2c01fed5db3fac9041736d9305145d8fc2039dd5b3714d38ede8 in / 
# Wed, 20 Sep 2023 02:44:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:24:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:25:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 22:20:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 22:20:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:39:44 GMT
ENV GOLANG_VERSION=1.21.3
# Tue, 10 Oct 2023 19:39:52 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.3.linux-mips64le.tar.gz'; 			sha256='a569ffbc88b4e14cf2682f65cec950460665e4392b0d78b8868b4718c979bda8'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 10 Oct 2023 19:39:53 GMT
ENV GOTOOLCHAIN=local
# Tue, 10 Oct 2023 19:39:54 GMT
ENV GOPATH=/go
# Tue, 10 Oct 2023 19:39:54 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:39:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 10 Oct 2023 19:39:54 GMT
WORKDIR /go
# Tue, 10 Oct 2023 20:02:25 GMT
LABEL org.opencontainers.image.title=Unit (go1.21)
# Tue, 10 Oct 2023 20:02:25 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Tue, 10 Oct 2023 20:02:25 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Tue, 10 Oct 2023 20:02:25 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Tue, 10 Oct 2023 20:02:26 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Tue, 10 Oct 2023 20:02:26 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 10 Oct 2023 20:02:26 GMT
LABEL org.opencontainers.image.version=1.31.0
# Tue, 10 Oct 2023 20:03:13 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure go --go-path=$GOPATH     && make -j $NCPU go-install-src libunit-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure go --go-path=$GOPATH     && make -j $NCPU go-install-src libunit-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Tue, 10 Oct 2023 20:03:13 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Tue, 10 Oct 2023 20:03:13 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Tue, 10 Oct 2023 20:03:13 GMT
STOPSIGNAL SIGTERM
# Tue, 10 Oct 2023 20:03:13 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 10 Oct 2023 20:03:13 GMT
EXPOSE 80
# Tue, 10 Oct 2023 20:03:14 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:31f5dc1f52c865588c43d8ec718f14d430e149b28f0b28232da825da7ae28f76`  
		Last Modified: Wed, 20 Sep 2023 02:47:53 GMT  
		Size: 53.7 MB (53704892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb60045eb75c62e890b95d28e4893132a6c7d61ec9979104ee4ff6e86c4badee`  
		Last Modified: Wed, 20 Sep 2023 09:33:11 GMT  
		Size: 15.7 MB (15746671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292737ab468ef80c6f78bdde4896157b8953d1e5556e1e526f40aeadcb547573`  
		Last Modified: Wed, 20 Sep 2023 09:33:26 GMT  
		Size: 54.7 MB (54676309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486d7167072fd25b2d2370fbba8326b8059274be0fa615a14d3e975fe46f1b4f`  
		Last Modified: Wed, 20 Sep 2023 22:21:57 GMT  
		Size: 81.5 MB (81468116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1306584d039cecaec0b207b88108f8c03ec361f1cf8015ae4ba23ec3c9406f50`  
		Last Modified: Tue, 10 Oct 2023 19:44:41 GMT  
		Size: 64.1 MB (64098318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815863143577abf9b2b650b8a28f205bfc32287c17ee2b8c0e8a8155b2a75ca3`  
		Last Modified: Tue, 10 Oct 2023 19:44:28 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd1b8471a82b8fb80921156f2b1abe4b85e1db1756650baa8a63c94cdb72a9ac`  
		Last Modified: Tue, 10 Oct 2023 20:05:01 GMT  
		Size: 19.6 MB (19571320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e45a03b84b12daccf9bbc14746f689f1d235d2526a77c4fa8e26e9e97ca6ff0`  
		Last Modified: Tue, 10 Oct 2023 20:04:58 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc16a37f4406cdb2846b682b8e11e00ea46efd01c2826567faa97e87146f0f20`  
		Last Modified: Tue, 10 Oct 2023 20:04:58 GMT  
		Size: 1.5 KB (1467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `unit:go1`

```console
$ docker pull unit@sha256:b9c9ddcce8c48adfce8f29648cdc7739cc01f07d86354fd751cb8728bc521186
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:go1` - linux; amd64

```console
$ docker pull unit@sha256:e25c525607700cb9afff5bf7ba2516c4af8a99eb8c374d614b52840ab4d2012a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.8 MB (299846746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0fba295b6f441f9cc6a84818fd1d58b0c3a5345fc0684fd72ab87fac731bc9f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 04:55:51 GMT
ADD file:85db4f4c5016f51f7112a5d09cb7d4620f565a1379ae4b8a03c5ffc23886a876 in / 
# Wed, 20 Sep 2023 04:55:51 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:22:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:22:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 03:29:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 03:29:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:19:57 GMT
ENV GOLANG_VERSION=1.21.3
# Tue, 10 Oct 2023 19:20:06 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.3.linux-mips64le.tar.gz'; 			sha256='a569ffbc88b4e14cf2682f65cec950460665e4392b0d78b8868b4718c979bda8'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 10 Oct 2023 19:20:07 GMT
ENV GOTOOLCHAIN=local
# Tue, 10 Oct 2023 19:20:07 GMT
ENV GOPATH=/go
# Tue, 10 Oct 2023 19:20:07 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:20:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 10 Oct 2023 19:20:07 GMT
WORKDIR /go
# Tue, 10 Oct 2023 19:45:00 GMT
LABEL org.opencontainers.image.title=Unit (go1.21)
# Tue, 10 Oct 2023 19:45:00 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Tue, 10 Oct 2023 19:45:00 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Tue, 10 Oct 2023 19:45:00 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Tue, 10 Oct 2023 19:45:00 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Tue, 10 Oct 2023 19:45:00 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 10 Oct 2023 19:45:00 GMT
LABEL org.opencontainers.image.version=1.31.0
# Tue, 10 Oct 2023 19:45:58 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure go --go-path=$GOPATH     && make -j $NCPU go-install-src libunit-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure go --go-path=$GOPATH     && make -j $NCPU go-install-src libunit-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Tue, 10 Oct 2023 19:45:59 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Tue, 10 Oct 2023 19:45:59 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Tue, 10 Oct 2023 19:45:59 GMT
STOPSIGNAL SIGTERM
# Tue, 10 Oct 2023 19:45:59 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 10 Oct 2023 19:45:59 GMT
EXPOSE 80
# Tue, 10 Oct 2023 19:45:59 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:ddf874abf16cc990e0fd75a154a34ca0a03ee310ad895a18fb62ae15bf4171fb`  
		Last Modified: Wed, 20 Sep 2023 05:00:41 GMT  
		Size: 55.1 MB (55056714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1459d3ab8b5e46ac1a0a00134fe2f7b693474eb6d75ace97ecbe811a6f5b0e`  
		Last Modified: Wed, 20 Sep 2023 09:31:06 GMT  
		Size: 15.8 MB (15760408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab00e7798a04602c3f6e2dc445a994d75e96c45533cd44701f58509982a8c5`  
		Last Modified: Wed, 20 Sep 2023 09:31:23 GMT  
		Size: 54.6 MB (54584790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9036a471a1c45233bf72245ae53bd00fd2b25cbdf75be2cafe1c6fd91309cdb7`  
		Last Modified: Thu, 21 Sep 2023 03:31:14 GMT  
		Size: 86.1 MB (86068436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a30056caa3534c4f704e37958c32100b96aa5535fff9af405b5bf4cd272e158`  
		Last Modified: Tue, 10 Oct 2023 19:25:53 GMT  
		Size: 67.0 MB (67001246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca402200ac32a0f6d38fdcae01d58d804e90543fabef314c0aaa4731ac3f9b6`  
		Last Modified: Tue, 10 Oct 2023 19:25:42 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62756cd2c6f084fd53a983f51ef7d6c5b3d9ef2f80d2fc122550940332ad324`  
		Last Modified: Tue, 10 Oct 2023 19:48:08 GMT  
		Size: 21.4 MB (21372254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13a00f1dc20f8f2006ac8c9b1c91c322d352fd41f2b3a41e00fb8bba12e3534`  
		Last Modified: Tue, 10 Oct 2023 19:48:05 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533fb155fbc122a1435f260e62b8f43d7de9a2c0675df5ecf4b5bc1a6f4d93ed`  
		Last Modified: Tue, 10 Oct 2023 19:48:05 GMT  
		Size: 1.5 KB (1470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:go1` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:8a3b8f2b9a104a7bab667ab4a73ad407817aab9ec14cb264a3e2df2814cf8b6a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289268520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9020087609178de15b4aea74b2bfc5530c392b2d08c4661713cdad84547c7415`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:20 GMT
ADD file:46dcdcde338d2c01fed5db3fac9041736d9305145d8fc2039dd5b3714d38ede8 in / 
# Wed, 20 Sep 2023 02:44:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:24:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:25:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 22:20:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 22:20:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:39:44 GMT
ENV GOLANG_VERSION=1.21.3
# Tue, 10 Oct 2023 19:39:52 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.3.linux-mips64le.tar.gz'; 			sha256='a569ffbc88b4e14cf2682f65cec950460665e4392b0d78b8868b4718c979bda8'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 10 Oct 2023 19:39:53 GMT
ENV GOTOOLCHAIN=local
# Tue, 10 Oct 2023 19:39:54 GMT
ENV GOPATH=/go
# Tue, 10 Oct 2023 19:39:54 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:39:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 10 Oct 2023 19:39:54 GMT
WORKDIR /go
# Tue, 10 Oct 2023 20:02:25 GMT
LABEL org.opencontainers.image.title=Unit (go1.21)
# Tue, 10 Oct 2023 20:02:25 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Tue, 10 Oct 2023 20:02:25 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Tue, 10 Oct 2023 20:02:25 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Tue, 10 Oct 2023 20:02:26 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Tue, 10 Oct 2023 20:02:26 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 10 Oct 2023 20:02:26 GMT
LABEL org.opencontainers.image.version=1.31.0
# Tue, 10 Oct 2023 20:03:13 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure go --go-path=$GOPATH     && make -j $NCPU go-install-src libunit-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure go --go-path=$GOPATH     && make -j $NCPU go-install-src libunit-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Tue, 10 Oct 2023 20:03:13 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Tue, 10 Oct 2023 20:03:13 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Tue, 10 Oct 2023 20:03:13 GMT
STOPSIGNAL SIGTERM
# Tue, 10 Oct 2023 20:03:13 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 10 Oct 2023 20:03:13 GMT
EXPOSE 80
# Tue, 10 Oct 2023 20:03:14 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:31f5dc1f52c865588c43d8ec718f14d430e149b28f0b28232da825da7ae28f76`  
		Last Modified: Wed, 20 Sep 2023 02:47:53 GMT  
		Size: 53.7 MB (53704892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb60045eb75c62e890b95d28e4893132a6c7d61ec9979104ee4ff6e86c4badee`  
		Last Modified: Wed, 20 Sep 2023 09:33:11 GMT  
		Size: 15.7 MB (15746671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292737ab468ef80c6f78bdde4896157b8953d1e5556e1e526f40aeadcb547573`  
		Last Modified: Wed, 20 Sep 2023 09:33:26 GMT  
		Size: 54.7 MB (54676309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486d7167072fd25b2d2370fbba8326b8059274be0fa615a14d3e975fe46f1b4f`  
		Last Modified: Wed, 20 Sep 2023 22:21:57 GMT  
		Size: 81.5 MB (81468116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1306584d039cecaec0b207b88108f8c03ec361f1cf8015ae4ba23ec3c9406f50`  
		Last Modified: Tue, 10 Oct 2023 19:44:41 GMT  
		Size: 64.1 MB (64098318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815863143577abf9b2b650b8a28f205bfc32287c17ee2b8c0e8a8155b2a75ca3`  
		Last Modified: Tue, 10 Oct 2023 19:44:28 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd1b8471a82b8fb80921156f2b1abe4b85e1db1756650baa8a63c94cdb72a9ac`  
		Last Modified: Tue, 10 Oct 2023 20:05:01 GMT  
		Size: 19.6 MB (19571320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e45a03b84b12daccf9bbc14746f689f1d235d2526a77c4fa8e26e9e97ca6ff0`  
		Last Modified: Tue, 10 Oct 2023 20:04:58 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc16a37f4406cdb2846b682b8e11e00ea46efd01c2826567faa97e87146f0f20`  
		Last Modified: Tue, 10 Oct 2023 20:04:58 GMT  
		Size: 1.5 KB (1467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `unit:go1.20`

```console
$ docker pull unit@sha256:983ac481c876d9a3dbff95fefbffeb722e8c673f91fc6fdaea65f470cbda7227
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:go1.20` - linux; amd64

```console
$ docker pull unit@sha256:95eede34f128ca4a9c7e330a06d5b4b715d5db4efcdf34b09918aea5fdb99fd7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.3 MB (333278660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a816302fbfc02ecd48d477a933362a0443cb9952a0e46e29c844e409dbe2583`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 04:55:51 GMT
ADD file:85db4f4c5016f51f7112a5d09cb7d4620f565a1379ae4b8a03c5ffc23886a876 in / 
# Wed, 20 Sep 2023 04:55:51 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:22:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:22:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 03:29:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 03:29:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:20:57 GMT
ENV GOLANG_VERSION=1.20.10
# Tue, 10 Oct 2023 19:21:08 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.10.linux-amd64.tar.gz'; 			sha256='80d34f1fd74e382d86c2d6102e0e60d4318461a7c2f457ec1efc4042752d4248'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.10.linux-armv6l.tar.gz'; 			sha256='a2229772434dee3dde1e974ef5ae7936160a05a1b82c57cc5c64660479aa98cb'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.10.linux-arm64.tar.gz'; 			sha256='fb3c7e15fc4413c5b81eb9f26dbd7cd4faedd5c720b30fa8e2ff77457f74cab6'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.10.linux-386.tar.gz'; 			sha256='3c918225d22ef5731b63f0426e48614fc05d8da120fc23101639c81ab152e133'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.10.linux-ppc64le.tar.gz'; 			sha256='ebac6e713810174f9ffd7f48c17c373fbf359d50d8e6233b1dfbbdebd524fd1c'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.10.linux-s390x.tar.gz'; 			sha256='fa32588cbdd1e8adfd7e9f1b4ba3f7a8b424f60e90bf2cc4716650374eb459ae'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.10.src.tar.gz'; 		sha256='72d2f51805c47150066c103754c75fddb2c19d48c9219fa33d1e46696c841dbb'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 10 Oct 2023 19:21:09 GMT
ENV GOPATH=/go
# Tue, 10 Oct 2023 19:21:09 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:21:09 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 10 Oct 2023 19:21:09 GMT
WORKDIR /go
# Tue, 10 Oct 2023 19:46:10 GMT
LABEL org.opencontainers.image.title=Unit (go1.20)
# Tue, 10 Oct 2023 19:46:10 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Tue, 10 Oct 2023 19:46:10 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Tue, 10 Oct 2023 19:46:10 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Tue, 10 Oct 2023 19:46:10 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Tue, 10 Oct 2023 19:46:10 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 10 Oct 2023 19:46:10 GMT
LABEL org.opencontainers.image.version=1.31.0
# Tue, 10 Oct 2023 19:47:05 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure go --go-path=$GOPATH     && make -j $NCPU go-install-src libunit-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure go --go-path=$GOPATH     && make -j $NCPU go-install-src libunit-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Tue, 10 Oct 2023 19:47:06 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Tue, 10 Oct 2023 19:47:06 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Tue, 10 Oct 2023 19:47:06 GMT
STOPSIGNAL SIGTERM
# Tue, 10 Oct 2023 19:47:06 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 10 Oct 2023 19:47:06 GMT
EXPOSE 80
# Tue, 10 Oct 2023 19:47:06 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:ddf874abf16cc990e0fd75a154a34ca0a03ee310ad895a18fb62ae15bf4171fb`  
		Last Modified: Wed, 20 Sep 2023 05:00:41 GMT  
		Size: 55.1 MB (55056714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1459d3ab8b5e46ac1a0a00134fe2f7b693474eb6d75ace97ecbe811a6f5b0e`  
		Last Modified: Wed, 20 Sep 2023 09:31:06 GMT  
		Size: 15.8 MB (15760408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab00e7798a04602c3f6e2dc445a994d75e96c45533cd44701f58509982a8c5`  
		Last Modified: Wed, 20 Sep 2023 09:31:23 GMT  
		Size: 54.6 MB (54584790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9036a471a1c45233bf72245ae53bd00fd2b25cbdf75be2cafe1c6fd91309cdb7`  
		Last Modified: Thu, 21 Sep 2023 03:31:14 GMT  
		Size: 86.1 MB (86068436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f860905235a993930bdd0d7418c0d8e87db9d0182e1aefaec8e37c0787579b`  
		Last Modified: Tue, 10 Oct 2023 19:27:37 GMT  
		Size: 100.4 MB (100433184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512a1d11f639f8a1ba9b7b87e551e39cbe3f2824bf2ed122a68981d6815e1a14`  
		Last Modified: Tue, 10 Oct 2023 19:27:24 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16efabcc1bbb8acc14957b20306cfc6b40cef3c4d63ccebfb4a9f800ced9a0b3`  
		Last Modified: Tue, 10 Oct 2023 19:48:25 GMT  
		Size: 21.4 MB (21372238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8c3847df07c19e00cc8dc749aee71a4d25c04ddda1880dfe6360b4418e1414c`  
		Last Modified: Tue, 10 Oct 2023 19:48:22 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:829580fa0a5a52a282d59cef9ad292ea6a107820f172e25f062e3143bdf36e1c`  
		Last Modified: Tue, 10 Oct 2023 19:48:22 GMT  
		Size: 1.5 KB (1466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:go1.20` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:b2b4fe008079d4f71bc2b8b3512ef693dcae1bdd8e6e24425f83632e2d78093d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **320.9 MB (320912278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a492b7d2f297049e2304bdf15362502f4e27365895ff9aad1b92b7e4d852a2fe`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:20 GMT
ADD file:46dcdcde338d2c01fed5db3fac9041736d9305145d8fc2039dd5b3714d38ede8 in / 
# Wed, 20 Sep 2023 02:44:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:24:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:25:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 22:20:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 22:20:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:40:40 GMT
ENV GOLANG_VERSION=1.20.10
# Tue, 10 Oct 2023 19:40:48 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.10.linux-amd64.tar.gz'; 			sha256='80d34f1fd74e382d86c2d6102e0e60d4318461a7c2f457ec1efc4042752d4248'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.10.linux-armv6l.tar.gz'; 			sha256='a2229772434dee3dde1e974ef5ae7936160a05a1b82c57cc5c64660479aa98cb'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.10.linux-arm64.tar.gz'; 			sha256='fb3c7e15fc4413c5b81eb9f26dbd7cd4faedd5c720b30fa8e2ff77457f74cab6'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.10.linux-386.tar.gz'; 			sha256='3c918225d22ef5731b63f0426e48614fc05d8da120fc23101639c81ab152e133'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.10.linux-ppc64le.tar.gz'; 			sha256='ebac6e713810174f9ffd7f48c17c373fbf359d50d8e6233b1dfbbdebd524fd1c'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.10.linux-s390x.tar.gz'; 			sha256='fa32588cbdd1e8adfd7e9f1b4ba3f7a8b424f60e90bf2cc4716650374eb459ae'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.10.src.tar.gz'; 		sha256='72d2f51805c47150066c103754c75fddb2c19d48c9219fa33d1e46696c841dbb'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 10 Oct 2023 19:40:50 GMT
ENV GOPATH=/go
# Tue, 10 Oct 2023 19:40:50 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:40:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 10 Oct 2023 19:40:50 GMT
WORKDIR /go
# Tue, 10 Oct 2023 20:03:23 GMT
LABEL org.opencontainers.image.title=Unit (go1.20)
# Tue, 10 Oct 2023 20:03:23 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Tue, 10 Oct 2023 20:03:23 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Tue, 10 Oct 2023 20:03:23 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Tue, 10 Oct 2023 20:03:23 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Tue, 10 Oct 2023 20:03:23 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 10 Oct 2023 20:03:23 GMT
LABEL org.opencontainers.image.version=1.31.0
# Tue, 10 Oct 2023 20:04:09 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure go --go-path=$GOPATH     && make -j $NCPU go-install-src libunit-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure go --go-path=$GOPATH     && make -j $NCPU go-install-src libunit-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Tue, 10 Oct 2023 20:04:09 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Tue, 10 Oct 2023 20:04:09 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Tue, 10 Oct 2023 20:04:10 GMT
STOPSIGNAL SIGTERM
# Tue, 10 Oct 2023 20:04:10 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 10 Oct 2023 20:04:10 GMT
EXPOSE 80
# Tue, 10 Oct 2023 20:04:10 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:31f5dc1f52c865588c43d8ec718f14d430e149b28f0b28232da825da7ae28f76`  
		Last Modified: Wed, 20 Sep 2023 02:47:53 GMT  
		Size: 53.7 MB (53704892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb60045eb75c62e890b95d28e4893132a6c7d61ec9979104ee4ff6e86c4badee`  
		Last Modified: Wed, 20 Sep 2023 09:33:11 GMT  
		Size: 15.7 MB (15746671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292737ab468ef80c6f78bdde4896157b8953d1e5556e1e526f40aeadcb547573`  
		Last Modified: Wed, 20 Sep 2023 09:33:26 GMT  
		Size: 54.7 MB (54676309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486d7167072fd25b2d2370fbba8326b8059274be0fa615a14d3e975fe46f1b4f`  
		Last Modified: Wed, 20 Sep 2023 22:21:57 GMT  
		Size: 81.5 MB (81468116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3620a3068a7e100c04f3a92008ab8fb7b5657d5a6df928e4df656cd7dc0c68`  
		Last Modified: Tue, 10 Oct 2023 19:46:15 GMT  
		Size: 95.7 MB (95742099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9fd2acf33b2386df69b659928d770708cc4733475aeb32c8e4f7401ece635f`  
		Last Modified: Tue, 10 Oct 2023 19:46:06 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327f70c6c88438458daaa74f214545f1fd4c8444e75c852f0251f82ecd3c534f`  
		Last Modified: Tue, 10 Oct 2023 20:05:17 GMT  
		Size: 19.6 MB (19571295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abadc26450eb0c18e9a42145d965b482edc4c4f1e24326ca00b8d51123457fae`  
		Last Modified: Tue, 10 Oct 2023 20:05:15 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdd7b8611cb2380a77472b6ca3da0f6e4893829857f497f8d58313fded8fbdbd`  
		Last Modified: Tue, 10 Oct 2023 20:05:15 GMT  
		Size: 1.5 KB (1468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `unit:go1.21`

```console
$ docker pull unit@sha256:b9c9ddcce8c48adfce8f29648cdc7739cc01f07d86354fd751cb8728bc521186
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:go1.21` - linux; amd64

```console
$ docker pull unit@sha256:e25c525607700cb9afff5bf7ba2516c4af8a99eb8c374d614b52840ab4d2012a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.8 MB (299846746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0fba295b6f441f9cc6a84818fd1d58b0c3a5345fc0684fd72ab87fac731bc9f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 04:55:51 GMT
ADD file:85db4f4c5016f51f7112a5d09cb7d4620f565a1379ae4b8a03c5ffc23886a876 in / 
# Wed, 20 Sep 2023 04:55:51 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:22:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:22:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 03:29:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 03:29:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:19:57 GMT
ENV GOLANG_VERSION=1.21.3
# Tue, 10 Oct 2023 19:20:06 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.3.linux-mips64le.tar.gz'; 			sha256='a569ffbc88b4e14cf2682f65cec950460665e4392b0d78b8868b4718c979bda8'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 10 Oct 2023 19:20:07 GMT
ENV GOTOOLCHAIN=local
# Tue, 10 Oct 2023 19:20:07 GMT
ENV GOPATH=/go
# Tue, 10 Oct 2023 19:20:07 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:20:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 10 Oct 2023 19:20:07 GMT
WORKDIR /go
# Tue, 10 Oct 2023 19:45:00 GMT
LABEL org.opencontainers.image.title=Unit (go1.21)
# Tue, 10 Oct 2023 19:45:00 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Tue, 10 Oct 2023 19:45:00 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Tue, 10 Oct 2023 19:45:00 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Tue, 10 Oct 2023 19:45:00 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Tue, 10 Oct 2023 19:45:00 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 10 Oct 2023 19:45:00 GMT
LABEL org.opencontainers.image.version=1.31.0
# Tue, 10 Oct 2023 19:45:58 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure go --go-path=$GOPATH     && make -j $NCPU go-install-src libunit-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure go --go-path=$GOPATH     && make -j $NCPU go-install-src libunit-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Tue, 10 Oct 2023 19:45:59 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Tue, 10 Oct 2023 19:45:59 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Tue, 10 Oct 2023 19:45:59 GMT
STOPSIGNAL SIGTERM
# Tue, 10 Oct 2023 19:45:59 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 10 Oct 2023 19:45:59 GMT
EXPOSE 80
# Tue, 10 Oct 2023 19:45:59 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:ddf874abf16cc990e0fd75a154a34ca0a03ee310ad895a18fb62ae15bf4171fb`  
		Last Modified: Wed, 20 Sep 2023 05:00:41 GMT  
		Size: 55.1 MB (55056714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1459d3ab8b5e46ac1a0a00134fe2f7b693474eb6d75ace97ecbe811a6f5b0e`  
		Last Modified: Wed, 20 Sep 2023 09:31:06 GMT  
		Size: 15.8 MB (15760408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab00e7798a04602c3f6e2dc445a994d75e96c45533cd44701f58509982a8c5`  
		Last Modified: Wed, 20 Sep 2023 09:31:23 GMT  
		Size: 54.6 MB (54584790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9036a471a1c45233bf72245ae53bd00fd2b25cbdf75be2cafe1c6fd91309cdb7`  
		Last Modified: Thu, 21 Sep 2023 03:31:14 GMT  
		Size: 86.1 MB (86068436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a30056caa3534c4f704e37958c32100b96aa5535fff9af405b5bf4cd272e158`  
		Last Modified: Tue, 10 Oct 2023 19:25:53 GMT  
		Size: 67.0 MB (67001246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca402200ac32a0f6d38fdcae01d58d804e90543fabef314c0aaa4731ac3f9b6`  
		Last Modified: Tue, 10 Oct 2023 19:25:42 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62756cd2c6f084fd53a983f51ef7d6c5b3d9ef2f80d2fc122550940332ad324`  
		Last Modified: Tue, 10 Oct 2023 19:48:08 GMT  
		Size: 21.4 MB (21372254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13a00f1dc20f8f2006ac8c9b1c91c322d352fd41f2b3a41e00fb8bba12e3534`  
		Last Modified: Tue, 10 Oct 2023 19:48:05 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533fb155fbc122a1435f260e62b8f43d7de9a2c0675df5ecf4b5bc1a6f4d93ed`  
		Last Modified: Tue, 10 Oct 2023 19:48:05 GMT  
		Size: 1.5 KB (1470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:go1.21` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:8a3b8f2b9a104a7bab667ab4a73ad407817aab9ec14cb264a3e2df2814cf8b6a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289268520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9020087609178de15b4aea74b2bfc5530c392b2d08c4661713cdad84547c7415`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:20 GMT
ADD file:46dcdcde338d2c01fed5db3fac9041736d9305145d8fc2039dd5b3714d38ede8 in / 
# Wed, 20 Sep 2023 02:44:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:24:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:25:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 22:20:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 22:20:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:39:44 GMT
ENV GOLANG_VERSION=1.21.3
# Tue, 10 Oct 2023 19:39:52 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.3.linux-mips64le.tar.gz'; 			sha256='a569ffbc88b4e14cf2682f65cec950460665e4392b0d78b8868b4718c979bda8'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 10 Oct 2023 19:39:53 GMT
ENV GOTOOLCHAIN=local
# Tue, 10 Oct 2023 19:39:54 GMT
ENV GOPATH=/go
# Tue, 10 Oct 2023 19:39:54 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:39:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 10 Oct 2023 19:39:54 GMT
WORKDIR /go
# Tue, 10 Oct 2023 20:02:25 GMT
LABEL org.opencontainers.image.title=Unit (go1.21)
# Tue, 10 Oct 2023 20:02:25 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Tue, 10 Oct 2023 20:02:25 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Tue, 10 Oct 2023 20:02:25 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Tue, 10 Oct 2023 20:02:26 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Tue, 10 Oct 2023 20:02:26 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 10 Oct 2023 20:02:26 GMT
LABEL org.opencontainers.image.version=1.31.0
# Tue, 10 Oct 2023 20:03:13 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure go --go-path=$GOPATH     && make -j $NCPU go-install-src libunit-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure go --go-path=$GOPATH     && make -j $NCPU go-install-src libunit-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Tue, 10 Oct 2023 20:03:13 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Tue, 10 Oct 2023 20:03:13 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Tue, 10 Oct 2023 20:03:13 GMT
STOPSIGNAL SIGTERM
# Tue, 10 Oct 2023 20:03:13 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 10 Oct 2023 20:03:13 GMT
EXPOSE 80
# Tue, 10 Oct 2023 20:03:14 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:31f5dc1f52c865588c43d8ec718f14d430e149b28f0b28232da825da7ae28f76`  
		Last Modified: Wed, 20 Sep 2023 02:47:53 GMT  
		Size: 53.7 MB (53704892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb60045eb75c62e890b95d28e4893132a6c7d61ec9979104ee4ff6e86c4badee`  
		Last Modified: Wed, 20 Sep 2023 09:33:11 GMT  
		Size: 15.7 MB (15746671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292737ab468ef80c6f78bdde4896157b8953d1e5556e1e526f40aeadcb547573`  
		Last Modified: Wed, 20 Sep 2023 09:33:26 GMT  
		Size: 54.7 MB (54676309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486d7167072fd25b2d2370fbba8326b8059274be0fa615a14d3e975fe46f1b4f`  
		Last Modified: Wed, 20 Sep 2023 22:21:57 GMT  
		Size: 81.5 MB (81468116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1306584d039cecaec0b207b88108f8c03ec361f1cf8015ae4ba23ec3c9406f50`  
		Last Modified: Tue, 10 Oct 2023 19:44:41 GMT  
		Size: 64.1 MB (64098318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815863143577abf9b2b650b8a28f205bfc32287c17ee2b8c0e8a8155b2a75ca3`  
		Last Modified: Tue, 10 Oct 2023 19:44:28 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd1b8471a82b8fb80921156f2b1abe4b85e1db1756650baa8a63c94cdb72a9ac`  
		Last Modified: Tue, 10 Oct 2023 20:05:01 GMT  
		Size: 19.6 MB (19571320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e45a03b84b12daccf9bbc14746f689f1d235d2526a77c4fa8e26e9e97ca6ff0`  
		Last Modified: Tue, 10 Oct 2023 20:04:58 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc16a37f4406cdb2846b682b8e11e00ea46efd01c2826567faa97e87146f0f20`  
		Last Modified: Tue, 10 Oct 2023 20:04:58 GMT  
		Size: 1.5 KB (1467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `unit:jsc`

```console
$ docker pull unit@sha256:e50d9d241fa875598b3297e8ec201d7dff76133c2175e38a250e5784be524c1b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:jsc` - linux; amd64

```console
$ docker pull unit@sha256:6016dbebad214783b916db5de81e16e7d24981a202b3259f0597a06e447d8f56
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.6 MB (202620873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:381ecba965946dd28e8467f802d866b567b6ac1f78b91a8a7cdafc202dd5c9a1`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Mon, 25 Sep 2023 10:17:05 GMT
ARG RELEASE
# Mon, 25 Sep 2023 10:17:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 25 Sep 2023 10:17:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 25 Sep 2023 10:17:05 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 25 Sep 2023 10:17:07 GMT
ADD file:194c886b88876c1804cc5f80719669653c16a388b664147b7f22402105f533c4 in / 
# Mon, 25 Sep 2023 10:17:08 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 05:11:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 03 Oct 2023 05:11:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 05:11:45 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 03 Oct 2023 05:12:00 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 05:12:35 GMT
ENV JAVA_VERSION=jdk-11.0.20.1+1
# Tue, 03 Oct 2023 05:12:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69d39682c4a2fac294a9eaacbf62c26d3c8a2f9123f1b5d287498a5472c6b672';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        armhf|arm)          ESUM='e83674aee238ebb5f359b9395b3c5e3fad5b645846095494662802d2f0fd01c9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_arm_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='b806f4bb526161bf9b2ffb37be4e1b77f56b4e726dc4d52c7902130a79e7d710';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='a7efbe804a4616d38b6ac0def40cd9feacc04aee2bb89132191f4d33fc0a7c1e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='398a64bff002f0e3b0c01ecd24a1a32c83cb72a5255344219e9757d4ddd9f857';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_x64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 03 Oct 2023 05:12:46 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 03 Oct 2023 05:12:46 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Tue, 03 Oct 2023 05:12:46 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Tue, 03 Oct 2023 05:12:46 GMT
CMD ["jshell"]
# Tue, 03 Oct 2023 09:52:09 GMT
LABEL org.opencontainers.image.title=Unit (jsc11)
# Tue, 03 Oct 2023 09:52:09 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Tue, 03 Oct 2023 09:52:09 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Tue, 03 Oct 2023 09:52:10 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Tue, 03 Oct 2023 09:52:10 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Tue, 03 Oct 2023 09:52:10 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 03 Oct 2023 09:52:10 GMT
LABEL org.opencontainers.image.version=1.31.0
# Tue, 03 Oct 2023 09:54:28 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure java --jars=/usr/share/unit-jsc-common/     && make -j $NCPU java-shared-install java-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure java --jars=/usr/share/unit-jsc-common/     && make -j $NCPU java-shared-install java-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && rm -rf /root/.m2     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Tue, 03 Oct 2023 09:54:28 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Tue, 03 Oct 2023 09:54:28 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Tue, 03 Oct 2023 09:54:28 GMT
STOPSIGNAL SIGTERM
# Tue, 03 Oct 2023 09:54:28 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 03 Oct 2023 09:54:28 GMT
EXPOSE 80
# Tue, 03 Oct 2023 09:54:28 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:707e32e9fc569fee476af9e92ae3d1df8b8e6dca47f9cb31db9d2c922a6de952`  
		Last Modified: Mon, 25 Sep 2023 12:54:05 GMT  
		Size: 30.4 MB (30440869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320d7b4a8f0a0932d6c981aa21a5793fb50fc408278be946023a29cdbe81594b`  
		Last Modified: Tue, 03 Oct 2023 05:16:04 GMT  
		Size: 12.9 MB (12902712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1198a528604fdd5b16e909383ab8d985b7cbc003c05ba6d441388bae6d5c79ea`  
		Last Modified: Tue, 03 Oct 2023 05:16:58 GMT  
		Size: 144.8 MB (144836065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5d4fd9d99dab5a8bf810d560d314fd9b72f50c074b510bc3699f524f1cd9b2`  
		Last Modified: Tue, 03 Oct 2023 05:16:47 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50cc5b9dc759b6d18830d982e59eb599ec2af11c6fdd227f0bbbe3954b2357be`  
		Last Modified: Tue, 03 Oct 2023 05:16:47 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b5ff4a0275694dfa99bab3a081be450836129cd75e6637e0722a6f476a10aed`  
		Last Modified: Tue, 03 Oct 2023 09:55:15 GMT  
		Size: 14.4 MB (14437584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8073bea624df40f4799f22f93c9a7f1be90fba7f0cd4c457d49db820287f75f`  
		Last Modified: Tue, 03 Oct 2023 09:55:13 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72af9c810665ef90c9790f16cabe13c6b839bc15a10a80fb75403e5dda76934e`  
		Last Modified: Tue, 03 Oct 2023 09:55:13 GMT  
		Size: 1.5 KB (1468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:jsc` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:ead51b31b9489fef27235b9da252b28ac0ff5f0e2502d384e4b698cb94b2edb1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.2 MB (197194795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ec37f60f6e40f250b3b060a062b9adb7f5522757c2d35b5e71a6b813761c883`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Mon, 25 Sep 2023 10:17:41 GMT
ARG RELEASE
# Mon, 25 Sep 2023 10:17:41 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 25 Sep 2023 10:17:41 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 25 Sep 2023 10:17:41 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 25 Sep 2023 10:17:44 GMT
ADD file:8540670760767f19eaf101fbce1da1881a2f24a7d65da6abdedc644b8fb00463 in / 
# Mon, 25 Sep 2023 10:17:45 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 06:06:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 03 Oct 2023 06:06:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 06:06:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 03 Oct 2023 06:07:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 06:07:36 GMT
ENV JAVA_VERSION=jdk-11.0.20.1+1
# Tue, 03 Oct 2023 06:07:45 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69d39682c4a2fac294a9eaacbf62c26d3c8a2f9123f1b5d287498a5472c6b672';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        armhf|arm)          ESUM='e83674aee238ebb5f359b9395b3c5e3fad5b645846095494662802d2f0fd01c9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_arm_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='b806f4bb526161bf9b2ffb37be4e1b77f56b4e726dc4d52c7902130a79e7d710';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='a7efbe804a4616d38b6ac0def40cd9feacc04aee2bb89132191f4d33fc0a7c1e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='398a64bff002f0e3b0c01ecd24a1a32c83cb72a5255344219e9757d4ddd9f857';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_x64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 03 Oct 2023 06:07:48 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 03 Oct 2023 06:07:48 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Tue, 03 Oct 2023 06:07:48 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Tue, 03 Oct 2023 06:07:48 GMT
CMD ["jshell"]
# Tue, 03 Oct 2023 07:15:07 GMT
LABEL org.opencontainers.image.title=Unit (jsc11)
# Tue, 03 Oct 2023 07:15:07 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Tue, 03 Oct 2023 07:15:07 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Tue, 03 Oct 2023 07:15:07 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Tue, 03 Oct 2023 07:15:07 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Tue, 03 Oct 2023 07:15:07 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 03 Oct 2023 07:15:07 GMT
LABEL org.opencontainers.image.version=1.31.0
# Tue, 03 Oct 2023 07:16:47 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure java --jars=/usr/share/unit-jsc-common/     && make -j $NCPU java-shared-install java-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure java --jars=/usr/share/unit-jsc-common/     && make -j $NCPU java-shared-install java-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && rm -rf /root/.m2     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Tue, 03 Oct 2023 07:16:47 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Tue, 03 Oct 2023 07:16:47 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Tue, 03 Oct 2023 07:16:47 GMT
STOPSIGNAL SIGTERM
# Tue, 03 Oct 2023 07:16:47 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 03 Oct 2023 07:16:47 GMT
EXPOSE 80
# Tue, 03 Oct 2023 07:16:47 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:6ea603f1df5e3d23206761eca19fba4cdf4e22d773256cb65b71b730aa5acced`  
		Last Modified: Mon, 25 Sep 2023 17:30:11 GMT  
		Size: 28.4 MB (28392073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db904450c39fc4ef39317a37a19b15df4a74bf6bb91100343e382470ce034d79`  
		Last Modified: Tue, 03 Oct 2023 06:10:10 GMT  
		Size: 12.8 MB (12843603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b47fc5d37efc4608b1cbe274678274c4b0b13ffba61a009da323e825c70dcd`  
		Last Modified: Tue, 03 Oct 2023 06:10:57 GMT  
		Size: 141.6 MB (141581350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de85af6ca814ebce4fe8e3c07e7d5e2099f636f57368a04174aa5b8b2f8bffb`  
		Last Modified: Tue, 03 Oct 2023 06:10:48 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c1a07105f3af8e80487db46085c03e9df93026a8e7f4c8a26654db2826a9d5e`  
		Last Modified: Tue, 03 Oct 2023 06:10:48 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2a175557d394fae17c79474734d29b5e49ff13dba8d6193c6bbb7d3779c82d`  
		Last Modified: Tue, 03 Oct 2023 07:17:38 GMT  
		Size: 14.4 MB (14374133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1960ccd711ddb8654be789e03ca9b87caa16611dafc565defef9b699e7758d`  
		Last Modified: Tue, 03 Oct 2023 07:17:36 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4bf78594cdc3a2cee6b96864eba53b2636f69f3354357a986b1fb1ff48fb75b`  
		Last Modified: Tue, 03 Oct 2023 07:17:36 GMT  
		Size: 1.5 KB (1466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `unit:jsc11`

```console
$ docker pull unit@sha256:e50d9d241fa875598b3297e8ec201d7dff76133c2175e38a250e5784be524c1b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:jsc11` - linux; amd64

```console
$ docker pull unit@sha256:6016dbebad214783b916db5de81e16e7d24981a202b3259f0597a06e447d8f56
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.6 MB (202620873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:381ecba965946dd28e8467f802d866b567b6ac1f78b91a8a7cdafc202dd5c9a1`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Mon, 25 Sep 2023 10:17:05 GMT
ARG RELEASE
# Mon, 25 Sep 2023 10:17:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 25 Sep 2023 10:17:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 25 Sep 2023 10:17:05 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 25 Sep 2023 10:17:07 GMT
ADD file:194c886b88876c1804cc5f80719669653c16a388b664147b7f22402105f533c4 in / 
# Mon, 25 Sep 2023 10:17:08 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 05:11:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 03 Oct 2023 05:11:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 05:11:45 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 03 Oct 2023 05:12:00 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 05:12:35 GMT
ENV JAVA_VERSION=jdk-11.0.20.1+1
# Tue, 03 Oct 2023 05:12:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69d39682c4a2fac294a9eaacbf62c26d3c8a2f9123f1b5d287498a5472c6b672';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        armhf|arm)          ESUM='e83674aee238ebb5f359b9395b3c5e3fad5b645846095494662802d2f0fd01c9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_arm_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='b806f4bb526161bf9b2ffb37be4e1b77f56b4e726dc4d52c7902130a79e7d710';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='a7efbe804a4616d38b6ac0def40cd9feacc04aee2bb89132191f4d33fc0a7c1e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='398a64bff002f0e3b0c01ecd24a1a32c83cb72a5255344219e9757d4ddd9f857';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_x64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 03 Oct 2023 05:12:46 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 03 Oct 2023 05:12:46 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Tue, 03 Oct 2023 05:12:46 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Tue, 03 Oct 2023 05:12:46 GMT
CMD ["jshell"]
# Tue, 03 Oct 2023 09:52:09 GMT
LABEL org.opencontainers.image.title=Unit (jsc11)
# Tue, 03 Oct 2023 09:52:09 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Tue, 03 Oct 2023 09:52:09 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Tue, 03 Oct 2023 09:52:10 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Tue, 03 Oct 2023 09:52:10 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Tue, 03 Oct 2023 09:52:10 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 03 Oct 2023 09:52:10 GMT
LABEL org.opencontainers.image.version=1.31.0
# Tue, 03 Oct 2023 09:54:28 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure java --jars=/usr/share/unit-jsc-common/     && make -j $NCPU java-shared-install java-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure java --jars=/usr/share/unit-jsc-common/     && make -j $NCPU java-shared-install java-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && rm -rf /root/.m2     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Tue, 03 Oct 2023 09:54:28 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Tue, 03 Oct 2023 09:54:28 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Tue, 03 Oct 2023 09:54:28 GMT
STOPSIGNAL SIGTERM
# Tue, 03 Oct 2023 09:54:28 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 03 Oct 2023 09:54:28 GMT
EXPOSE 80
# Tue, 03 Oct 2023 09:54:28 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:707e32e9fc569fee476af9e92ae3d1df8b8e6dca47f9cb31db9d2c922a6de952`  
		Last Modified: Mon, 25 Sep 2023 12:54:05 GMT  
		Size: 30.4 MB (30440869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320d7b4a8f0a0932d6c981aa21a5793fb50fc408278be946023a29cdbe81594b`  
		Last Modified: Tue, 03 Oct 2023 05:16:04 GMT  
		Size: 12.9 MB (12902712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1198a528604fdd5b16e909383ab8d985b7cbc003c05ba6d441388bae6d5c79ea`  
		Last Modified: Tue, 03 Oct 2023 05:16:58 GMT  
		Size: 144.8 MB (144836065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5d4fd9d99dab5a8bf810d560d314fd9b72f50c074b510bc3699f524f1cd9b2`  
		Last Modified: Tue, 03 Oct 2023 05:16:47 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50cc5b9dc759b6d18830d982e59eb599ec2af11c6fdd227f0bbbe3954b2357be`  
		Last Modified: Tue, 03 Oct 2023 05:16:47 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b5ff4a0275694dfa99bab3a081be450836129cd75e6637e0722a6f476a10aed`  
		Last Modified: Tue, 03 Oct 2023 09:55:15 GMT  
		Size: 14.4 MB (14437584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8073bea624df40f4799f22f93c9a7f1be90fba7f0cd4c457d49db820287f75f`  
		Last Modified: Tue, 03 Oct 2023 09:55:13 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72af9c810665ef90c9790f16cabe13c6b839bc15a10a80fb75403e5dda76934e`  
		Last Modified: Tue, 03 Oct 2023 09:55:13 GMT  
		Size: 1.5 KB (1468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:jsc11` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:ead51b31b9489fef27235b9da252b28ac0ff5f0e2502d384e4b698cb94b2edb1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.2 MB (197194795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ec37f60f6e40f250b3b060a062b9adb7f5522757c2d35b5e71a6b813761c883`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Mon, 25 Sep 2023 10:17:41 GMT
ARG RELEASE
# Mon, 25 Sep 2023 10:17:41 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 25 Sep 2023 10:17:41 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 25 Sep 2023 10:17:41 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 25 Sep 2023 10:17:44 GMT
ADD file:8540670760767f19eaf101fbce1da1881a2f24a7d65da6abdedc644b8fb00463 in / 
# Mon, 25 Sep 2023 10:17:45 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 06:06:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 03 Oct 2023 06:06:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 06:06:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 03 Oct 2023 06:07:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 06:07:36 GMT
ENV JAVA_VERSION=jdk-11.0.20.1+1
# Tue, 03 Oct 2023 06:07:45 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69d39682c4a2fac294a9eaacbf62c26d3c8a2f9123f1b5d287498a5472c6b672';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        armhf|arm)          ESUM='e83674aee238ebb5f359b9395b3c5e3fad5b645846095494662802d2f0fd01c9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_arm_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='b806f4bb526161bf9b2ffb37be4e1b77f56b4e726dc4d52c7902130a79e7d710';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='a7efbe804a4616d38b6ac0def40cd9feacc04aee2bb89132191f4d33fc0a7c1e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='398a64bff002f0e3b0c01ecd24a1a32c83cb72a5255344219e9757d4ddd9f857';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_x64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 03 Oct 2023 06:07:48 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 03 Oct 2023 06:07:48 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Tue, 03 Oct 2023 06:07:48 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Tue, 03 Oct 2023 06:07:48 GMT
CMD ["jshell"]
# Tue, 03 Oct 2023 07:15:07 GMT
LABEL org.opencontainers.image.title=Unit (jsc11)
# Tue, 03 Oct 2023 07:15:07 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Tue, 03 Oct 2023 07:15:07 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Tue, 03 Oct 2023 07:15:07 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Tue, 03 Oct 2023 07:15:07 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Tue, 03 Oct 2023 07:15:07 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 03 Oct 2023 07:15:07 GMT
LABEL org.opencontainers.image.version=1.31.0
# Tue, 03 Oct 2023 07:16:47 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure java --jars=/usr/share/unit-jsc-common/     && make -j $NCPU java-shared-install java-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure java --jars=/usr/share/unit-jsc-common/     && make -j $NCPU java-shared-install java-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && rm -rf /root/.m2     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Tue, 03 Oct 2023 07:16:47 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Tue, 03 Oct 2023 07:16:47 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Tue, 03 Oct 2023 07:16:47 GMT
STOPSIGNAL SIGTERM
# Tue, 03 Oct 2023 07:16:47 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 03 Oct 2023 07:16:47 GMT
EXPOSE 80
# Tue, 03 Oct 2023 07:16:47 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:6ea603f1df5e3d23206761eca19fba4cdf4e22d773256cb65b71b730aa5acced`  
		Last Modified: Mon, 25 Sep 2023 17:30:11 GMT  
		Size: 28.4 MB (28392073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db904450c39fc4ef39317a37a19b15df4a74bf6bb91100343e382470ce034d79`  
		Last Modified: Tue, 03 Oct 2023 06:10:10 GMT  
		Size: 12.8 MB (12843603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b47fc5d37efc4608b1cbe274678274c4b0b13ffba61a009da323e825c70dcd`  
		Last Modified: Tue, 03 Oct 2023 06:10:57 GMT  
		Size: 141.6 MB (141581350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de85af6ca814ebce4fe8e3c07e7d5e2099f636f57368a04174aa5b8b2f8bffb`  
		Last Modified: Tue, 03 Oct 2023 06:10:48 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c1a07105f3af8e80487db46085c03e9df93026a8e7f4c8a26654db2826a9d5e`  
		Last Modified: Tue, 03 Oct 2023 06:10:48 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2a175557d394fae17c79474734d29b5e49ff13dba8d6193c6bbb7d3779c82d`  
		Last Modified: Tue, 03 Oct 2023 07:17:38 GMT  
		Size: 14.4 MB (14374133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1960ccd711ddb8654be789e03ca9b87caa16611dafc565defef9b699e7758d`  
		Last Modified: Tue, 03 Oct 2023 07:17:36 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4bf78594cdc3a2cee6b96864eba53b2636f69f3354357a986b1fb1ff48fb75b`  
		Last Modified: Tue, 03 Oct 2023 07:17:36 GMT  
		Size: 1.5 KB (1466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `unit:latest`

```console
$ docker pull unit@sha256:d3557fce352d557ecaa5fb542a4330875b55800b84f9999643b11f00ce7dec90
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:latest` - linux; amd64

```console
$ docker pull unit@sha256:8a058f2ff2357725a0e2d43771b4b90127c7c34e70f8d4f4d82a7e4b4ab8eb56
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40261522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9594c8601a63442da9eafb2f3e26140881d6aaddcda8909fc46b77c5085f2805`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:56:57 GMT
LABEL org.opencontainers.image.title=Unit (minimal)
# Wed, 11 Oct 2023 19:56:57 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Wed, 11 Oct 2023 19:56:57 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Wed, 11 Oct 2023 19:56:58 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Wed, 11 Oct 2023 19:56:58 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Wed, 11 Oct 2023 19:56:58 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 11 Oct 2023 19:56:58 GMT
LABEL org.opencontainers.image.version=1.31.0
# Wed, 11 Oct 2023 19:58:10 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure      && make -j $NCPU version     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure      && make -j $NCPU version     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Wed, 11 Oct 2023 19:58:10 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Wed, 11 Oct 2023 19:58:10 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Wed, 11 Oct 2023 19:58:10 GMT
STOPSIGNAL SIGTERM
# Wed, 11 Oct 2023 19:58:10 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Wed, 11 Oct 2023 19:58:10 GMT
EXPOSE 80
# Wed, 11 Oct 2023 19:58:10 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5c7861ad106bab941590b1d57e5271280238a482a62fae3a844f35758d6cf7`  
		Last Modified: Wed, 11 Oct 2023 19:59:14 GMT  
		Size: 8.8 MB (8840929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab66ee2cb20cc896b833b4cac356f5b8e28033978c6cb561db3684ff1682aeab`  
		Last Modified: Wed, 11 Oct 2023 19:59:12 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d2941a2f57e962e97d0feb6ed0ba2e47520d777a33cddab81bdb2e23380087`  
		Last Modified: Wed, 11 Oct 2023 19:59:12 GMT  
		Size: 1.5 KB (1466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:latest` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:ccb78488948a120aa107a189c9ec3141b59dbe074b90d58fff0722300f58d688
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38766827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5cfb5b45514db84628b66c8c7d11190d1b56b910be1b5ac53b473d3b093b1a0`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:06 GMT
ADD file:2c3e5451390c62f0b85f20139d2c88011cc54d649cdda5567084c050ad373372 in / 
# Wed, 11 Oct 2023 18:25:06 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:12:20 GMT
LABEL org.opencontainers.image.title=Unit (minimal)
# Wed, 11 Oct 2023 19:12:20 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Wed, 11 Oct 2023 19:12:20 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Wed, 11 Oct 2023 19:12:20 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Wed, 11 Oct 2023 19:12:20 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Wed, 11 Oct 2023 19:12:20 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 11 Oct 2023 19:12:20 GMT
LABEL org.opencontainers.image.version=1.31.0
# Wed, 11 Oct 2023 19:13:19 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure      && make -j $NCPU version     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure      && make -j $NCPU version     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Wed, 11 Oct 2023 19:13:19 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Wed, 11 Oct 2023 19:13:19 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Wed, 11 Oct 2023 19:13:19 GMT
STOPSIGNAL SIGTERM
# Wed, 11 Oct 2023 19:13:19 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Wed, 11 Oct 2023 19:13:19 GMT
EXPOSE 80
# Wed, 11 Oct 2023 19:13:19 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:85e50d2242ceaba78c3726e059dbd2fa06f5c18e265554bd43a482d19b256d20`  
		Last Modified: Wed, 11 Oct 2023 18:29:07 GMT  
		Size: 30.1 MB (30064086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd2be98a787512e0f31ff5098e023ab6f7741e004bd83a019f3338a55b88442`  
		Last Modified: Wed, 11 Oct 2023 19:14:15 GMT  
		Size: 8.7 MB (8700007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e73e3e6505fafe6a4bb27553af1b9d11b649958d6b791bf4262e079a5a2ac97`  
		Last Modified: Wed, 11 Oct 2023 19:14:14 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b9dcc88e7522a2402575f94c8416ef9bdf27633408d51eaee97dab9216e948`  
		Last Modified: Wed, 11 Oct 2023 19:14:14 GMT  
		Size: 1.5 KB (1469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `unit:minimal`

```console
$ docker pull unit@sha256:d3557fce352d557ecaa5fb542a4330875b55800b84f9999643b11f00ce7dec90
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:minimal` - linux; amd64

```console
$ docker pull unit@sha256:8a058f2ff2357725a0e2d43771b4b90127c7c34e70f8d4f4d82a7e4b4ab8eb56
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40261522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9594c8601a63442da9eafb2f3e26140881d6aaddcda8909fc46b77c5085f2805`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:56:57 GMT
LABEL org.opencontainers.image.title=Unit (minimal)
# Wed, 11 Oct 2023 19:56:57 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Wed, 11 Oct 2023 19:56:57 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Wed, 11 Oct 2023 19:56:58 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Wed, 11 Oct 2023 19:56:58 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Wed, 11 Oct 2023 19:56:58 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 11 Oct 2023 19:56:58 GMT
LABEL org.opencontainers.image.version=1.31.0
# Wed, 11 Oct 2023 19:58:10 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure      && make -j $NCPU version     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure      && make -j $NCPU version     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Wed, 11 Oct 2023 19:58:10 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Wed, 11 Oct 2023 19:58:10 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Wed, 11 Oct 2023 19:58:10 GMT
STOPSIGNAL SIGTERM
# Wed, 11 Oct 2023 19:58:10 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Wed, 11 Oct 2023 19:58:10 GMT
EXPOSE 80
# Wed, 11 Oct 2023 19:58:10 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5c7861ad106bab941590b1d57e5271280238a482a62fae3a844f35758d6cf7`  
		Last Modified: Wed, 11 Oct 2023 19:59:14 GMT  
		Size: 8.8 MB (8840929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab66ee2cb20cc896b833b4cac356f5b8e28033978c6cb561db3684ff1682aeab`  
		Last Modified: Wed, 11 Oct 2023 19:59:12 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d2941a2f57e962e97d0feb6ed0ba2e47520d777a33cddab81bdb2e23380087`  
		Last Modified: Wed, 11 Oct 2023 19:59:12 GMT  
		Size: 1.5 KB (1466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:minimal` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:ccb78488948a120aa107a189c9ec3141b59dbe074b90d58fff0722300f58d688
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38766827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5cfb5b45514db84628b66c8c7d11190d1b56b910be1b5ac53b473d3b093b1a0`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:06 GMT
ADD file:2c3e5451390c62f0b85f20139d2c88011cc54d649cdda5567084c050ad373372 in / 
# Wed, 11 Oct 2023 18:25:06 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:12:20 GMT
LABEL org.opencontainers.image.title=Unit (minimal)
# Wed, 11 Oct 2023 19:12:20 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Wed, 11 Oct 2023 19:12:20 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Wed, 11 Oct 2023 19:12:20 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Wed, 11 Oct 2023 19:12:20 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Wed, 11 Oct 2023 19:12:20 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 11 Oct 2023 19:12:20 GMT
LABEL org.opencontainers.image.version=1.31.0
# Wed, 11 Oct 2023 19:13:19 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure      && make -j $NCPU version     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure      && make -j $NCPU version     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Wed, 11 Oct 2023 19:13:19 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Wed, 11 Oct 2023 19:13:19 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Wed, 11 Oct 2023 19:13:19 GMT
STOPSIGNAL SIGTERM
# Wed, 11 Oct 2023 19:13:19 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Wed, 11 Oct 2023 19:13:19 GMT
EXPOSE 80
# Wed, 11 Oct 2023 19:13:19 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:85e50d2242ceaba78c3726e059dbd2fa06f5c18e265554bd43a482d19b256d20`  
		Last Modified: Wed, 11 Oct 2023 18:29:07 GMT  
		Size: 30.1 MB (30064086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd2be98a787512e0f31ff5098e023ab6f7741e004bd83a019f3338a55b88442`  
		Last Modified: Wed, 11 Oct 2023 19:14:15 GMT  
		Size: 8.7 MB (8700007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e73e3e6505fafe6a4bb27553af1b9d11b649958d6b791bf4262e079a5a2ac97`  
		Last Modified: Wed, 11 Oct 2023 19:14:14 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b9dcc88e7522a2402575f94c8416ef9bdf27633408d51eaee97dab9216e948`  
		Last Modified: Wed, 11 Oct 2023 19:14:14 GMT  
		Size: 1.5 KB (1469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `unit:node`

```console
$ docker pull unit@sha256:2e5fdd933383b2f8b36ddd1ff597467b8f7fb6082b30afcca4c574a3c79f24aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:node` - linux; amd64

```console
$ docker pull unit@sha256:9a17e1115cff9de798eee7bb865e2e74f001de34c20b6fc2b44c868f94a45d83
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **382.2 MB (382169133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ce8f24e50447c2c131f7c2f7aa0edb8605448cae812158185bf76cd3dffa3fd`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 04:55:51 GMT
ADD file:85db4f4c5016f51f7112a5d09cb7d4620f565a1379ae4b8a03c5ffc23886a876 in / 
# Wed, 20 Sep 2023 04:55:51 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:22:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:22:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:23:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 03:33:48 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Fri, 29 Sep 2023 19:24:14 GMT
ENV NODE_VERSION=20.8.0
# Fri, 29 Sep 2023 19:24:30 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     4ED778F539E3634C779C87C6D7062848A1AB005C     141F07595B7B3FFE74309A937405533BE57C7D57     74F12602B6F1C4E913FAA37AD3A89613643B6201     DD792F5973C6DE52C432CBDAC77ABFA00DDBF2B7     61FC681DFB92A079F1685E77973F295594EC4689     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4     C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     108F52B48DB57BB0CC439B2997B01419BD92F80A     A363A499291CBBC940DD62E41F10027AF002F8B0   ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Fri, 29 Sep 2023 19:24:31 GMT
ENV YARN_VERSION=1.22.19
# Fri, 29 Sep 2023 19:24:34 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Fri, 29 Sep 2023 19:24:34 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 29 Sep 2023 19:24:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Sep 2023 19:24:34 GMT
CMD ["node"]
# Fri, 29 Sep 2023 20:10:13 GMT
LABEL org.opencontainers.image.title=Unit (node20)
# Fri, 29 Sep 2023 20:10:13 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Fri, 29 Sep 2023 20:10:14 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Fri, 29 Sep 2023 20:10:14 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Fri, 29 Sep 2023 20:10:14 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Fri, 29 Sep 2023 20:10:14 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Fri, 29 Sep 2023 20:10:14 GMT
LABEL org.opencontainers.image.version=1.31.0
# Fri, 29 Sep 2023 20:11:13 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && npm -g install node-gyp     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure nodejs --node-gyp=/usr/local/bin/node-gyp     && make -j $NCPU node node-install libunit-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure nodejs --node-gyp=/usr/local/bin/node-gyp     && make -j $NCPU node node-install libunit-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && rm -rf /root/.cache/ && rm -rf /root/.npm     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Fri, 29 Sep 2023 20:11:13 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Fri, 29 Sep 2023 20:11:13 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Fri, 29 Sep 2023 20:11:13 GMT
STOPSIGNAL SIGTERM
# Fri, 29 Sep 2023 20:11:13 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Fri, 29 Sep 2023 20:11:14 GMT
EXPOSE 80
# Fri, 29 Sep 2023 20:11:14 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:ddf874abf16cc990e0fd75a154a34ca0a03ee310ad895a18fb62ae15bf4171fb`  
		Last Modified: Wed, 20 Sep 2023 05:00:41 GMT  
		Size: 55.1 MB (55056714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1459d3ab8b5e46ac1a0a00134fe2f7b693474eb6d75ace97ecbe811a6f5b0e`  
		Last Modified: Wed, 20 Sep 2023 09:31:06 GMT  
		Size: 15.8 MB (15760408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab00e7798a04602c3f6e2dc445a994d75e96c45533cd44701f58509982a8c5`  
		Last Modified: Wed, 20 Sep 2023 09:31:23 GMT  
		Size: 54.6 MB (54584790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7883a473306cf6632abe7e913e0f1a21ac2fed038a4116473b25738b8b88b294`  
		Last Modified: Wed, 20 Sep 2023 09:31:55 GMT  
		Size: 196.8 MB (196842512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ea6a75eb435af25ba0b42343548bee2f6eb322326d98e39823aa45c2ff2b21`  
		Last Modified: Thu, 21 Sep 2023 03:37:33 GMT  
		Size: 4.2 KB (4201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4adcb3caaf61e057ad5e1d45646af5af38d7ed33278d2648d3673a3813a5ad0`  
		Last Modified: Fri, 29 Sep 2023 19:29:53 GMT  
		Size: 47.9 MB (47890750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074c9dbbb6a5fe5d4fbd49fd8130e8e295774aa9dfeb84f34aec191872569665`  
		Last Modified: Fri, 29 Sep 2023 19:29:46 GMT  
		Size: 2.3 MB (2280831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ab1c2aa4a9bd2cf26470d4a68b1adddc4ede0a127bc3e58c67675f9be39b2d`  
		Last Modified: Fri, 29 Sep 2023 19:29:46 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b1c647298a5806b069632bf26a9123073d2e6fe603aa7b55b83bcc3370f2970`  
		Last Modified: Fri, 29 Sep 2023 20:12:11 GMT  
		Size: 9.7 MB (9745734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29feecf70dcceefb09dc67128ccdd0ecebc069afc29c84c9853f0a9ba6ffdd73`  
		Last Modified: Fri, 29 Sep 2023 20:12:09 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbe243da98f864346f2177531540a62578a5cbd7f9f28eb535390ae195df6e9`  
		Last Modified: Fri, 29 Sep 2023 20:12:09 GMT  
		Size: 1.5 KB (1471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:node` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:9a0f79ed710800179506279f8abf519d2212fb2442c58130e994abd08d09c541
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **373.7 MB (373674910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46fc524ca4f70502a07c6995aa6dfc61c0bd1fa20d500d61386f005d8139e836`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:20 GMT
ADD file:46dcdcde338d2c01fed5db3fac9041736d9305145d8fc2039dd5b3714d38ede8 in / 
# Wed, 20 Sep 2023 02:44:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:24:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:25:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:26:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 11:57:12 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Fri, 29 Sep 2023 20:33:52 GMT
ENV NODE_VERSION=20.8.0
# Fri, 29 Sep 2023 20:34:06 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     4ED778F539E3634C779C87C6D7062848A1AB005C     141F07595B7B3FFE74309A937405533BE57C7D57     74F12602B6F1C4E913FAA37AD3A89613643B6201     DD792F5973C6DE52C432CBDAC77ABFA00DDBF2B7     61FC681DFB92A079F1685E77973F295594EC4689     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4     C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     108F52B48DB57BB0CC439B2997B01419BD92F80A     A363A499291CBBC940DD62E41F10027AF002F8B0   ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Fri, 29 Sep 2023 20:34:07 GMT
ENV YARN_VERSION=1.22.19
# Fri, 29 Sep 2023 20:34:10 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Fri, 29 Sep 2023 20:34:10 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 29 Sep 2023 20:34:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Sep 2023 20:34:10 GMT
CMD ["node"]
# Fri, 29 Sep 2023 21:30:12 GMT
LABEL org.opencontainers.image.title=Unit (node20)
# Fri, 29 Sep 2023 21:30:12 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Fri, 29 Sep 2023 21:30:12 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Fri, 29 Sep 2023 21:30:12 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Fri, 29 Sep 2023 21:30:12 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Fri, 29 Sep 2023 21:30:13 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Fri, 29 Sep 2023 21:30:13 GMT
LABEL org.opencontainers.image.version=1.31.0
# Fri, 29 Sep 2023 21:31:03 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && npm -g install node-gyp     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure nodejs --node-gyp=/usr/local/bin/node-gyp     && make -j $NCPU node node-install libunit-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure nodejs --node-gyp=/usr/local/bin/node-gyp     && make -j $NCPU node node-install libunit-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && rm -rf /root/.cache/ && rm -rf /root/.npm     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Fri, 29 Sep 2023 21:31:03 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Fri, 29 Sep 2023 21:31:03 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Fri, 29 Sep 2023 21:31:03 GMT
STOPSIGNAL SIGTERM
# Fri, 29 Sep 2023 21:31:03 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Fri, 29 Sep 2023 21:31:03 GMT
EXPOSE 80
# Fri, 29 Sep 2023 21:31:03 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:31f5dc1f52c865588c43d8ec718f14d430e149b28f0b28232da825da7ae28f76`  
		Last Modified: Wed, 20 Sep 2023 02:47:53 GMT  
		Size: 53.7 MB (53704892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb60045eb75c62e890b95d28e4893132a6c7d61ec9979104ee4ff6e86c4badee`  
		Last Modified: Wed, 20 Sep 2023 09:33:11 GMT  
		Size: 15.7 MB (15746671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292737ab468ef80c6f78bdde4896157b8953d1e5556e1e526f40aeadcb547573`  
		Last Modified: Wed, 20 Sep 2023 09:33:26 GMT  
		Size: 54.7 MB (54676309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d93979d624211374be152eee1c99ed4ca9e6bae68694135fc440ab6c8fd2044`  
		Last Modified: Wed, 20 Sep 2023 09:33:51 GMT  
		Size: 189.8 MB (189778334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb09eadf5e4e66f30b34eb75eb93cef58634d965f2a8ac2e17dc33d89c4080f`  
		Last Modified: Wed, 20 Sep 2023 12:04:28 GMT  
		Size: 4.2 KB (4204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24debdbd9457a0eb10a03ae601118a956b98fa2398012c256f56bf86c85f3e82`  
		Last Modified: Fri, 29 Sep 2023 20:39:17 GMT  
		Size: 47.9 MB (47887557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0420cb46253f07a9a438ceb9fb754f50231810e402e5d0cc102c603ab7a81e63`  
		Last Modified: Fri, 29 Sep 2023 20:39:12 GMT  
		Size: 2.3 MB (2280989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5352f9acdfe7faf9aca15154311a32d6202f149fe040531018acccc56a009fc`  
		Last Modified: Fri, 29 Sep 2023 20:39:11 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c2ebc1082453fd2911237585674e39ca8703025029b63cfd45f948f78517be`  
		Last Modified: Fri, 29 Sep 2023 21:31:46 GMT  
		Size: 9.6 MB (9592758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e88f1e59c0db97a5a8f3b473c48187fb5c181f7e0466fe4e6b67abe6a0ba0ce`  
		Last Modified: Fri, 29 Sep 2023 21:31:45 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b45aeeecd92e7513ded27236a3f362b72a18420700fb28ca4e7bc6db3068b0`  
		Last Modified: Fri, 29 Sep 2023 21:31:45 GMT  
		Size: 1.5 KB (1468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `unit:node18`

```console
$ docker pull unit@sha256:e68a25b71a9114a0044cdaea34df4cadde567335b2787fa4b2d7da011256bcc4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:node18` - linux; amd64

```console
$ docker pull unit@sha256:fa50021bd72995919e871c6f1d02261d4692a610e7ac7c03915a37f8514dcedc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **395.6 MB (395574915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53d99c0dc02a1abd926ee6f0b175466990afae60a9bd60c3091a263668c02bb4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 04:55:51 GMT
ADD file:85db4f4c5016f51f7112a5d09cb7d4620f565a1379ae4b8a03c5ffc23886a876 in / 
# Wed, 20 Sep 2023 04:55:51 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:22:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:22:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:23:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 03:33:48 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Thu, 12 Oct 2023 00:11:34 GMT
ENV NODE_VERSION=18.18.1
# Thu, 12 Oct 2023 00:11:50 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     4ED778F539E3634C779C87C6D7062848A1AB005C     141F07595B7B3FFE74309A937405533BE57C7D57     74F12602B6F1C4E913FAA37AD3A89613643B6201     DD792F5973C6DE52C432CBDAC77ABFA00DDBF2B7     61FC681DFB92A079F1685E77973F295594EC4689     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4     C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     108F52B48DB57BB0CC439B2997B01419BD92F80A     A363A499291CBBC940DD62E41F10027AF002F8B0   ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Thu, 12 Oct 2023 00:11:51 GMT
ENV YARN_VERSION=1.22.19
# Thu, 12 Oct 2023 00:11:54 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Thu, 12 Oct 2023 00:11:54 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Thu, 12 Oct 2023 00:11:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 Oct 2023 00:11:54 GMT
CMD ["node"]
# Thu, 12 Oct 2023 05:51:37 GMT
LABEL org.opencontainers.image.title=Unit (node18)
# Thu, 12 Oct 2023 05:51:37 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Thu, 12 Oct 2023 05:51:37 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Thu, 12 Oct 2023 05:51:37 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Thu, 12 Oct 2023 05:51:37 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Thu, 12 Oct 2023 05:51:37 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Thu, 12 Oct 2023 05:51:37 GMT
LABEL org.opencontainers.image.version=1.31.0
# Thu, 12 Oct 2023 05:52:44 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && npm -g install node-gyp     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure nodejs --node-gyp=/usr/local/bin/node-gyp     && make -j $NCPU node node-install libunit-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure nodejs --node-gyp=/usr/local/bin/node-gyp     && make -j $NCPU node node-install libunit-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && rm -rf /root/.cache/ && rm -rf /root/.npm     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Thu, 12 Oct 2023 05:52:45 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Thu, 12 Oct 2023 05:52:45 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Thu, 12 Oct 2023 05:52:45 GMT
STOPSIGNAL SIGTERM
# Thu, 12 Oct 2023 05:52:45 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 12 Oct 2023 05:52:45 GMT
EXPOSE 80
# Thu, 12 Oct 2023 05:52:45 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:ddf874abf16cc990e0fd75a154a34ca0a03ee310ad895a18fb62ae15bf4171fb`  
		Last Modified: Wed, 20 Sep 2023 05:00:41 GMT  
		Size: 55.1 MB (55056714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1459d3ab8b5e46ac1a0a00134fe2f7b693474eb6d75ace97ecbe811a6f5b0e`  
		Last Modified: Wed, 20 Sep 2023 09:31:06 GMT  
		Size: 15.8 MB (15760408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab00e7798a04602c3f6e2dc445a994d75e96c45533cd44701f58509982a8c5`  
		Last Modified: Wed, 20 Sep 2023 09:31:23 GMT  
		Size: 54.6 MB (54584790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7883a473306cf6632abe7e913e0f1a21ac2fed038a4116473b25738b8b88b294`  
		Last Modified: Wed, 20 Sep 2023 09:31:55 GMT  
		Size: 196.8 MB (196842512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ea6a75eb435af25ba0b42343548bee2f6eb322326d98e39823aa45c2ff2b21`  
		Last Modified: Thu, 21 Sep 2023 03:37:33 GMT  
		Size: 4.2 KB (4201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bdebbc0d5036b999a378c1ca2357cf358ab6ecfdd8896372522f140f4cc843a`  
		Last Modified: Thu, 12 Oct 2023 00:18:24 GMT  
		Size: 45.9 MB (45920712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff7a673b7589fa8817b773a39cf9b4090edaed28fd18f6519b4ef530251d4c9`  
		Last Modified: Thu, 12 Oct 2023 00:18:17 GMT  
		Size: 2.3 MB (2282356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11925737d6f606c4cc192f42f33a4d08b7888d13dffc884c7d5d0acb4c84189f`  
		Last Modified: Thu, 12 Oct 2023 00:18:17 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1460cb765d966efc06550cd495ceab89c072bd5091310515f25f4e1daafd641`  
		Last Modified: Thu, 12 Oct 2023 05:55:04 GMT  
		Size: 25.1 MB (25120029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cbba6d81182e15ddd86af1b2c9855f06dff1725d982b28d8cb8b52dd8cb1aa3`  
		Last Modified: Thu, 12 Oct 2023 05:55:00 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:728963f3a996e7f4d5cd802fb3dc0e43ce45414eb200a37a594445342c1c7cf0`  
		Last Modified: Thu, 12 Oct 2023 05:55:00 GMT  
		Size: 1.5 KB (1468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:node18` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:45ac93d65b15ac754ec07e25f60788514fa0b08dd4f09df5994030f0c3fc7657
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **371.8 MB (371830804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07b42b9a686c23bf7326fceb8a9cecb28e2756776f609c8c0c364657995b3e52`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:20 GMT
ADD file:46dcdcde338d2c01fed5db3fac9041736d9305145d8fc2039dd5b3714d38ede8 in / 
# Wed, 20 Sep 2023 02:44:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:24:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:25:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:26:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 11:57:12 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Wed, 20 Sep 2023 12:00:25 GMT
ENV NODE_VERSION=18.18.0
# Wed, 20 Sep 2023 12:00:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     4ED778F539E3634C779C87C6D7062848A1AB005C     141F07595B7B3FFE74309A937405533BE57C7D57     74F12602B6F1C4E913FAA37AD3A89613643B6201     DD792F5973C6DE52C432CBDAC77ABFA00DDBF2B7     61FC681DFB92A079F1685E77973F295594EC4689     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4     C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     108F52B48DB57BB0CC439B2997B01419BD92F80A     A363A499291CBBC940DD62E41F10027AF002F8B0   ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Wed, 20 Sep 2023 12:00:41 GMT
ENV YARN_VERSION=1.22.19
# Wed, 20 Sep 2023 12:00:43 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Wed, 20 Sep 2023 12:00:44 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Wed, 20 Sep 2023 12:00:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Sep 2023 12:00:44 GMT
CMD ["node"]
# Wed, 20 Sep 2023 16:35:00 GMT
LABEL org.opencontainers.image.title=Unit (node18)
# Wed, 20 Sep 2023 16:35:00 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Wed, 20 Sep 2023 16:35:00 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Wed, 20 Sep 2023 16:35:00 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Wed, 20 Sep 2023 16:35:00 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Wed, 20 Sep 2023 16:35:00 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 20 Sep 2023 16:35:01 GMT
LABEL org.opencontainers.image.version=1.31.0
# Wed, 20 Sep 2023 16:35:48 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && npm -g install node-gyp     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure nodejs --node-gyp=/usr/local/bin/node-gyp     && make -j $NCPU node node-install libunit-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure nodejs --node-gyp=/usr/local/bin/node-gyp     && make -j $NCPU node node-install libunit-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && rm -rf /root/.cache/ && rm -rf /root/.npm     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Wed, 20 Sep 2023 16:35:49 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Wed, 20 Sep 2023 16:35:49 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Wed, 20 Sep 2023 16:35:49 GMT
STOPSIGNAL SIGTERM
# Wed, 20 Sep 2023 16:35:49 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Wed, 20 Sep 2023 16:35:49 GMT
EXPOSE 80
# Wed, 20 Sep 2023 16:35:49 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:31f5dc1f52c865588c43d8ec718f14d430e149b28f0b28232da825da7ae28f76`  
		Last Modified: Wed, 20 Sep 2023 02:47:53 GMT  
		Size: 53.7 MB (53704892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb60045eb75c62e890b95d28e4893132a6c7d61ec9979104ee4ff6e86c4badee`  
		Last Modified: Wed, 20 Sep 2023 09:33:11 GMT  
		Size: 15.7 MB (15746671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292737ab468ef80c6f78bdde4896157b8953d1e5556e1e526f40aeadcb547573`  
		Last Modified: Wed, 20 Sep 2023 09:33:26 GMT  
		Size: 54.7 MB (54676309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d93979d624211374be152eee1c99ed4ca9e6bae68694135fc440ab6c8fd2044`  
		Last Modified: Wed, 20 Sep 2023 09:33:51 GMT  
		Size: 189.8 MB (189778334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb09eadf5e4e66f30b34eb75eb93cef58634d965f2a8ac2e17dc33d89c4080f`  
		Last Modified: Wed, 20 Sep 2023 12:04:28 GMT  
		Size: 4.2 KB (4204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e4f179e1dbb42e377b9b3f6063a56f2c2123ebf49298a91892232927a0813a`  
		Last Modified: Wed, 20 Sep 2023 12:07:07 GMT  
		Size: 46.0 MB (46042536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9f5fbe4a6f071732862a0191dcefbe066c976172f11bdf45c6f480f6514e9f`  
		Last Modified: Wed, 20 Sep 2023 12:07:02 GMT  
		Size: 2.3 MB (2282453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6c3942de3b3640682578129a868919d480f825bbd409d9010c4205b8da3694`  
		Last Modified: Wed, 20 Sep 2023 12:07:01 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15348bc59ac653a1eca05468f9b80d95633effc2ecb5990010669d62125f1fdf`  
		Last Modified: Wed, 20 Sep 2023 16:47:35 GMT  
		Size: 9.6 MB (9592214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bae505592bea869518bd481ff8fc7683c43aa12820c7538593a449f458dcaba`  
		Last Modified: Wed, 20 Sep 2023 16:47:33 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b8b268e85b393e5d4752e8d08749afb692adf8611ad2b45034fea3e959ae88`  
		Last Modified: Wed, 20 Sep 2023 16:47:33 GMT  
		Size: 1.5 KB (1466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `unit:node20`

```console
$ docker pull unit@sha256:2e5fdd933383b2f8b36ddd1ff597467b8f7fb6082b30afcca4c574a3c79f24aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:node20` - linux; amd64

```console
$ docker pull unit@sha256:9a17e1115cff9de798eee7bb865e2e74f001de34c20b6fc2b44c868f94a45d83
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **382.2 MB (382169133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ce8f24e50447c2c131f7c2f7aa0edb8605448cae812158185bf76cd3dffa3fd`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 04:55:51 GMT
ADD file:85db4f4c5016f51f7112a5d09cb7d4620f565a1379ae4b8a03c5ffc23886a876 in / 
# Wed, 20 Sep 2023 04:55:51 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:22:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:22:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:23:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 03:33:48 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Fri, 29 Sep 2023 19:24:14 GMT
ENV NODE_VERSION=20.8.0
# Fri, 29 Sep 2023 19:24:30 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     4ED778F539E3634C779C87C6D7062848A1AB005C     141F07595B7B3FFE74309A937405533BE57C7D57     74F12602B6F1C4E913FAA37AD3A89613643B6201     DD792F5973C6DE52C432CBDAC77ABFA00DDBF2B7     61FC681DFB92A079F1685E77973F295594EC4689     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4     C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     108F52B48DB57BB0CC439B2997B01419BD92F80A     A363A499291CBBC940DD62E41F10027AF002F8B0   ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Fri, 29 Sep 2023 19:24:31 GMT
ENV YARN_VERSION=1.22.19
# Fri, 29 Sep 2023 19:24:34 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Fri, 29 Sep 2023 19:24:34 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 29 Sep 2023 19:24:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Sep 2023 19:24:34 GMT
CMD ["node"]
# Fri, 29 Sep 2023 20:10:13 GMT
LABEL org.opencontainers.image.title=Unit (node20)
# Fri, 29 Sep 2023 20:10:13 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Fri, 29 Sep 2023 20:10:14 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Fri, 29 Sep 2023 20:10:14 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Fri, 29 Sep 2023 20:10:14 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Fri, 29 Sep 2023 20:10:14 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Fri, 29 Sep 2023 20:10:14 GMT
LABEL org.opencontainers.image.version=1.31.0
# Fri, 29 Sep 2023 20:11:13 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && npm -g install node-gyp     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure nodejs --node-gyp=/usr/local/bin/node-gyp     && make -j $NCPU node node-install libunit-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure nodejs --node-gyp=/usr/local/bin/node-gyp     && make -j $NCPU node node-install libunit-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && rm -rf /root/.cache/ && rm -rf /root/.npm     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Fri, 29 Sep 2023 20:11:13 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Fri, 29 Sep 2023 20:11:13 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Fri, 29 Sep 2023 20:11:13 GMT
STOPSIGNAL SIGTERM
# Fri, 29 Sep 2023 20:11:13 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Fri, 29 Sep 2023 20:11:14 GMT
EXPOSE 80
# Fri, 29 Sep 2023 20:11:14 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:ddf874abf16cc990e0fd75a154a34ca0a03ee310ad895a18fb62ae15bf4171fb`  
		Last Modified: Wed, 20 Sep 2023 05:00:41 GMT  
		Size: 55.1 MB (55056714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1459d3ab8b5e46ac1a0a00134fe2f7b693474eb6d75ace97ecbe811a6f5b0e`  
		Last Modified: Wed, 20 Sep 2023 09:31:06 GMT  
		Size: 15.8 MB (15760408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab00e7798a04602c3f6e2dc445a994d75e96c45533cd44701f58509982a8c5`  
		Last Modified: Wed, 20 Sep 2023 09:31:23 GMT  
		Size: 54.6 MB (54584790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7883a473306cf6632abe7e913e0f1a21ac2fed038a4116473b25738b8b88b294`  
		Last Modified: Wed, 20 Sep 2023 09:31:55 GMT  
		Size: 196.8 MB (196842512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ea6a75eb435af25ba0b42343548bee2f6eb322326d98e39823aa45c2ff2b21`  
		Last Modified: Thu, 21 Sep 2023 03:37:33 GMT  
		Size: 4.2 KB (4201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4adcb3caaf61e057ad5e1d45646af5af38d7ed33278d2648d3673a3813a5ad0`  
		Last Modified: Fri, 29 Sep 2023 19:29:53 GMT  
		Size: 47.9 MB (47890750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074c9dbbb6a5fe5d4fbd49fd8130e8e295774aa9dfeb84f34aec191872569665`  
		Last Modified: Fri, 29 Sep 2023 19:29:46 GMT  
		Size: 2.3 MB (2280831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ab1c2aa4a9bd2cf26470d4a68b1adddc4ede0a127bc3e58c67675f9be39b2d`  
		Last Modified: Fri, 29 Sep 2023 19:29:46 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b1c647298a5806b069632bf26a9123073d2e6fe603aa7b55b83bcc3370f2970`  
		Last Modified: Fri, 29 Sep 2023 20:12:11 GMT  
		Size: 9.7 MB (9745734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29feecf70dcceefb09dc67128ccdd0ecebc069afc29c84c9853f0a9ba6ffdd73`  
		Last Modified: Fri, 29 Sep 2023 20:12:09 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbe243da98f864346f2177531540a62578a5cbd7f9f28eb535390ae195df6e9`  
		Last Modified: Fri, 29 Sep 2023 20:12:09 GMT  
		Size: 1.5 KB (1471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:node20` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:9a0f79ed710800179506279f8abf519d2212fb2442c58130e994abd08d09c541
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **373.7 MB (373674910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46fc524ca4f70502a07c6995aa6dfc61c0bd1fa20d500d61386f005d8139e836`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:20 GMT
ADD file:46dcdcde338d2c01fed5db3fac9041736d9305145d8fc2039dd5b3714d38ede8 in / 
# Wed, 20 Sep 2023 02:44:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:24:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:25:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:26:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 11:57:12 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Fri, 29 Sep 2023 20:33:52 GMT
ENV NODE_VERSION=20.8.0
# Fri, 29 Sep 2023 20:34:06 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     4ED778F539E3634C779C87C6D7062848A1AB005C     141F07595B7B3FFE74309A937405533BE57C7D57     74F12602B6F1C4E913FAA37AD3A89613643B6201     DD792F5973C6DE52C432CBDAC77ABFA00DDBF2B7     61FC681DFB92A079F1685E77973F295594EC4689     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4     C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     108F52B48DB57BB0CC439B2997B01419BD92F80A     A363A499291CBBC940DD62E41F10027AF002F8B0   ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Fri, 29 Sep 2023 20:34:07 GMT
ENV YARN_VERSION=1.22.19
# Fri, 29 Sep 2023 20:34:10 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Fri, 29 Sep 2023 20:34:10 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 29 Sep 2023 20:34:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Sep 2023 20:34:10 GMT
CMD ["node"]
# Fri, 29 Sep 2023 21:30:12 GMT
LABEL org.opencontainers.image.title=Unit (node20)
# Fri, 29 Sep 2023 21:30:12 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Fri, 29 Sep 2023 21:30:12 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Fri, 29 Sep 2023 21:30:12 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Fri, 29 Sep 2023 21:30:12 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Fri, 29 Sep 2023 21:30:13 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Fri, 29 Sep 2023 21:30:13 GMT
LABEL org.opencontainers.image.version=1.31.0
# Fri, 29 Sep 2023 21:31:03 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && npm -g install node-gyp     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure nodejs --node-gyp=/usr/local/bin/node-gyp     && make -j $NCPU node node-install libunit-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure nodejs --node-gyp=/usr/local/bin/node-gyp     && make -j $NCPU node node-install libunit-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && rm -rf /root/.cache/ && rm -rf /root/.npm     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Fri, 29 Sep 2023 21:31:03 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Fri, 29 Sep 2023 21:31:03 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Fri, 29 Sep 2023 21:31:03 GMT
STOPSIGNAL SIGTERM
# Fri, 29 Sep 2023 21:31:03 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Fri, 29 Sep 2023 21:31:03 GMT
EXPOSE 80
# Fri, 29 Sep 2023 21:31:03 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:31f5dc1f52c865588c43d8ec718f14d430e149b28f0b28232da825da7ae28f76`  
		Last Modified: Wed, 20 Sep 2023 02:47:53 GMT  
		Size: 53.7 MB (53704892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb60045eb75c62e890b95d28e4893132a6c7d61ec9979104ee4ff6e86c4badee`  
		Last Modified: Wed, 20 Sep 2023 09:33:11 GMT  
		Size: 15.7 MB (15746671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292737ab468ef80c6f78bdde4896157b8953d1e5556e1e526f40aeadcb547573`  
		Last Modified: Wed, 20 Sep 2023 09:33:26 GMT  
		Size: 54.7 MB (54676309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d93979d624211374be152eee1c99ed4ca9e6bae68694135fc440ab6c8fd2044`  
		Last Modified: Wed, 20 Sep 2023 09:33:51 GMT  
		Size: 189.8 MB (189778334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb09eadf5e4e66f30b34eb75eb93cef58634d965f2a8ac2e17dc33d89c4080f`  
		Last Modified: Wed, 20 Sep 2023 12:04:28 GMT  
		Size: 4.2 KB (4204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24debdbd9457a0eb10a03ae601118a956b98fa2398012c256f56bf86c85f3e82`  
		Last Modified: Fri, 29 Sep 2023 20:39:17 GMT  
		Size: 47.9 MB (47887557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0420cb46253f07a9a438ceb9fb754f50231810e402e5d0cc102c603ab7a81e63`  
		Last Modified: Fri, 29 Sep 2023 20:39:12 GMT  
		Size: 2.3 MB (2280989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5352f9acdfe7faf9aca15154311a32d6202f149fe040531018acccc56a009fc`  
		Last Modified: Fri, 29 Sep 2023 20:39:11 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c2ebc1082453fd2911237585674e39ca8703025029b63cfd45f948f78517be`  
		Last Modified: Fri, 29 Sep 2023 21:31:46 GMT  
		Size: 9.6 MB (9592758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e88f1e59c0db97a5a8f3b473c48187fb5c181f7e0466fe4e6b67abe6a0ba0ce`  
		Last Modified: Fri, 29 Sep 2023 21:31:45 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b45aeeecd92e7513ded27236a3f362b72a18420700fb28ca4e7bc6db3068b0`  
		Last Modified: Fri, 29 Sep 2023 21:31:45 GMT  
		Size: 1.5 KB (1468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `unit:perl`

```console
$ docker pull unit@sha256:3c8e1eace3473a976477d60002f38209ae5ed55cf67898083eb6e9c688ceca09
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:perl` - linux; amd64

```console
$ docker pull unit@sha256:5c8da37c00d90a41311793367b010c025b198bca791f4a48c1917dd5972ac6aa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **345.1 MB (345143371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f90ea950a89663407724e0fadeea9c93e63be29cb6cbd80b2223e894425414b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 04:55:51 GMT
ADD file:85db4f4c5016f51f7112a5d09cb7d4620f565a1379ae4b8a03c5ffc23886a876 in / 
# Wed, 20 Sep 2023 04:55:51 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:22:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:22:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:23:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 12:31:20 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 20 Sep 2023 12:31:20 GMT
WORKDIR /usr/src/perl
# Wed, 20 Sep 2023 12:36:40 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Wed, 20 Sep 2023 12:36:40 GMT
WORKDIR /usr/src/app
# Wed, 20 Sep 2023 12:36:40 GMT
CMD ["perl5.38.0" "-de0"]
# Wed, 20 Sep 2023 21:38:09 GMT
LABEL org.opencontainers.image.title=Unit (perl5.38)
# Wed, 20 Sep 2023 21:38:09 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Wed, 20 Sep 2023 21:38:09 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Wed, 20 Sep 2023 21:38:09 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Wed, 20 Sep 2023 21:38:09 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Wed, 20 Sep 2023 21:38:09 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 20 Sep 2023 21:38:09 GMT
LABEL org.opencontainers.image.version=1.31.0
# Wed, 20 Sep 2023 21:39:01 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure perl     && make -j $NCPU perl-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure perl     && make -j $NCPU perl-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Wed, 20 Sep 2023 21:39:01 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Wed, 20 Sep 2023 21:39:01 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Wed, 20 Sep 2023 21:39:01 GMT
STOPSIGNAL SIGTERM
# Wed, 20 Sep 2023 21:39:01 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Wed, 20 Sep 2023 21:39:02 GMT
EXPOSE 80
# Wed, 20 Sep 2023 21:39:02 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:ddf874abf16cc990e0fd75a154a34ca0a03ee310ad895a18fb62ae15bf4171fb`  
		Last Modified: Wed, 20 Sep 2023 05:00:41 GMT  
		Size: 55.1 MB (55056714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1459d3ab8b5e46ac1a0a00134fe2f7b693474eb6d75ace97ecbe811a6f5b0e`  
		Last Modified: Wed, 20 Sep 2023 09:31:06 GMT  
		Size: 15.8 MB (15760408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab00e7798a04602c3f6e2dc445a994d75e96c45533cd44701f58509982a8c5`  
		Last Modified: Wed, 20 Sep 2023 09:31:23 GMT  
		Size: 54.6 MB (54584790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7883a473306cf6632abe7e913e0f1a21ac2fed038a4116473b25738b8b88b294`  
		Last Modified: Wed, 20 Sep 2023 09:31:55 GMT  
		Size: 196.8 MB (196842512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52b3edeb95fa7a0041689ffc83f83c850c381908d41acdd82e901f87878cdfd`  
		Last Modified: Wed, 20 Sep 2023 16:26:00 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024bd37d7f953a74bb38362b5317ae998d40ca2fee8b8a8dca43148a8a3f4cfb`  
		Last Modified: Wed, 20 Sep 2023 16:26:03 GMT  
		Size: 15.6 MB (15635163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587b5a52835c5daacc0e54325851e643a1154769e8db9e765060b7fc4b43493d`  
		Last Modified: Wed, 20 Sep 2023 16:26:00 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66dfb10c0b36ce058292ef115f82b9ac08a5475f9e99e422fce5aabd7c51ba1f`  
		Last Modified: Wed, 20 Sep 2023 21:42:45 GMT  
		Size: 7.3 MB (7260721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f52778a1e6d26c16c061d9f1f0ce15b47ae70e29ba231b39f9e8ec2efe2ba4`  
		Last Modified: Wed, 20 Sep 2023 21:42:43 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fb22967b16e13a68371214b23ec1abf149a140a54d40230ae032b26df9d492`  
		Last Modified: Wed, 20 Sep 2023 21:42:43 GMT  
		Size: 1.5 KB (1468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:perl` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:215346afdcf662582d06311303dc561b27195a9cd91b6b832805b504ecf15d32
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.6 MB (336614710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72b2d67a5c47a9faffd0dfa45b15e7e137607ed5b61f6a4c5fa0ce4e1b7b6fef`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:20 GMT
ADD file:46dcdcde338d2c01fed5db3fac9041736d9305145d8fc2039dd5b3714d38ede8 in / 
# Wed, 20 Sep 2023 02:44:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:24:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:25:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:26:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 12:49:59 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 20 Sep 2023 12:49:59 GMT
WORKDIR /usr/src/perl
# Wed, 20 Sep 2023 12:54:12 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Wed, 20 Sep 2023 12:54:13 GMT
WORKDIR /usr/src/app
# Wed, 20 Sep 2023 12:54:13 GMT
CMD ["perl5.38.0" "-de0"]
# Wed, 20 Sep 2023 16:35:58 GMT
LABEL org.opencontainers.image.title=Unit (perl5.38)
# Wed, 20 Sep 2023 16:35:58 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Wed, 20 Sep 2023 16:35:58 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Wed, 20 Sep 2023 16:35:58 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Wed, 20 Sep 2023 16:35:58 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Wed, 20 Sep 2023 16:35:58 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 20 Sep 2023 16:35:58 GMT
LABEL org.opencontainers.image.version=1.31.0
# Wed, 20 Sep 2023 16:36:39 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure perl     && make -j $NCPU perl-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure perl     && make -j $NCPU perl-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Wed, 20 Sep 2023 16:36:39 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Wed, 20 Sep 2023 16:36:39 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Wed, 20 Sep 2023 16:36:39 GMT
STOPSIGNAL SIGTERM
# Wed, 20 Sep 2023 16:36:39 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Wed, 20 Sep 2023 16:36:39 GMT
EXPOSE 80
# Wed, 20 Sep 2023 16:36:39 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:31f5dc1f52c865588c43d8ec718f14d430e149b28f0b28232da825da7ae28f76`  
		Last Modified: Wed, 20 Sep 2023 02:47:53 GMT  
		Size: 53.7 MB (53704892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb60045eb75c62e890b95d28e4893132a6c7d61ec9979104ee4ff6e86c4badee`  
		Last Modified: Wed, 20 Sep 2023 09:33:11 GMT  
		Size: 15.7 MB (15746671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292737ab468ef80c6f78bdde4896157b8953d1e5556e1e526f40aeadcb547573`  
		Last Modified: Wed, 20 Sep 2023 09:33:26 GMT  
		Size: 54.7 MB (54676309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d93979d624211374be152eee1c99ed4ca9e6bae68694135fc440ab6c8fd2044`  
		Last Modified: Wed, 20 Sep 2023 09:33:51 GMT  
		Size: 189.8 MB (189778334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1117f9029f2f12e3c0ea1a49d453513b6d3c4ec5a2cf433fd56be576e3c53290`  
		Last Modified: Wed, 20 Sep 2023 15:58:14 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b317f1f02fe8dd016d19c93440ae1ccfd4b40693bf91614faefd972e49128e`  
		Last Modified: Wed, 20 Sep 2023 15:58:16 GMT  
		Size: 15.6 MB (15569671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4ff545690965c4c8230cb542b04cbb5df00908ce2f26782b952990cb2a2dcf`  
		Last Modified: Wed, 20 Sep 2023 15:58:14 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e086d049566a67139ff421c28ba34c3a886279adff787914ca7d2c24aaca14b`  
		Last Modified: Wed, 20 Sep 2023 16:47:45 GMT  
		Size: 7.1 MB (7135766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dfd51d8d916894d7797d4c9a60e0eac911429596844e9663d88aea528066cfc`  
		Last Modified: Wed, 20 Sep 2023 16:47:44 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b8a03d176384e4135d0956f78c091cced19e54a2a562bf63b3224dea0a2197`  
		Last Modified: Wed, 20 Sep 2023 16:47:44 GMT  
		Size: 1.5 KB (1471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `unit:perl5`

```console
$ docker pull unit@sha256:3c8e1eace3473a976477d60002f38209ae5ed55cf67898083eb6e9c688ceca09
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:perl5` - linux; amd64

```console
$ docker pull unit@sha256:5c8da37c00d90a41311793367b010c025b198bca791f4a48c1917dd5972ac6aa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **345.1 MB (345143371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f90ea950a89663407724e0fadeea9c93e63be29cb6cbd80b2223e894425414b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 04:55:51 GMT
ADD file:85db4f4c5016f51f7112a5d09cb7d4620f565a1379ae4b8a03c5ffc23886a876 in / 
# Wed, 20 Sep 2023 04:55:51 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:22:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:22:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:23:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 12:31:20 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 20 Sep 2023 12:31:20 GMT
WORKDIR /usr/src/perl
# Wed, 20 Sep 2023 12:36:40 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Wed, 20 Sep 2023 12:36:40 GMT
WORKDIR /usr/src/app
# Wed, 20 Sep 2023 12:36:40 GMT
CMD ["perl5.38.0" "-de0"]
# Wed, 20 Sep 2023 21:38:09 GMT
LABEL org.opencontainers.image.title=Unit (perl5.38)
# Wed, 20 Sep 2023 21:38:09 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Wed, 20 Sep 2023 21:38:09 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Wed, 20 Sep 2023 21:38:09 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Wed, 20 Sep 2023 21:38:09 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Wed, 20 Sep 2023 21:38:09 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 20 Sep 2023 21:38:09 GMT
LABEL org.opencontainers.image.version=1.31.0
# Wed, 20 Sep 2023 21:39:01 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure perl     && make -j $NCPU perl-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure perl     && make -j $NCPU perl-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Wed, 20 Sep 2023 21:39:01 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Wed, 20 Sep 2023 21:39:01 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Wed, 20 Sep 2023 21:39:01 GMT
STOPSIGNAL SIGTERM
# Wed, 20 Sep 2023 21:39:01 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Wed, 20 Sep 2023 21:39:02 GMT
EXPOSE 80
# Wed, 20 Sep 2023 21:39:02 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:ddf874abf16cc990e0fd75a154a34ca0a03ee310ad895a18fb62ae15bf4171fb`  
		Last Modified: Wed, 20 Sep 2023 05:00:41 GMT  
		Size: 55.1 MB (55056714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1459d3ab8b5e46ac1a0a00134fe2f7b693474eb6d75ace97ecbe811a6f5b0e`  
		Last Modified: Wed, 20 Sep 2023 09:31:06 GMT  
		Size: 15.8 MB (15760408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab00e7798a04602c3f6e2dc445a994d75e96c45533cd44701f58509982a8c5`  
		Last Modified: Wed, 20 Sep 2023 09:31:23 GMT  
		Size: 54.6 MB (54584790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7883a473306cf6632abe7e913e0f1a21ac2fed038a4116473b25738b8b88b294`  
		Last Modified: Wed, 20 Sep 2023 09:31:55 GMT  
		Size: 196.8 MB (196842512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52b3edeb95fa7a0041689ffc83f83c850c381908d41acdd82e901f87878cdfd`  
		Last Modified: Wed, 20 Sep 2023 16:26:00 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024bd37d7f953a74bb38362b5317ae998d40ca2fee8b8a8dca43148a8a3f4cfb`  
		Last Modified: Wed, 20 Sep 2023 16:26:03 GMT  
		Size: 15.6 MB (15635163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587b5a52835c5daacc0e54325851e643a1154769e8db9e765060b7fc4b43493d`  
		Last Modified: Wed, 20 Sep 2023 16:26:00 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66dfb10c0b36ce058292ef115f82b9ac08a5475f9e99e422fce5aabd7c51ba1f`  
		Last Modified: Wed, 20 Sep 2023 21:42:45 GMT  
		Size: 7.3 MB (7260721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f52778a1e6d26c16c061d9f1f0ce15b47ae70e29ba231b39f9e8ec2efe2ba4`  
		Last Modified: Wed, 20 Sep 2023 21:42:43 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fb22967b16e13a68371214b23ec1abf149a140a54d40230ae032b26df9d492`  
		Last Modified: Wed, 20 Sep 2023 21:42:43 GMT  
		Size: 1.5 KB (1468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:perl5` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:215346afdcf662582d06311303dc561b27195a9cd91b6b832805b504ecf15d32
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.6 MB (336614710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72b2d67a5c47a9faffd0dfa45b15e7e137607ed5b61f6a4c5fa0ce4e1b7b6fef`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:20 GMT
ADD file:46dcdcde338d2c01fed5db3fac9041736d9305145d8fc2039dd5b3714d38ede8 in / 
# Wed, 20 Sep 2023 02:44:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:24:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:25:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:26:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 12:49:59 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 20 Sep 2023 12:49:59 GMT
WORKDIR /usr/src/perl
# Wed, 20 Sep 2023 12:54:12 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Wed, 20 Sep 2023 12:54:13 GMT
WORKDIR /usr/src/app
# Wed, 20 Sep 2023 12:54:13 GMT
CMD ["perl5.38.0" "-de0"]
# Wed, 20 Sep 2023 16:35:58 GMT
LABEL org.opencontainers.image.title=Unit (perl5.38)
# Wed, 20 Sep 2023 16:35:58 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Wed, 20 Sep 2023 16:35:58 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Wed, 20 Sep 2023 16:35:58 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Wed, 20 Sep 2023 16:35:58 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Wed, 20 Sep 2023 16:35:58 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 20 Sep 2023 16:35:58 GMT
LABEL org.opencontainers.image.version=1.31.0
# Wed, 20 Sep 2023 16:36:39 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure perl     && make -j $NCPU perl-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure perl     && make -j $NCPU perl-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Wed, 20 Sep 2023 16:36:39 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Wed, 20 Sep 2023 16:36:39 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Wed, 20 Sep 2023 16:36:39 GMT
STOPSIGNAL SIGTERM
# Wed, 20 Sep 2023 16:36:39 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Wed, 20 Sep 2023 16:36:39 GMT
EXPOSE 80
# Wed, 20 Sep 2023 16:36:39 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:31f5dc1f52c865588c43d8ec718f14d430e149b28f0b28232da825da7ae28f76`  
		Last Modified: Wed, 20 Sep 2023 02:47:53 GMT  
		Size: 53.7 MB (53704892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb60045eb75c62e890b95d28e4893132a6c7d61ec9979104ee4ff6e86c4badee`  
		Last Modified: Wed, 20 Sep 2023 09:33:11 GMT  
		Size: 15.7 MB (15746671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292737ab468ef80c6f78bdde4896157b8953d1e5556e1e526f40aeadcb547573`  
		Last Modified: Wed, 20 Sep 2023 09:33:26 GMT  
		Size: 54.7 MB (54676309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d93979d624211374be152eee1c99ed4ca9e6bae68694135fc440ab6c8fd2044`  
		Last Modified: Wed, 20 Sep 2023 09:33:51 GMT  
		Size: 189.8 MB (189778334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1117f9029f2f12e3c0ea1a49d453513b6d3c4ec5a2cf433fd56be576e3c53290`  
		Last Modified: Wed, 20 Sep 2023 15:58:14 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b317f1f02fe8dd016d19c93440ae1ccfd4b40693bf91614faefd972e49128e`  
		Last Modified: Wed, 20 Sep 2023 15:58:16 GMT  
		Size: 15.6 MB (15569671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4ff545690965c4c8230cb542b04cbb5df00908ce2f26782b952990cb2a2dcf`  
		Last Modified: Wed, 20 Sep 2023 15:58:14 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e086d049566a67139ff421c28ba34c3a886279adff787914ca7d2c24aaca14b`  
		Last Modified: Wed, 20 Sep 2023 16:47:45 GMT  
		Size: 7.1 MB (7135766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dfd51d8d916894d7797d4c9a60e0eac911429596844e9663d88aea528066cfc`  
		Last Modified: Wed, 20 Sep 2023 16:47:44 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b8a03d176384e4135d0956f78c091cced19e54a2a562bf63b3224dea0a2197`  
		Last Modified: Wed, 20 Sep 2023 16:47:44 GMT  
		Size: 1.5 KB (1471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `unit:perl5.36`

```console
$ docker pull unit@sha256:e0f01023f2b4a55743f179baa4df204e66de3b578d76c5751a8e23be8b77c589
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:perl5.36` - linux; amd64

```console
$ docker pull unit@sha256:ef50de0b9c58bbbd5847056f3c7e4729038d51221785c34997b5cc71aad4932b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.7 MB (344722709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ba2be77e69bbbc055fdbf3993f1f99d53ab5bb80978b32f5b6cda84becdd29b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 04:55:51 GMT
ADD file:85db4f4c5016f51f7112a5d09cb7d4620f565a1379ae4b8a03c5ffc23886a876 in / 
# Wed, 20 Sep 2023 04:55:51 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:22:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:22:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:23:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 12:31:20 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 20 Sep 2023 12:31:20 GMT
WORKDIR /usr/src/perl
# Wed, 20 Sep 2023 13:49:26 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.1.tar.xz -o perl-5.36.1.tar.xz     && echo 'bd91217ea8a8c8b81f21ebbb6cefdf0d13ae532013f944cdece2cd51aef4b6a7 *perl-5.36.1.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.1.tar.xz -C /usr/src/perl     && rm perl-5.36.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Wed, 20 Sep 2023 13:49:27 GMT
WORKDIR /usr/src/app
# Wed, 20 Sep 2023 13:49:27 GMT
CMD ["perl5.36.1" "-de0"]
# Wed, 20 Sep 2023 21:39:07 GMT
LABEL org.opencontainers.image.title=Unit (perl5.36)
# Wed, 20 Sep 2023 21:39:08 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Wed, 20 Sep 2023 21:39:08 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Wed, 20 Sep 2023 21:39:08 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Wed, 20 Sep 2023 21:39:08 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Wed, 20 Sep 2023 21:39:08 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 20 Sep 2023 21:39:08 GMT
LABEL org.opencontainers.image.version=1.31.0
# Wed, 20 Sep 2023 21:39:58 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure perl     && make -j $NCPU perl-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure perl     && make -j $NCPU perl-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Wed, 20 Sep 2023 21:39:58 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Wed, 20 Sep 2023 21:39:59 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Wed, 20 Sep 2023 21:39:59 GMT
STOPSIGNAL SIGTERM
# Wed, 20 Sep 2023 21:39:59 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Wed, 20 Sep 2023 21:39:59 GMT
EXPOSE 80
# Wed, 20 Sep 2023 21:39:59 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:ddf874abf16cc990e0fd75a154a34ca0a03ee310ad895a18fb62ae15bf4171fb`  
		Last Modified: Wed, 20 Sep 2023 05:00:41 GMT  
		Size: 55.1 MB (55056714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1459d3ab8b5e46ac1a0a00134fe2f7b693474eb6d75ace97ecbe811a6f5b0e`  
		Last Modified: Wed, 20 Sep 2023 09:31:06 GMT  
		Size: 15.8 MB (15760408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab00e7798a04602c3f6e2dc445a994d75e96c45533cd44701f58509982a8c5`  
		Last Modified: Wed, 20 Sep 2023 09:31:23 GMT  
		Size: 54.6 MB (54584790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7883a473306cf6632abe7e913e0f1a21ac2fed038a4116473b25738b8b88b294`  
		Last Modified: Wed, 20 Sep 2023 09:31:55 GMT  
		Size: 196.8 MB (196842512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52b3edeb95fa7a0041689ffc83f83c850c381908d41acdd82e901f87878cdfd`  
		Last Modified: Wed, 20 Sep 2023 16:26:00 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801fec7181e64cb33e9618fc12991ed305fdc90cb37ba97513a9814b7da3b14d`  
		Last Modified: Wed, 20 Sep 2023 16:30:09 GMT  
		Size: 15.2 MB (15226973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13355de3cf006b6d46c2682a3c1a7980543832e27a6814162bcf2c11c78f4bac`  
		Last Modified: Wed, 20 Sep 2023 16:30:06 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1fde6eb25125a7410bf2ba9789a64d9d0b9f3b2e6bcfdfbb463132c6ec08df4`  
		Last Modified: Wed, 20 Sep 2023 21:42:59 GMT  
		Size: 7.2 MB (7248249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0d21cdf1397df3869aba37cbca4e46d401c97eabf8dfab51c9a1f1d7257128`  
		Last Modified: Wed, 20 Sep 2023 21:42:57 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8684e4982998d379d595ff34fce63e1ee9a5364e73b2b00ffb4f0f1fe2aff25b`  
		Last Modified: Wed, 20 Sep 2023 21:42:57 GMT  
		Size: 1.5 KB (1467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:perl5.36` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:0765c0cce675be3ac6160eef54947c98d790882fac94ca2e62d7432f8a710267
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.2 MB (336198228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c76a0625c259cb3b83797c395eab3e7b7f3b7f827bdf5bc3264262653a723e0`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:20 GMT
ADD file:46dcdcde338d2c01fed5db3fac9041736d9305145d8fc2039dd5b3714d38ede8 in / 
# Wed, 20 Sep 2023 02:44:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:24:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:25:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:26:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 12:49:59 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 20 Sep 2023 12:49:59 GMT
WORKDIR /usr/src/perl
# Wed, 20 Sep 2023 13:52:05 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.1.tar.xz -o perl-5.36.1.tar.xz     && echo 'bd91217ea8a8c8b81f21ebbb6cefdf0d13ae532013f944cdece2cd51aef4b6a7 *perl-5.36.1.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.1.tar.xz -C /usr/src/perl     && rm perl-5.36.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Wed, 20 Sep 2023 13:52:06 GMT
WORKDIR /usr/src/app
# Wed, 20 Sep 2023 13:52:06 GMT
CMD ["perl5.36.1" "-de0"]
# Wed, 20 Sep 2023 16:36:46 GMT
LABEL org.opencontainers.image.title=Unit (perl5.36)
# Wed, 20 Sep 2023 16:36:46 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Wed, 20 Sep 2023 16:36:46 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Wed, 20 Sep 2023 16:36:46 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Wed, 20 Sep 2023 16:36:46 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Wed, 20 Sep 2023 16:36:46 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 20 Sep 2023 16:36:46 GMT
LABEL org.opencontainers.image.version=1.31.0
# Wed, 20 Sep 2023 16:37:27 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure perl     && make -j $NCPU perl-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure perl     && make -j $NCPU perl-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Wed, 20 Sep 2023 16:37:27 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Wed, 20 Sep 2023 16:37:27 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Wed, 20 Sep 2023 16:37:27 GMT
STOPSIGNAL SIGTERM
# Wed, 20 Sep 2023 16:37:27 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Wed, 20 Sep 2023 16:37:27 GMT
EXPOSE 80
# Wed, 20 Sep 2023 16:37:27 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:31f5dc1f52c865588c43d8ec718f14d430e149b28f0b28232da825da7ae28f76`  
		Last Modified: Wed, 20 Sep 2023 02:47:53 GMT  
		Size: 53.7 MB (53704892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb60045eb75c62e890b95d28e4893132a6c7d61ec9979104ee4ff6e86c4badee`  
		Last Modified: Wed, 20 Sep 2023 09:33:11 GMT  
		Size: 15.7 MB (15746671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292737ab468ef80c6f78bdde4896157b8953d1e5556e1e526f40aeadcb547573`  
		Last Modified: Wed, 20 Sep 2023 09:33:26 GMT  
		Size: 54.7 MB (54676309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d93979d624211374be152eee1c99ed4ca9e6bae68694135fc440ab6c8fd2044`  
		Last Modified: Wed, 20 Sep 2023 09:33:51 GMT  
		Size: 189.8 MB (189778334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1117f9029f2f12e3c0ea1a49d453513b6d3c4ec5a2cf433fd56be576e3c53290`  
		Last Modified: Wed, 20 Sep 2023 15:58:14 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8093c0fb05a13b2a87dc07b437542e7a922365faaa15cbce8f4d7384483a02e`  
		Last Modified: Wed, 20 Sep 2023 16:02:31 GMT  
		Size: 15.2 MB (15164956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f04ba44dcfc11add9e8950c97672f1d8fbd34378618fda92771d4fc1f7d89e61`  
		Last Modified: Wed, 20 Sep 2023 16:02:29 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6686249ee24f0cea74da9d6bd6af97ab214e86c31ddbf1a6240ceb6d85e58b9`  
		Last Modified: Wed, 20 Sep 2023 16:48:00 GMT  
		Size: 7.1 MB (7124001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0e3baba03795b87967e901297e79c21e3bc8e1575373ee369d36f0b78b8b35`  
		Last Modified: Wed, 20 Sep 2023 16:47:59 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f15f31f41115dc86198f9372e52e119c904149c9a09c4660c16f458d434c15a`  
		Last Modified: Wed, 20 Sep 2023 16:47:59 GMT  
		Size: 1.5 KB (1466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `unit:perl5.38`

```console
$ docker pull unit@sha256:3c8e1eace3473a976477d60002f38209ae5ed55cf67898083eb6e9c688ceca09
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:perl5.38` - linux; amd64

```console
$ docker pull unit@sha256:5c8da37c00d90a41311793367b010c025b198bca791f4a48c1917dd5972ac6aa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **345.1 MB (345143371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f90ea950a89663407724e0fadeea9c93e63be29cb6cbd80b2223e894425414b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 04:55:51 GMT
ADD file:85db4f4c5016f51f7112a5d09cb7d4620f565a1379ae4b8a03c5ffc23886a876 in / 
# Wed, 20 Sep 2023 04:55:51 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:22:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:22:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:23:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 12:31:20 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 20 Sep 2023 12:31:20 GMT
WORKDIR /usr/src/perl
# Wed, 20 Sep 2023 12:36:40 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Wed, 20 Sep 2023 12:36:40 GMT
WORKDIR /usr/src/app
# Wed, 20 Sep 2023 12:36:40 GMT
CMD ["perl5.38.0" "-de0"]
# Wed, 20 Sep 2023 21:38:09 GMT
LABEL org.opencontainers.image.title=Unit (perl5.38)
# Wed, 20 Sep 2023 21:38:09 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Wed, 20 Sep 2023 21:38:09 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Wed, 20 Sep 2023 21:38:09 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Wed, 20 Sep 2023 21:38:09 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Wed, 20 Sep 2023 21:38:09 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 20 Sep 2023 21:38:09 GMT
LABEL org.opencontainers.image.version=1.31.0
# Wed, 20 Sep 2023 21:39:01 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure perl     && make -j $NCPU perl-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure perl     && make -j $NCPU perl-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Wed, 20 Sep 2023 21:39:01 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Wed, 20 Sep 2023 21:39:01 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Wed, 20 Sep 2023 21:39:01 GMT
STOPSIGNAL SIGTERM
# Wed, 20 Sep 2023 21:39:01 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Wed, 20 Sep 2023 21:39:02 GMT
EXPOSE 80
# Wed, 20 Sep 2023 21:39:02 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:ddf874abf16cc990e0fd75a154a34ca0a03ee310ad895a18fb62ae15bf4171fb`  
		Last Modified: Wed, 20 Sep 2023 05:00:41 GMT  
		Size: 55.1 MB (55056714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1459d3ab8b5e46ac1a0a00134fe2f7b693474eb6d75ace97ecbe811a6f5b0e`  
		Last Modified: Wed, 20 Sep 2023 09:31:06 GMT  
		Size: 15.8 MB (15760408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab00e7798a04602c3f6e2dc445a994d75e96c45533cd44701f58509982a8c5`  
		Last Modified: Wed, 20 Sep 2023 09:31:23 GMT  
		Size: 54.6 MB (54584790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7883a473306cf6632abe7e913e0f1a21ac2fed038a4116473b25738b8b88b294`  
		Last Modified: Wed, 20 Sep 2023 09:31:55 GMT  
		Size: 196.8 MB (196842512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52b3edeb95fa7a0041689ffc83f83c850c381908d41acdd82e901f87878cdfd`  
		Last Modified: Wed, 20 Sep 2023 16:26:00 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024bd37d7f953a74bb38362b5317ae998d40ca2fee8b8a8dca43148a8a3f4cfb`  
		Last Modified: Wed, 20 Sep 2023 16:26:03 GMT  
		Size: 15.6 MB (15635163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587b5a52835c5daacc0e54325851e643a1154769e8db9e765060b7fc4b43493d`  
		Last Modified: Wed, 20 Sep 2023 16:26:00 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66dfb10c0b36ce058292ef115f82b9ac08a5475f9e99e422fce5aabd7c51ba1f`  
		Last Modified: Wed, 20 Sep 2023 21:42:45 GMT  
		Size: 7.3 MB (7260721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f52778a1e6d26c16c061d9f1f0ce15b47ae70e29ba231b39f9e8ec2efe2ba4`  
		Last Modified: Wed, 20 Sep 2023 21:42:43 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fb22967b16e13a68371214b23ec1abf149a140a54d40230ae032b26df9d492`  
		Last Modified: Wed, 20 Sep 2023 21:42:43 GMT  
		Size: 1.5 KB (1468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:perl5.38` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:215346afdcf662582d06311303dc561b27195a9cd91b6b832805b504ecf15d32
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.6 MB (336614710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72b2d67a5c47a9faffd0dfa45b15e7e137607ed5b61f6a4c5fa0ce4e1b7b6fef`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:20 GMT
ADD file:46dcdcde338d2c01fed5db3fac9041736d9305145d8fc2039dd5b3714d38ede8 in / 
# Wed, 20 Sep 2023 02:44:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:24:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:25:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:26:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 12:49:59 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 20 Sep 2023 12:49:59 GMT
WORKDIR /usr/src/perl
# Wed, 20 Sep 2023 12:54:12 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Wed, 20 Sep 2023 12:54:13 GMT
WORKDIR /usr/src/app
# Wed, 20 Sep 2023 12:54:13 GMT
CMD ["perl5.38.0" "-de0"]
# Wed, 20 Sep 2023 16:35:58 GMT
LABEL org.opencontainers.image.title=Unit (perl5.38)
# Wed, 20 Sep 2023 16:35:58 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Wed, 20 Sep 2023 16:35:58 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Wed, 20 Sep 2023 16:35:58 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Wed, 20 Sep 2023 16:35:58 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Wed, 20 Sep 2023 16:35:58 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 20 Sep 2023 16:35:58 GMT
LABEL org.opencontainers.image.version=1.31.0
# Wed, 20 Sep 2023 16:36:39 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure perl     && make -j $NCPU perl-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure perl     && make -j $NCPU perl-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Wed, 20 Sep 2023 16:36:39 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Wed, 20 Sep 2023 16:36:39 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Wed, 20 Sep 2023 16:36:39 GMT
STOPSIGNAL SIGTERM
# Wed, 20 Sep 2023 16:36:39 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Wed, 20 Sep 2023 16:36:39 GMT
EXPOSE 80
# Wed, 20 Sep 2023 16:36:39 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:31f5dc1f52c865588c43d8ec718f14d430e149b28f0b28232da825da7ae28f76`  
		Last Modified: Wed, 20 Sep 2023 02:47:53 GMT  
		Size: 53.7 MB (53704892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb60045eb75c62e890b95d28e4893132a6c7d61ec9979104ee4ff6e86c4badee`  
		Last Modified: Wed, 20 Sep 2023 09:33:11 GMT  
		Size: 15.7 MB (15746671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292737ab468ef80c6f78bdde4896157b8953d1e5556e1e526f40aeadcb547573`  
		Last Modified: Wed, 20 Sep 2023 09:33:26 GMT  
		Size: 54.7 MB (54676309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d93979d624211374be152eee1c99ed4ca9e6bae68694135fc440ab6c8fd2044`  
		Last Modified: Wed, 20 Sep 2023 09:33:51 GMT  
		Size: 189.8 MB (189778334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1117f9029f2f12e3c0ea1a49d453513b6d3c4ec5a2cf433fd56be576e3c53290`  
		Last Modified: Wed, 20 Sep 2023 15:58:14 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b317f1f02fe8dd016d19c93440ae1ccfd4b40693bf91614faefd972e49128e`  
		Last Modified: Wed, 20 Sep 2023 15:58:16 GMT  
		Size: 15.6 MB (15569671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4ff545690965c4c8230cb542b04cbb5df00908ce2f26782b952990cb2a2dcf`  
		Last Modified: Wed, 20 Sep 2023 15:58:14 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e086d049566a67139ff421c28ba34c3a886279adff787914ca7d2c24aaca14b`  
		Last Modified: Wed, 20 Sep 2023 16:47:45 GMT  
		Size: 7.1 MB (7135766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dfd51d8d916894d7797d4c9a60e0eac911429596844e9663d88aea528066cfc`  
		Last Modified: Wed, 20 Sep 2023 16:47:44 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b8a03d176384e4135d0956f78c091cced19e54a2a562bf63b3224dea0a2197`  
		Last Modified: Wed, 20 Sep 2023 16:47:44 GMT  
		Size: 1.5 KB (1471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `unit:php`

```console
$ docker pull unit@sha256:98a08f025af091d8e63156d9913c2264b8bd2fe6f7fd76eac388713ffff7cd7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:php` - linux; amd64

```console
$ docker pull unit@sha256:3489384ba2bdfa707d08431b335b0f776c206863e93e5998892199036d767468
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.3 MB (177316657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1376dc93023d0e476b2a7d5762eede2dc29c43a2ef48986784e2b83701098818`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:51:31 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 12 Oct 2023 03:51:31 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 12 Oct 2023 03:51:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:51:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 12 Oct 2023 03:51:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 12 Oct 2023 03:51:50 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 12 Oct 2023 03:51:50 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 12 Oct 2023 03:51:50 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 12 Oct 2023 04:20:25 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 12 Oct 2023 04:20:25 GMT
ENV PHP_VERSION=8.2.11
# Thu, 12 Oct 2023 04:20:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.11.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.11.tar.xz.asc
# Thu, 12 Oct 2023 04:20:25 GMT
ENV PHP_SHA256=29af82e4f7509831490552918aad502697453f0869a579ee1b80b08f9112c5b8
# Thu, 12 Oct 2023 04:20:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 12 Oct 2023 04:20:38 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 12 Oct 2023 04:23:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--enable-embed 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 12 Oct 2023 04:23:40 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 12 Oct 2023 04:23:40 GMT
RUN docker-php-ext-enable sodium
# Thu, 12 Oct 2023 04:23:41 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 12 Oct 2023 04:23:41 GMT
CMD ["php" "-a"]
# Thu, 12 Oct 2023 05:53:05 GMT
LABEL org.opencontainers.image.title=Unit (php8.2)
# Thu, 12 Oct 2023 05:53:05 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Thu, 12 Oct 2023 05:53:06 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Thu, 12 Oct 2023 05:53:06 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Thu, 12 Oct 2023 05:53:06 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Thu, 12 Oct 2023 05:53:06 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Thu, 12 Oct 2023 05:53:06 GMT
LABEL org.opencontainers.image.version=1.31.0
# Thu, 12 Oct 2023 05:54:04 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure php     && make -j $NCPU php-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure php     && make -j $NCPU php-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && ldconfig     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Thu, 12 Oct 2023 05:54:04 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Thu, 12 Oct 2023 05:54:05 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Thu, 12 Oct 2023 05:54:05 GMT
STOPSIGNAL SIGTERM
# Thu, 12 Oct 2023 05:54:05 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 12 Oct 2023 05:54:05 GMT
EXPOSE 80
# Thu, 12 Oct 2023 05:54:05 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a19ba793cb30aa4b42c5ad97548d55ae00fec0c4877c76126583715d708ce9`  
		Last Modified: Thu, 12 Oct 2023 05:32:53 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e4193503519ae06279df9269c22245e20b0acb785371e054e848264cb901c2`  
		Last Modified: Thu, 12 Oct 2023 05:33:06 GMT  
		Size: 91.6 MB (91635233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de997c28946e5c94cd3025094a7aee8f9df3ea9dedc8e2d250d1edd5786ca21`  
		Last Modified: Thu, 12 Oct 2023 05:32:53 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:873f439f47bcfe71f69387163cbdee5f5916f1a239621af82adeb6545c8ebc9e`  
		Last Modified: Thu, 12 Oct 2023 05:36:20 GMT  
		Size: 12.4 MB (12366685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f4856de7837698b7c3f763062a2517b23adf18b5f61951f75c45e4f2f44b48`  
		Last Modified: Thu, 12 Oct 2023 05:36:19 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732fb5749b825ba822de67840caf6e00fc3c04541a5fb4da950ef79484b9a212`  
		Last Modified: Thu, 12 Oct 2023 05:36:24 GMT  
		Size: 34.6 MB (34578752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b802f88bd6721adf7730d5d3d154ec4fb86d8a0ba9b5a68e8b21f0641788cc`  
		Last Modified: Thu, 12 Oct 2023 05:36:19 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc1bfbe94373cbbdf1f91bd9f7d1ce800915c9dff4534f9e480b565522cea63`  
		Last Modified: Thu, 12 Oct 2023 05:36:19 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c18b9d27728522e863897b864d23bab4ac72a317b907a4947385190fa8cd76`  
		Last Modified: Thu, 12 Oct 2023 05:55:17 GMT  
		Size: 7.3 MB (7311692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d399b38b2e7a680119855d6a3c02175a9fca6045029fe034007c7c35159138`  
		Last Modified: Thu, 12 Oct 2023 05:55:16 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdd7d3b6ce6a617dbb942596a3aaf0ed6d14fefa6f7c507122bb9988213382ca`  
		Last Modified: Thu, 12 Oct 2023 05:55:16 GMT  
		Size: 1.5 KB (1473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:php` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:9437be31a41199971c8c97470dc6210d02940181cf88412da7418b328e6fb65e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.0 MB (171047539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80a74fa49a48de50ce64633c1cfc1d6e8319ebf8d0900de19dce27e35f4cc22c`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:28 GMT
ADD file:024479be439b4ecb37c939e68673adc72955f3345ca0e809bd13e897709e59e4 in / 
# Wed, 20 Sep 2023 02:44:28 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 03:08:10 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 03:08:10 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 03:08:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 03:08:28 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 03:08:28 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 03:08:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 03:08:29 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 03:08:29 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 03:34:37 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Sat, 30 Sep 2023 02:00:47 GMT
ENV PHP_VERSION=8.2.11
# Sat, 30 Sep 2023 02:00:47 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.11.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.11.tar.xz.asc
# Sat, 30 Sep 2023 02:00:47 GMT
ENV PHP_SHA256=29af82e4f7509831490552918aad502697453f0869a579ee1b80b08f9112c5b8
# Sat, 30 Sep 2023 02:00:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 30 Sep 2023 02:00:57 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 30 Sep 2023 02:03:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--enable-embed 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 30 Sep 2023 02:03:41 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Sat, 30 Sep 2023 02:03:42 GMT
RUN docker-php-ext-enable sodium
# Sat, 30 Sep 2023 02:03:42 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 30 Sep 2023 02:03:42 GMT
CMD ["php" "-a"]
# Sat, 30 Sep 2023 06:58:25 GMT
LABEL org.opencontainers.image.title=Unit (php8.2)
# Sat, 30 Sep 2023 06:58:25 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Sat, 30 Sep 2023 06:58:25 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Sat, 30 Sep 2023 06:58:25 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Sat, 30 Sep 2023 06:58:25 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Sat, 30 Sep 2023 06:58:25 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Sat, 30 Sep 2023 06:58:26 GMT
LABEL org.opencontainers.image.version=1.31.0
# Sat, 30 Sep 2023 06:59:14 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure php     && make -j $NCPU php-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure php     && make -j $NCPU php-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && ldconfig     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Sat, 30 Sep 2023 06:59:14 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Sat, 30 Sep 2023 06:59:15 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Sat, 30 Sep 2023 06:59:15 GMT
STOPSIGNAL SIGTERM
# Sat, 30 Sep 2023 06:59:15 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Sat, 30 Sep 2023 06:59:15 GMT
EXPOSE 80
# Sat, 30 Sep 2023 06:59:15 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:fc521c5b98350f6fd8c72ace1e48558bb7b53cb3db201a2a3b42095401cd02f1`  
		Last Modified: Wed, 20 Sep 2023 02:48:13 GMT  
		Size: 30.1 MB (30062869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011d119a94c0f59e8eabde01f2b7a4da9d92360102426dcaad9d1d0be4b4092c`  
		Last Modified: Wed, 20 Sep 2023 06:01:09 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c2e7320620034b78e6c4122bdaf225b766ba582397845df17e1ca60098d29c`  
		Last Modified: Wed, 20 Sep 2023 06:01:20 GMT  
		Size: 86.9 MB (86929113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aff55be7dadd795271386506373641b927cc6f05b8efda3e6ff839f8419b6b1`  
		Last Modified: Wed, 20 Sep 2023 06:01:09 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454bbb352bd352bcfb21a488d3c30d4c5bd361cc4d710c6c074ee2b2a195c427`  
		Last Modified: Sat, 30 Sep 2023 03:44:41 GMT  
		Size: 12.4 MB (12364849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ed8e7b4178686ac6d44751dfb2df41c828db70441a966b5e9990ced097a483`  
		Last Modified: Sat, 30 Sep 2023 03:44:39 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe154f23538ad101fbd710d1152a33004c79ccdc6e535141f45e8338ea0d95d`  
		Last Modified: Sat, 30 Sep 2023 03:44:43 GMT  
		Size: 34.5 MB (34500324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4112cbf9310ae8cf8dd3cafe076e961454810770e4d6754f569e84f41eefb654`  
		Last Modified: Sat, 30 Sep 2023 03:44:39 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c11bd2118fe41faeb02374298f96d20fd1856d59a76c721cf384b44839e6582`  
		Last Modified: Sat, 30 Sep 2023 03:44:39 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050dd55155fdfd13168a12283c20639e5417b26741fd7b2176631945880a03f4`  
		Last Modified: Sat, 30 Sep 2023 07:00:01 GMT  
		Size: 7.2 MB (7183962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb54f4b569069290b7de89ebf3fb8ad666b51d307f3a23d3bd934fe26b1438d`  
		Last Modified: Sat, 30 Sep 2023 07:00:00 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fba378c9872d4d6a4444ea03d8a49f1eca4fc97928ac5aa68c747896ec36daf`  
		Last Modified: Sat, 30 Sep 2023 07:00:00 GMT  
		Size: 1.5 KB (1468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `unit:php8`

```console
$ docker pull unit@sha256:98a08f025af091d8e63156d9913c2264b8bd2fe6f7fd76eac388713ffff7cd7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:php8` - linux; amd64

```console
$ docker pull unit@sha256:3489384ba2bdfa707d08431b335b0f776c206863e93e5998892199036d767468
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.3 MB (177316657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1376dc93023d0e476b2a7d5762eede2dc29c43a2ef48986784e2b83701098818`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:51:31 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 12 Oct 2023 03:51:31 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 12 Oct 2023 03:51:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:51:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 12 Oct 2023 03:51:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 12 Oct 2023 03:51:50 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 12 Oct 2023 03:51:50 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 12 Oct 2023 03:51:50 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 12 Oct 2023 04:20:25 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 12 Oct 2023 04:20:25 GMT
ENV PHP_VERSION=8.2.11
# Thu, 12 Oct 2023 04:20:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.11.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.11.tar.xz.asc
# Thu, 12 Oct 2023 04:20:25 GMT
ENV PHP_SHA256=29af82e4f7509831490552918aad502697453f0869a579ee1b80b08f9112c5b8
# Thu, 12 Oct 2023 04:20:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 12 Oct 2023 04:20:38 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 12 Oct 2023 04:23:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--enable-embed 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 12 Oct 2023 04:23:40 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 12 Oct 2023 04:23:40 GMT
RUN docker-php-ext-enable sodium
# Thu, 12 Oct 2023 04:23:41 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 12 Oct 2023 04:23:41 GMT
CMD ["php" "-a"]
# Thu, 12 Oct 2023 05:53:05 GMT
LABEL org.opencontainers.image.title=Unit (php8.2)
# Thu, 12 Oct 2023 05:53:05 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Thu, 12 Oct 2023 05:53:06 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Thu, 12 Oct 2023 05:53:06 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Thu, 12 Oct 2023 05:53:06 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Thu, 12 Oct 2023 05:53:06 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Thu, 12 Oct 2023 05:53:06 GMT
LABEL org.opencontainers.image.version=1.31.0
# Thu, 12 Oct 2023 05:54:04 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure php     && make -j $NCPU php-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure php     && make -j $NCPU php-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && ldconfig     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Thu, 12 Oct 2023 05:54:04 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Thu, 12 Oct 2023 05:54:05 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Thu, 12 Oct 2023 05:54:05 GMT
STOPSIGNAL SIGTERM
# Thu, 12 Oct 2023 05:54:05 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 12 Oct 2023 05:54:05 GMT
EXPOSE 80
# Thu, 12 Oct 2023 05:54:05 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a19ba793cb30aa4b42c5ad97548d55ae00fec0c4877c76126583715d708ce9`  
		Last Modified: Thu, 12 Oct 2023 05:32:53 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e4193503519ae06279df9269c22245e20b0acb785371e054e848264cb901c2`  
		Last Modified: Thu, 12 Oct 2023 05:33:06 GMT  
		Size: 91.6 MB (91635233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de997c28946e5c94cd3025094a7aee8f9df3ea9dedc8e2d250d1edd5786ca21`  
		Last Modified: Thu, 12 Oct 2023 05:32:53 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:873f439f47bcfe71f69387163cbdee5f5916f1a239621af82adeb6545c8ebc9e`  
		Last Modified: Thu, 12 Oct 2023 05:36:20 GMT  
		Size: 12.4 MB (12366685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f4856de7837698b7c3f763062a2517b23adf18b5f61951f75c45e4f2f44b48`  
		Last Modified: Thu, 12 Oct 2023 05:36:19 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732fb5749b825ba822de67840caf6e00fc3c04541a5fb4da950ef79484b9a212`  
		Last Modified: Thu, 12 Oct 2023 05:36:24 GMT  
		Size: 34.6 MB (34578752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b802f88bd6721adf7730d5d3d154ec4fb86d8a0ba9b5a68e8b21f0641788cc`  
		Last Modified: Thu, 12 Oct 2023 05:36:19 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc1bfbe94373cbbdf1f91bd9f7d1ce800915c9dff4534f9e480b565522cea63`  
		Last Modified: Thu, 12 Oct 2023 05:36:19 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c18b9d27728522e863897b864d23bab4ac72a317b907a4947385190fa8cd76`  
		Last Modified: Thu, 12 Oct 2023 05:55:17 GMT  
		Size: 7.3 MB (7311692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d399b38b2e7a680119855d6a3c02175a9fca6045029fe034007c7c35159138`  
		Last Modified: Thu, 12 Oct 2023 05:55:16 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdd7d3b6ce6a617dbb942596a3aaf0ed6d14fefa6f7c507122bb9988213382ca`  
		Last Modified: Thu, 12 Oct 2023 05:55:16 GMT  
		Size: 1.5 KB (1473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:php8` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:9437be31a41199971c8c97470dc6210d02940181cf88412da7418b328e6fb65e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.0 MB (171047539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80a74fa49a48de50ce64633c1cfc1d6e8319ebf8d0900de19dce27e35f4cc22c`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:28 GMT
ADD file:024479be439b4ecb37c939e68673adc72955f3345ca0e809bd13e897709e59e4 in / 
# Wed, 20 Sep 2023 02:44:28 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 03:08:10 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 03:08:10 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 03:08:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 03:08:28 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 03:08:28 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 03:08:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 03:08:29 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 03:08:29 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 03:34:37 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Sat, 30 Sep 2023 02:00:47 GMT
ENV PHP_VERSION=8.2.11
# Sat, 30 Sep 2023 02:00:47 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.11.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.11.tar.xz.asc
# Sat, 30 Sep 2023 02:00:47 GMT
ENV PHP_SHA256=29af82e4f7509831490552918aad502697453f0869a579ee1b80b08f9112c5b8
# Sat, 30 Sep 2023 02:00:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 30 Sep 2023 02:00:57 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 30 Sep 2023 02:03:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--enable-embed 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 30 Sep 2023 02:03:41 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Sat, 30 Sep 2023 02:03:42 GMT
RUN docker-php-ext-enable sodium
# Sat, 30 Sep 2023 02:03:42 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 30 Sep 2023 02:03:42 GMT
CMD ["php" "-a"]
# Sat, 30 Sep 2023 06:58:25 GMT
LABEL org.opencontainers.image.title=Unit (php8.2)
# Sat, 30 Sep 2023 06:58:25 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Sat, 30 Sep 2023 06:58:25 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Sat, 30 Sep 2023 06:58:25 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Sat, 30 Sep 2023 06:58:25 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Sat, 30 Sep 2023 06:58:25 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Sat, 30 Sep 2023 06:58:26 GMT
LABEL org.opencontainers.image.version=1.31.0
# Sat, 30 Sep 2023 06:59:14 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure php     && make -j $NCPU php-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure php     && make -j $NCPU php-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && ldconfig     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Sat, 30 Sep 2023 06:59:14 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Sat, 30 Sep 2023 06:59:15 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Sat, 30 Sep 2023 06:59:15 GMT
STOPSIGNAL SIGTERM
# Sat, 30 Sep 2023 06:59:15 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Sat, 30 Sep 2023 06:59:15 GMT
EXPOSE 80
# Sat, 30 Sep 2023 06:59:15 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:fc521c5b98350f6fd8c72ace1e48558bb7b53cb3db201a2a3b42095401cd02f1`  
		Last Modified: Wed, 20 Sep 2023 02:48:13 GMT  
		Size: 30.1 MB (30062869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011d119a94c0f59e8eabde01f2b7a4da9d92360102426dcaad9d1d0be4b4092c`  
		Last Modified: Wed, 20 Sep 2023 06:01:09 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c2e7320620034b78e6c4122bdaf225b766ba582397845df17e1ca60098d29c`  
		Last Modified: Wed, 20 Sep 2023 06:01:20 GMT  
		Size: 86.9 MB (86929113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aff55be7dadd795271386506373641b927cc6f05b8efda3e6ff839f8419b6b1`  
		Last Modified: Wed, 20 Sep 2023 06:01:09 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454bbb352bd352bcfb21a488d3c30d4c5bd361cc4d710c6c074ee2b2a195c427`  
		Last Modified: Sat, 30 Sep 2023 03:44:41 GMT  
		Size: 12.4 MB (12364849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ed8e7b4178686ac6d44751dfb2df41c828db70441a966b5e9990ced097a483`  
		Last Modified: Sat, 30 Sep 2023 03:44:39 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe154f23538ad101fbd710d1152a33004c79ccdc6e535141f45e8338ea0d95d`  
		Last Modified: Sat, 30 Sep 2023 03:44:43 GMT  
		Size: 34.5 MB (34500324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4112cbf9310ae8cf8dd3cafe076e961454810770e4d6754f569e84f41eefb654`  
		Last Modified: Sat, 30 Sep 2023 03:44:39 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c11bd2118fe41faeb02374298f96d20fd1856d59a76c721cf384b44839e6582`  
		Last Modified: Sat, 30 Sep 2023 03:44:39 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050dd55155fdfd13168a12283c20639e5417b26741fd7b2176631945880a03f4`  
		Last Modified: Sat, 30 Sep 2023 07:00:01 GMT  
		Size: 7.2 MB (7183962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb54f4b569069290b7de89ebf3fb8ad666b51d307f3a23d3bd934fe26b1438d`  
		Last Modified: Sat, 30 Sep 2023 07:00:00 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fba378c9872d4d6a4444ea03d8a49f1eca4fc97928ac5aa68c747896ec36daf`  
		Last Modified: Sat, 30 Sep 2023 07:00:00 GMT  
		Size: 1.5 KB (1468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `unit:php8.2`

```console
$ docker pull unit@sha256:98a08f025af091d8e63156d9913c2264b8bd2fe6f7fd76eac388713ffff7cd7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:php8.2` - linux; amd64

```console
$ docker pull unit@sha256:3489384ba2bdfa707d08431b335b0f776c206863e93e5998892199036d767468
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.3 MB (177316657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1376dc93023d0e476b2a7d5762eede2dc29c43a2ef48986784e2b83701098818`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:51:31 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 12 Oct 2023 03:51:31 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 12 Oct 2023 03:51:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:51:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 12 Oct 2023 03:51:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 12 Oct 2023 03:51:50 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 12 Oct 2023 03:51:50 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 12 Oct 2023 03:51:50 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 12 Oct 2023 04:20:25 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 12 Oct 2023 04:20:25 GMT
ENV PHP_VERSION=8.2.11
# Thu, 12 Oct 2023 04:20:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.11.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.11.tar.xz.asc
# Thu, 12 Oct 2023 04:20:25 GMT
ENV PHP_SHA256=29af82e4f7509831490552918aad502697453f0869a579ee1b80b08f9112c5b8
# Thu, 12 Oct 2023 04:20:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 12 Oct 2023 04:20:38 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 12 Oct 2023 04:23:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--enable-embed 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 12 Oct 2023 04:23:40 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 12 Oct 2023 04:23:40 GMT
RUN docker-php-ext-enable sodium
# Thu, 12 Oct 2023 04:23:41 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 12 Oct 2023 04:23:41 GMT
CMD ["php" "-a"]
# Thu, 12 Oct 2023 05:53:05 GMT
LABEL org.opencontainers.image.title=Unit (php8.2)
# Thu, 12 Oct 2023 05:53:05 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Thu, 12 Oct 2023 05:53:06 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Thu, 12 Oct 2023 05:53:06 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Thu, 12 Oct 2023 05:53:06 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Thu, 12 Oct 2023 05:53:06 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Thu, 12 Oct 2023 05:53:06 GMT
LABEL org.opencontainers.image.version=1.31.0
# Thu, 12 Oct 2023 05:54:04 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure php     && make -j $NCPU php-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure php     && make -j $NCPU php-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && ldconfig     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Thu, 12 Oct 2023 05:54:04 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Thu, 12 Oct 2023 05:54:05 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Thu, 12 Oct 2023 05:54:05 GMT
STOPSIGNAL SIGTERM
# Thu, 12 Oct 2023 05:54:05 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 12 Oct 2023 05:54:05 GMT
EXPOSE 80
# Thu, 12 Oct 2023 05:54:05 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a19ba793cb30aa4b42c5ad97548d55ae00fec0c4877c76126583715d708ce9`  
		Last Modified: Thu, 12 Oct 2023 05:32:53 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e4193503519ae06279df9269c22245e20b0acb785371e054e848264cb901c2`  
		Last Modified: Thu, 12 Oct 2023 05:33:06 GMT  
		Size: 91.6 MB (91635233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de997c28946e5c94cd3025094a7aee8f9df3ea9dedc8e2d250d1edd5786ca21`  
		Last Modified: Thu, 12 Oct 2023 05:32:53 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:873f439f47bcfe71f69387163cbdee5f5916f1a239621af82adeb6545c8ebc9e`  
		Last Modified: Thu, 12 Oct 2023 05:36:20 GMT  
		Size: 12.4 MB (12366685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f4856de7837698b7c3f763062a2517b23adf18b5f61951f75c45e4f2f44b48`  
		Last Modified: Thu, 12 Oct 2023 05:36:19 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732fb5749b825ba822de67840caf6e00fc3c04541a5fb4da950ef79484b9a212`  
		Last Modified: Thu, 12 Oct 2023 05:36:24 GMT  
		Size: 34.6 MB (34578752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b802f88bd6721adf7730d5d3d154ec4fb86d8a0ba9b5a68e8b21f0641788cc`  
		Last Modified: Thu, 12 Oct 2023 05:36:19 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc1bfbe94373cbbdf1f91bd9f7d1ce800915c9dff4534f9e480b565522cea63`  
		Last Modified: Thu, 12 Oct 2023 05:36:19 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c18b9d27728522e863897b864d23bab4ac72a317b907a4947385190fa8cd76`  
		Last Modified: Thu, 12 Oct 2023 05:55:17 GMT  
		Size: 7.3 MB (7311692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d399b38b2e7a680119855d6a3c02175a9fca6045029fe034007c7c35159138`  
		Last Modified: Thu, 12 Oct 2023 05:55:16 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdd7d3b6ce6a617dbb942596a3aaf0ed6d14fefa6f7c507122bb9988213382ca`  
		Last Modified: Thu, 12 Oct 2023 05:55:16 GMT  
		Size: 1.5 KB (1473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:php8.2` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:9437be31a41199971c8c97470dc6210d02940181cf88412da7418b328e6fb65e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.0 MB (171047539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80a74fa49a48de50ce64633c1cfc1d6e8319ebf8d0900de19dce27e35f4cc22c`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:28 GMT
ADD file:024479be439b4ecb37c939e68673adc72955f3345ca0e809bd13e897709e59e4 in / 
# Wed, 20 Sep 2023 02:44:28 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 03:08:10 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 03:08:10 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 03:08:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 03:08:28 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 03:08:28 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 03:08:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 03:08:29 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 03:08:29 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 03:34:37 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Sat, 30 Sep 2023 02:00:47 GMT
ENV PHP_VERSION=8.2.11
# Sat, 30 Sep 2023 02:00:47 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.11.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.11.tar.xz.asc
# Sat, 30 Sep 2023 02:00:47 GMT
ENV PHP_SHA256=29af82e4f7509831490552918aad502697453f0869a579ee1b80b08f9112c5b8
# Sat, 30 Sep 2023 02:00:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 30 Sep 2023 02:00:57 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 30 Sep 2023 02:03:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--enable-embed 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 30 Sep 2023 02:03:41 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Sat, 30 Sep 2023 02:03:42 GMT
RUN docker-php-ext-enable sodium
# Sat, 30 Sep 2023 02:03:42 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 30 Sep 2023 02:03:42 GMT
CMD ["php" "-a"]
# Sat, 30 Sep 2023 06:58:25 GMT
LABEL org.opencontainers.image.title=Unit (php8.2)
# Sat, 30 Sep 2023 06:58:25 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Sat, 30 Sep 2023 06:58:25 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Sat, 30 Sep 2023 06:58:25 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Sat, 30 Sep 2023 06:58:25 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Sat, 30 Sep 2023 06:58:25 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Sat, 30 Sep 2023 06:58:26 GMT
LABEL org.opencontainers.image.version=1.31.0
# Sat, 30 Sep 2023 06:59:14 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure php     && make -j $NCPU php-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure php     && make -j $NCPU php-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && ldconfig     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Sat, 30 Sep 2023 06:59:14 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Sat, 30 Sep 2023 06:59:15 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Sat, 30 Sep 2023 06:59:15 GMT
STOPSIGNAL SIGTERM
# Sat, 30 Sep 2023 06:59:15 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Sat, 30 Sep 2023 06:59:15 GMT
EXPOSE 80
# Sat, 30 Sep 2023 06:59:15 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:fc521c5b98350f6fd8c72ace1e48558bb7b53cb3db201a2a3b42095401cd02f1`  
		Last Modified: Wed, 20 Sep 2023 02:48:13 GMT  
		Size: 30.1 MB (30062869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011d119a94c0f59e8eabde01f2b7a4da9d92360102426dcaad9d1d0be4b4092c`  
		Last Modified: Wed, 20 Sep 2023 06:01:09 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c2e7320620034b78e6c4122bdaf225b766ba582397845df17e1ca60098d29c`  
		Last Modified: Wed, 20 Sep 2023 06:01:20 GMT  
		Size: 86.9 MB (86929113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aff55be7dadd795271386506373641b927cc6f05b8efda3e6ff839f8419b6b1`  
		Last Modified: Wed, 20 Sep 2023 06:01:09 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454bbb352bd352bcfb21a488d3c30d4c5bd361cc4d710c6c074ee2b2a195c427`  
		Last Modified: Sat, 30 Sep 2023 03:44:41 GMT  
		Size: 12.4 MB (12364849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ed8e7b4178686ac6d44751dfb2df41c828db70441a966b5e9990ced097a483`  
		Last Modified: Sat, 30 Sep 2023 03:44:39 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe154f23538ad101fbd710d1152a33004c79ccdc6e535141f45e8338ea0d95d`  
		Last Modified: Sat, 30 Sep 2023 03:44:43 GMT  
		Size: 34.5 MB (34500324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4112cbf9310ae8cf8dd3cafe076e961454810770e4d6754f569e84f41eefb654`  
		Last Modified: Sat, 30 Sep 2023 03:44:39 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c11bd2118fe41faeb02374298f96d20fd1856d59a76c721cf384b44839e6582`  
		Last Modified: Sat, 30 Sep 2023 03:44:39 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050dd55155fdfd13168a12283c20639e5417b26741fd7b2176631945880a03f4`  
		Last Modified: Sat, 30 Sep 2023 07:00:01 GMT  
		Size: 7.2 MB (7183962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb54f4b569069290b7de89ebf3fb8ad666b51d307f3a23d3bd934fe26b1438d`  
		Last Modified: Sat, 30 Sep 2023 07:00:00 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fba378c9872d4d6a4444ea03d8a49f1eca4fc97928ac5aa68c747896ec36daf`  
		Last Modified: Sat, 30 Sep 2023 07:00:00 GMT  
		Size: 1.5 KB (1468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `unit:python`

```console
$ docker pull unit@sha256:97f7574d4ce36f8eca74f25555dce4835dfc479d033acb68e20d19dec141e112
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:python` - linux; amd64

```console
$ docker pull unit@sha256:7e930385f350c30f67fb9d8af68e500c684c6a7037a887fb28e8e9bb17f21a63
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.2 MB (359180856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f539861a71c1bdb6090a4ad0d937ad8e88c23b4e00971e8aee44a140ca84439`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 04:55:51 GMT
ADD file:85db4f4c5016f51f7112a5d09cb7d4620f565a1379ae4b8a03c5ffc23886a876 in / 
# Wed, 20 Sep 2023 04:55:51 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:22:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:22:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:23:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 02 Oct 2023 16:48:26 GMT
ENV LANG=C.UTF-8
# Mon, 02 Oct 2023 16:48:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 02 Oct 2023 16:48:26 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_VERSION=3.11.6
# Mon, 02 Oct 2023 16:48:26 GMT
RUN set -eux; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		bin="$(readlink -ve /usr/local/bin/python3)"; 	dir="$(dirname "$bin")"; 	mkdir -p "/usr/share/gdb/auto-load/$dir"; 	cp -vL Tools/gdb/libpython.py "/usr/share/gdb/auto-load/$bin-gdb.py"; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		python3 --version # buildkit
# Mon, 02 Oct 2023 16:48:26 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_PIP_VERSION=23.2.1
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/9af82b715db434abb94a0a6f3569f43e72157346/public/get-pip.py
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_GET_PIP_SHA256=45a2bb8bf2bb5eff16fdd00faef6f29731831c7c59bd9fc2bf1f3bed511ff1fe
# Mon, 02 Oct 2023 16:48:26 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Mon, 02 Oct 2023 16:48:26 GMT
CMD ["python3"]
# Tue, 03 Oct 2023 04:27:32 GMT
LABEL org.opencontainers.image.title=Unit (python3.11)
# Tue, 03 Oct 2023 04:27:32 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Tue, 03 Oct 2023 04:27:32 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Tue, 03 Oct 2023 04:27:32 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Tue, 03 Oct 2023 04:27:32 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Tue, 03 Oct 2023 04:27:32 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 03 Oct 2023 04:27:33 GMT
LABEL org.opencontainers.image.version=1.31.0
# Tue, 03 Oct 2023 04:28:23 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure python --config=/usr/local/bin/python3-config     && make -j $NCPU python3-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure python --config=/usr/local/bin/python3-config     && make -j $NCPU python3-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Tue, 03 Oct 2023 04:28:23 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Tue, 03 Oct 2023 04:28:23 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Tue, 03 Oct 2023 04:28:24 GMT
STOPSIGNAL SIGTERM
# Tue, 03 Oct 2023 04:28:24 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 03 Oct 2023 04:28:24 GMT
EXPOSE 80
# Tue, 03 Oct 2023 04:28:24 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:ddf874abf16cc990e0fd75a154a34ca0a03ee310ad895a18fb62ae15bf4171fb`  
		Last Modified: Wed, 20 Sep 2023 05:00:41 GMT  
		Size: 55.1 MB (55056714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1459d3ab8b5e46ac1a0a00134fe2f7b693474eb6d75ace97ecbe811a6f5b0e`  
		Last Modified: Wed, 20 Sep 2023 09:31:06 GMT  
		Size: 15.8 MB (15760408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab00e7798a04602c3f6e2dc445a994d75e96c45533cd44701f58509982a8c5`  
		Last Modified: Wed, 20 Sep 2023 09:31:23 GMT  
		Size: 54.6 MB (54584790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7883a473306cf6632abe7e913e0f1a21ac2fed038a4116473b25738b8b88b294`  
		Last Modified: Wed, 20 Sep 2023 09:31:55 GMT  
		Size: 196.8 MB (196842512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ab175b762c07a73f43bc078229d225d45a4810a8f4e8cb19602122986eadb5`  
		Last Modified: Wed, 20 Sep 2023 12:17:10 GMT  
		Size: 6.3 MB (6291084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19164320e566edd82bea237a00344772e5cdaceb1c0581eab62ea66b8a812d5c`  
		Last Modified: Tue, 03 Oct 2023 03:58:29 GMT  
		Size: 20.1 MB (20053476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccfa8e20789038925a7a0ac61d49b8337c2ff7f1b923e8190271a936e206413e`  
		Last Modified: Tue, 03 Oct 2023 03:58:26 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a5bfb4de08e5dbf05e323300db82d3423385e2e4a87ff92c93574cfe940306`  
		Last Modified: Tue, 03 Oct 2023 03:58:26 GMT  
		Size: 3.1 MB (3109666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2853480534c9003652abee52b8564d53ec16ae60da13fdca042d57b323bab888`  
		Last Modified: Tue, 03 Oct 2023 04:29:10 GMT  
		Size: 7.5 MB (7479231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d411f454564bf8a14d13d91dcef8dec6c34ec244c7580c88c8a1d529f08b848`  
		Last Modified: Tue, 03 Oct 2023 04:29:08 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14417cd73e58663a678f0c5a0fce443306ffd56f455e0d42c0264ef51dfadc2a`  
		Last Modified: Tue, 03 Oct 2023 04:29:08 GMT  
		Size: 1.5 KB (1464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:python` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:6fed15916314569b43402551b06ad9ecde8957e827a4628b195d31304271e3ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.7 MB (350717878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:705609da8fdf387160dd80f7413f642a4b06072f958b38bbd8c0137df5d6db1b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:20 GMT
ADD file:46dcdcde338d2c01fed5db3fac9041736d9305145d8fc2039dd5b3714d38ede8 in / 
# Wed, 20 Sep 2023 02:44:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:24:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:25:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:26:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 02 Oct 2023 16:48:26 GMT
ENV LANG=C.UTF-8
# Mon, 02 Oct 2023 16:48:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 02 Oct 2023 16:48:26 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_VERSION=3.11.6
# Mon, 02 Oct 2023 16:48:26 GMT
RUN set -eux; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		bin="$(readlink -ve /usr/local/bin/python3)"; 	dir="$(dirname "$bin")"; 	mkdir -p "/usr/share/gdb/auto-load/$dir"; 	cp -vL Tools/gdb/libpython.py "/usr/share/gdb/auto-load/$bin-gdb.py"; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		python3 --version # buildkit
# Mon, 02 Oct 2023 16:48:26 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_PIP_VERSION=23.2.1
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/9af82b715db434abb94a0a6f3569f43e72157346/public/get-pip.py
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_GET_PIP_SHA256=45a2bb8bf2bb5eff16fdd00faef6f29731831c7c59bd9fc2bf1f3bed511ff1fe
# Mon, 02 Oct 2023 16:48:26 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Mon, 02 Oct 2023 16:48:26 GMT
CMD ["python3"]
# Tue, 03 Oct 2023 04:37:55 GMT
LABEL org.opencontainers.image.title=Unit (python3.11)
# Tue, 03 Oct 2023 04:37:55 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Tue, 03 Oct 2023 04:37:55 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Tue, 03 Oct 2023 04:37:55 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Tue, 03 Oct 2023 04:37:55 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Tue, 03 Oct 2023 04:37:56 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 03 Oct 2023 04:37:56 GMT
LABEL org.opencontainers.image.version=1.31.0
# Tue, 03 Oct 2023 04:38:36 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure python --config=/usr/local/bin/python3-config     && make -j $NCPU python3-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure python --config=/usr/local/bin/python3-config     && make -j $NCPU python3-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Tue, 03 Oct 2023 04:38:36 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Tue, 03 Oct 2023 04:38:36 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Tue, 03 Oct 2023 04:38:36 GMT
STOPSIGNAL SIGTERM
# Tue, 03 Oct 2023 04:38:37 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 03 Oct 2023 04:38:37 GMT
EXPOSE 80
# Tue, 03 Oct 2023 04:38:37 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:31f5dc1f52c865588c43d8ec718f14d430e149b28f0b28232da825da7ae28f76`  
		Last Modified: Wed, 20 Sep 2023 02:47:53 GMT  
		Size: 53.7 MB (53704892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb60045eb75c62e890b95d28e4893132a6c7d61ec9979104ee4ff6e86c4badee`  
		Last Modified: Wed, 20 Sep 2023 09:33:11 GMT  
		Size: 15.7 MB (15746671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292737ab468ef80c6f78bdde4896157b8953d1e5556e1e526f40aeadcb547573`  
		Last Modified: Wed, 20 Sep 2023 09:33:26 GMT  
		Size: 54.7 MB (54676309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d93979d624211374be152eee1c99ed4ca9e6bae68694135fc440ab6c8fd2044`  
		Last Modified: Wed, 20 Sep 2023 09:33:51 GMT  
		Size: 189.8 MB (189778334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a9f8670f1b8c5bf3a5389568c9f40d95526c380daa5b707640ce7a9be9076c4`  
		Last Modified: Wed, 20 Sep 2023 21:58:21 GMT  
		Size: 6.4 MB (6405066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4ee3feee6bb07e1e690530f4073cefe52850fc7ce215c60cde9f743293dd97`  
		Last Modified: Tue, 03 Oct 2023 04:12:56 GMT  
		Size: 19.9 MB (19937158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4091e9efdd6b4028377199af2b8bac46c9f271309e560152e21888f5d7f4ad0b`  
		Last Modified: Tue, 03 Oct 2023 04:12:53 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306fc013432d7365870d985fbeb02a5ea64cd70a0ff047dae8f958b3fa1b944e`  
		Last Modified: Tue, 03 Oct 2023 04:12:54 GMT  
		Size: 3.1 MB (3109607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e94fb5ebc22b2c1377eb006509be69bc493b269685b3dac417cdfbbe99501a`  
		Last Modified: Tue, 03 Oct 2023 04:39:18 GMT  
		Size: 7.4 MB (7356865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1c327971a0e691baac3b8e16245c90d68517bdd5ebd62c8672c393b21007ab`  
		Last Modified: Tue, 03 Oct 2023 04:39:16 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36b452cc0eb4a32a12308190469a5a96a527d292337bf035d0bdd865341fa34`  
		Last Modified: Tue, 03 Oct 2023 04:39:17 GMT  
		Size: 1.5 KB (1468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `unit:python3`

```console
$ docker pull unit@sha256:97f7574d4ce36f8eca74f25555dce4835dfc479d033acb68e20d19dec141e112
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:python3` - linux; amd64

```console
$ docker pull unit@sha256:7e930385f350c30f67fb9d8af68e500c684c6a7037a887fb28e8e9bb17f21a63
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.2 MB (359180856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f539861a71c1bdb6090a4ad0d937ad8e88c23b4e00971e8aee44a140ca84439`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 04:55:51 GMT
ADD file:85db4f4c5016f51f7112a5d09cb7d4620f565a1379ae4b8a03c5ffc23886a876 in / 
# Wed, 20 Sep 2023 04:55:51 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:22:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:22:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:23:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 02 Oct 2023 16:48:26 GMT
ENV LANG=C.UTF-8
# Mon, 02 Oct 2023 16:48:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 02 Oct 2023 16:48:26 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_VERSION=3.11.6
# Mon, 02 Oct 2023 16:48:26 GMT
RUN set -eux; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		bin="$(readlink -ve /usr/local/bin/python3)"; 	dir="$(dirname "$bin")"; 	mkdir -p "/usr/share/gdb/auto-load/$dir"; 	cp -vL Tools/gdb/libpython.py "/usr/share/gdb/auto-load/$bin-gdb.py"; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		python3 --version # buildkit
# Mon, 02 Oct 2023 16:48:26 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_PIP_VERSION=23.2.1
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/9af82b715db434abb94a0a6f3569f43e72157346/public/get-pip.py
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_GET_PIP_SHA256=45a2bb8bf2bb5eff16fdd00faef6f29731831c7c59bd9fc2bf1f3bed511ff1fe
# Mon, 02 Oct 2023 16:48:26 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Mon, 02 Oct 2023 16:48:26 GMT
CMD ["python3"]
# Tue, 03 Oct 2023 04:27:32 GMT
LABEL org.opencontainers.image.title=Unit (python3.11)
# Tue, 03 Oct 2023 04:27:32 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Tue, 03 Oct 2023 04:27:32 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Tue, 03 Oct 2023 04:27:32 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Tue, 03 Oct 2023 04:27:32 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Tue, 03 Oct 2023 04:27:32 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 03 Oct 2023 04:27:33 GMT
LABEL org.opencontainers.image.version=1.31.0
# Tue, 03 Oct 2023 04:28:23 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure python --config=/usr/local/bin/python3-config     && make -j $NCPU python3-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure python --config=/usr/local/bin/python3-config     && make -j $NCPU python3-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Tue, 03 Oct 2023 04:28:23 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Tue, 03 Oct 2023 04:28:23 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Tue, 03 Oct 2023 04:28:24 GMT
STOPSIGNAL SIGTERM
# Tue, 03 Oct 2023 04:28:24 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 03 Oct 2023 04:28:24 GMT
EXPOSE 80
# Tue, 03 Oct 2023 04:28:24 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:ddf874abf16cc990e0fd75a154a34ca0a03ee310ad895a18fb62ae15bf4171fb`  
		Last Modified: Wed, 20 Sep 2023 05:00:41 GMT  
		Size: 55.1 MB (55056714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1459d3ab8b5e46ac1a0a00134fe2f7b693474eb6d75ace97ecbe811a6f5b0e`  
		Last Modified: Wed, 20 Sep 2023 09:31:06 GMT  
		Size: 15.8 MB (15760408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab00e7798a04602c3f6e2dc445a994d75e96c45533cd44701f58509982a8c5`  
		Last Modified: Wed, 20 Sep 2023 09:31:23 GMT  
		Size: 54.6 MB (54584790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7883a473306cf6632abe7e913e0f1a21ac2fed038a4116473b25738b8b88b294`  
		Last Modified: Wed, 20 Sep 2023 09:31:55 GMT  
		Size: 196.8 MB (196842512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ab175b762c07a73f43bc078229d225d45a4810a8f4e8cb19602122986eadb5`  
		Last Modified: Wed, 20 Sep 2023 12:17:10 GMT  
		Size: 6.3 MB (6291084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19164320e566edd82bea237a00344772e5cdaceb1c0581eab62ea66b8a812d5c`  
		Last Modified: Tue, 03 Oct 2023 03:58:29 GMT  
		Size: 20.1 MB (20053476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccfa8e20789038925a7a0ac61d49b8337c2ff7f1b923e8190271a936e206413e`  
		Last Modified: Tue, 03 Oct 2023 03:58:26 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a5bfb4de08e5dbf05e323300db82d3423385e2e4a87ff92c93574cfe940306`  
		Last Modified: Tue, 03 Oct 2023 03:58:26 GMT  
		Size: 3.1 MB (3109666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2853480534c9003652abee52b8564d53ec16ae60da13fdca042d57b323bab888`  
		Last Modified: Tue, 03 Oct 2023 04:29:10 GMT  
		Size: 7.5 MB (7479231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d411f454564bf8a14d13d91dcef8dec6c34ec244c7580c88c8a1d529f08b848`  
		Last Modified: Tue, 03 Oct 2023 04:29:08 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14417cd73e58663a678f0c5a0fce443306ffd56f455e0d42c0264ef51dfadc2a`  
		Last Modified: Tue, 03 Oct 2023 04:29:08 GMT  
		Size: 1.5 KB (1464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:python3` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:6fed15916314569b43402551b06ad9ecde8957e827a4628b195d31304271e3ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.7 MB (350717878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:705609da8fdf387160dd80f7413f642a4b06072f958b38bbd8c0137df5d6db1b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:20 GMT
ADD file:46dcdcde338d2c01fed5db3fac9041736d9305145d8fc2039dd5b3714d38ede8 in / 
# Wed, 20 Sep 2023 02:44:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:24:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:25:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:26:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 02 Oct 2023 16:48:26 GMT
ENV LANG=C.UTF-8
# Mon, 02 Oct 2023 16:48:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 02 Oct 2023 16:48:26 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_VERSION=3.11.6
# Mon, 02 Oct 2023 16:48:26 GMT
RUN set -eux; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		bin="$(readlink -ve /usr/local/bin/python3)"; 	dir="$(dirname "$bin")"; 	mkdir -p "/usr/share/gdb/auto-load/$dir"; 	cp -vL Tools/gdb/libpython.py "/usr/share/gdb/auto-load/$bin-gdb.py"; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		python3 --version # buildkit
# Mon, 02 Oct 2023 16:48:26 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_PIP_VERSION=23.2.1
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/9af82b715db434abb94a0a6f3569f43e72157346/public/get-pip.py
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_GET_PIP_SHA256=45a2bb8bf2bb5eff16fdd00faef6f29731831c7c59bd9fc2bf1f3bed511ff1fe
# Mon, 02 Oct 2023 16:48:26 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Mon, 02 Oct 2023 16:48:26 GMT
CMD ["python3"]
# Tue, 03 Oct 2023 04:37:55 GMT
LABEL org.opencontainers.image.title=Unit (python3.11)
# Tue, 03 Oct 2023 04:37:55 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Tue, 03 Oct 2023 04:37:55 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Tue, 03 Oct 2023 04:37:55 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Tue, 03 Oct 2023 04:37:55 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Tue, 03 Oct 2023 04:37:56 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 03 Oct 2023 04:37:56 GMT
LABEL org.opencontainers.image.version=1.31.0
# Tue, 03 Oct 2023 04:38:36 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure python --config=/usr/local/bin/python3-config     && make -j $NCPU python3-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure python --config=/usr/local/bin/python3-config     && make -j $NCPU python3-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Tue, 03 Oct 2023 04:38:36 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Tue, 03 Oct 2023 04:38:36 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Tue, 03 Oct 2023 04:38:36 GMT
STOPSIGNAL SIGTERM
# Tue, 03 Oct 2023 04:38:37 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 03 Oct 2023 04:38:37 GMT
EXPOSE 80
# Tue, 03 Oct 2023 04:38:37 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:31f5dc1f52c865588c43d8ec718f14d430e149b28f0b28232da825da7ae28f76`  
		Last Modified: Wed, 20 Sep 2023 02:47:53 GMT  
		Size: 53.7 MB (53704892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb60045eb75c62e890b95d28e4893132a6c7d61ec9979104ee4ff6e86c4badee`  
		Last Modified: Wed, 20 Sep 2023 09:33:11 GMT  
		Size: 15.7 MB (15746671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292737ab468ef80c6f78bdde4896157b8953d1e5556e1e526f40aeadcb547573`  
		Last Modified: Wed, 20 Sep 2023 09:33:26 GMT  
		Size: 54.7 MB (54676309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d93979d624211374be152eee1c99ed4ca9e6bae68694135fc440ab6c8fd2044`  
		Last Modified: Wed, 20 Sep 2023 09:33:51 GMT  
		Size: 189.8 MB (189778334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a9f8670f1b8c5bf3a5389568c9f40d95526c380daa5b707640ce7a9be9076c4`  
		Last Modified: Wed, 20 Sep 2023 21:58:21 GMT  
		Size: 6.4 MB (6405066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4ee3feee6bb07e1e690530f4073cefe52850fc7ce215c60cde9f743293dd97`  
		Last Modified: Tue, 03 Oct 2023 04:12:56 GMT  
		Size: 19.9 MB (19937158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4091e9efdd6b4028377199af2b8bac46c9f271309e560152e21888f5d7f4ad0b`  
		Last Modified: Tue, 03 Oct 2023 04:12:53 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306fc013432d7365870d985fbeb02a5ea64cd70a0ff047dae8f958b3fa1b944e`  
		Last Modified: Tue, 03 Oct 2023 04:12:54 GMT  
		Size: 3.1 MB (3109607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e94fb5ebc22b2c1377eb006509be69bc493b269685b3dac417cdfbbe99501a`  
		Last Modified: Tue, 03 Oct 2023 04:39:18 GMT  
		Size: 7.4 MB (7356865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1c327971a0e691baac3b8e16245c90d68517bdd5ebd62c8672c393b21007ab`  
		Last Modified: Tue, 03 Oct 2023 04:39:16 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36b452cc0eb4a32a12308190469a5a96a527d292337bf035d0bdd865341fa34`  
		Last Modified: Tue, 03 Oct 2023 04:39:17 GMT  
		Size: 1.5 KB (1468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `unit:python3.11`

```console
$ docker pull unit@sha256:97f7574d4ce36f8eca74f25555dce4835dfc479d033acb68e20d19dec141e112
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:python3.11` - linux; amd64

```console
$ docker pull unit@sha256:7e930385f350c30f67fb9d8af68e500c684c6a7037a887fb28e8e9bb17f21a63
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.2 MB (359180856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f539861a71c1bdb6090a4ad0d937ad8e88c23b4e00971e8aee44a140ca84439`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 04:55:51 GMT
ADD file:85db4f4c5016f51f7112a5d09cb7d4620f565a1379ae4b8a03c5ffc23886a876 in / 
# Wed, 20 Sep 2023 04:55:51 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:22:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:22:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:23:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 02 Oct 2023 16:48:26 GMT
ENV LANG=C.UTF-8
# Mon, 02 Oct 2023 16:48:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 02 Oct 2023 16:48:26 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_VERSION=3.11.6
# Mon, 02 Oct 2023 16:48:26 GMT
RUN set -eux; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		bin="$(readlink -ve /usr/local/bin/python3)"; 	dir="$(dirname "$bin")"; 	mkdir -p "/usr/share/gdb/auto-load/$dir"; 	cp -vL Tools/gdb/libpython.py "/usr/share/gdb/auto-load/$bin-gdb.py"; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		python3 --version # buildkit
# Mon, 02 Oct 2023 16:48:26 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_PIP_VERSION=23.2.1
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/9af82b715db434abb94a0a6f3569f43e72157346/public/get-pip.py
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_GET_PIP_SHA256=45a2bb8bf2bb5eff16fdd00faef6f29731831c7c59bd9fc2bf1f3bed511ff1fe
# Mon, 02 Oct 2023 16:48:26 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Mon, 02 Oct 2023 16:48:26 GMT
CMD ["python3"]
# Tue, 03 Oct 2023 04:27:32 GMT
LABEL org.opencontainers.image.title=Unit (python3.11)
# Tue, 03 Oct 2023 04:27:32 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Tue, 03 Oct 2023 04:27:32 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Tue, 03 Oct 2023 04:27:32 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Tue, 03 Oct 2023 04:27:32 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Tue, 03 Oct 2023 04:27:32 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 03 Oct 2023 04:27:33 GMT
LABEL org.opencontainers.image.version=1.31.0
# Tue, 03 Oct 2023 04:28:23 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure python --config=/usr/local/bin/python3-config     && make -j $NCPU python3-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure python --config=/usr/local/bin/python3-config     && make -j $NCPU python3-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Tue, 03 Oct 2023 04:28:23 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Tue, 03 Oct 2023 04:28:23 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Tue, 03 Oct 2023 04:28:24 GMT
STOPSIGNAL SIGTERM
# Tue, 03 Oct 2023 04:28:24 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 03 Oct 2023 04:28:24 GMT
EXPOSE 80
# Tue, 03 Oct 2023 04:28:24 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:ddf874abf16cc990e0fd75a154a34ca0a03ee310ad895a18fb62ae15bf4171fb`  
		Last Modified: Wed, 20 Sep 2023 05:00:41 GMT  
		Size: 55.1 MB (55056714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1459d3ab8b5e46ac1a0a00134fe2f7b693474eb6d75ace97ecbe811a6f5b0e`  
		Last Modified: Wed, 20 Sep 2023 09:31:06 GMT  
		Size: 15.8 MB (15760408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab00e7798a04602c3f6e2dc445a994d75e96c45533cd44701f58509982a8c5`  
		Last Modified: Wed, 20 Sep 2023 09:31:23 GMT  
		Size: 54.6 MB (54584790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7883a473306cf6632abe7e913e0f1a21ac2fed038a4116473b25738b8b88b294`  
		Last Modified: Wed, 20 Sep 2023 09:31:55 GMT  
		Size: 196.8 MB (196842512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ab175b762c07a73f43bc078229d225d45a4810a8f4e8cb19602122986eadb5`  
		Last Modified: Wed, 20 Sep 2023 12:17:10 GMT  
		Size: 6.3 MB (6291084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19164320e566edd82bea237a00344772e5cdaceb1c0581eab62ea66b8a812d5c`  
		Last Modified: Tue, 03 Oct 2023 03:58:29 GMT  
		Size: 20.1 MB (20053476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccfa8e20789038925a7a0ac61d49b8337c2ff7f1b923e8190271a936e206413e`  
		Last Modified: Tue, 03 Oct 2023 03:58:26 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a5bfb4de08e5dbf05e323300db82d3423385e2e4a87ff92c93574cfe940306`  
		Last Modified: Tue, 03 Oct 2023 03:58:26 GMT  
		Size: 3.1 MB (3109666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2853480534c9003652abee52b8564d53ec16ae60da13fdca042d57b323bab888`  
		Last Modified: Tue, 03 Oct 2023 04:29:10 GMT  
		Size: 7.5 MB (7479231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d411f454564bf8a14d13d91dcef8dec6c34ec244c7580c88c8a1d529f08b848`  
		Last Modified: Tue, 03 Oct 2023 04:29:08 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14417cd73e58663a678f0c5a0fce443306ffd56f455e0d42c0264ef51dfadc2a`  
		Last Modified: Tue, 03 Oct 2023 04:29:08 GMT  
		Size: 1.5 KB (1464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:python3.11` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:6fed15916314569b43402551b06ad9ecde8957e827a4628b195d31304271e3ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.7 MB (350717878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:705609da8fdf387160dd80f7413f642a4b06072f958b38bbd8c0137df5d6db1b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:20 GMT
ADD file:46dcdcde338d2c01fed5db3fac9041736d9305145d8fc2039dd5b3714d38ede8 in / 
# Wed, 20 Sep 2023 02:44:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:24:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:25:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:26:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 02 Oct 2023 16:48:26 GMT
ENV LANG=C.UTF-8
# Mon, 02 Oct 2023 16:48:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 02 Oct 2023 16:48:26 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_VERSION=3.11.6
# Mon, 02 Oct 2023 16:48:26 GMT
RUN set -eux; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		bin="$(readlink -ve /usr/local/bin/python3)"; 	dir="$(dirname "$bin")"; 	mkdir -p "/usr/share/gdb/auto-load/$dir"; 	cp -vL Tools/gdb/libpython.py "/usr/share/gdb/auto-load/$bin-gdb.py"; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		python3 --version # buildkit
# Mon, 02 Oct 2023 16:48:26 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_PIP_VERSION=23.2.1
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/9af82b715db434abb94a0a6f3569f43e72157346/public/get-pip.py
# Mon, 02 Oct 2023 16:48:26 GMT
ENV PYTHON_GET_PIP_SHA256=45a2bb8bf2bb5eff16fdd00faef6f29731831c7c59bd9fc2bf1f3bed511ff1fe
# Mon, 02 Oct 2023 16:48:26 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Mon, 02 Oct 2023 16:48:26 GMT
CMD ["python3"]
# Tue, 03 Oct 2023 04:37:55 GMT
LABEL org.opencontainers.image.title=Unit (python3.11)
# Tue, 03 Oct 2023 04:37:55 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Tue, 03 Oct 2023 04:37:55 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Tue, 03 Oct 2023 04:37:55 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Tue, 03 Oct 2023 04:37:55 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Tue, 03 Oct 2023 04:37:56 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 03 Oct 2023 04:37:56 GMT
LABEL org.opencontainers.image.version=1.31.0
# Tue, 03 Oct 2023 04:38:36 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure python --config=/usr/local/bin/python3-config     && make -j $NCPU python3-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure python --config=/usr/local/bin/python3-config     && make -j $NCPU python3-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Tue, 03 Oct 2023 04:38:36 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Tue, 03 Oct 2023 04:38:36 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Tue, 03 Oct 2023 04:38:36 GMT
STOPSIGNAL SIGTERM
# Tue, 03 Oct 2023 04:38:37 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 03 Oct 2023 04:38:37 GMT
EXPOSE 80
# Tue, 03 Oct 2023 04:38:37 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:31f5dc1f52c865588c43d8ec718f14d430e149b28f0b28232da825da7ae28f76`  
		Last Modified: Wed, 20 Sep 2023 02:47:53 GMT  
		Size: 53.7 MB (53704892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb60045eb75c62e890b95d28e4893132a6c7d61ec9979104ee4ff6e86c4badee`  
		Last Modified: Wed, 20 Sep 2023 09:33:11 GMT  
		Size: 15.7 MB (15746671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292737ab468ef80c6f78bdde4896157b8953d1e5556e1e526f40aeadcb547573`  
		Last Modified: Wed, 20 Sep 2023 09:33:26 GMT  
		Size: 54.7 MB (54676309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d93979d624211374be152eee1c99ed4ca9e6bae68694135fc440ab6c8fd2044`  
		Last Modified: Wed, 20 Sep 2023 09:33:51 GMT  
		Size: 189.8 MB (189778334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a9f8670f1b8c5bf3a5389568c9f40d95526c380daa5b707640ce7a9be9076c4`  
		Last Modified: Wed, 20 Sep 2023 21:58:21 GMT  
		Size: 6.4 MB (6405066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4ee3feee6bb07e1e690530f4073cefe52850fc7ce215c60cde9f743293dd97`  
		Last Modified: Tue, 03 Oct 2023 04:12:56 GMT  
		Size: 19.9 MB (19937158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4091e9efdd6b4028377199af2b8bac46c9f271309e560152e21888f5d7f4ad0b`  
		Last Modified: Tue, 03 Oct 2023 04:12:53 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306fc013432d7365870d985fbeb02a5ea64cd70a0ff047dae8f958b3fa1b944e`  
		Last Modified: Tue, 03 Oct 2023 04:12:54 GMT  
		Size: 3.1 MB (3109607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e94fb5ebc22b2c1377eb006509be69bc493b269685b3dac417cdfbbe99501a`  
		Last Modified: Tue, 03 Oct 2023 04:39:18 GMT  
		Size: 7.4 MB (7356865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1c327971a0e691baac3b8e16245c90d68517bdd5ebd62c8672c393b21007ab`  
		Last Modified: Tue, 03 Oct 2023 04:39:16 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36b452cc0eb4a32a12308190469a5a96a527d292337bf035d0bdd865341fa34`  
		Last Modified: Tue, 03 Oct 2023 04:39:17 GMT  
		Size: 1.5 KB (1468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `unit:ruby`

```console
$ docker pull unit@sha256:a5e6024510f124beb927b8856bbb21d3b41fc416478cf5a804c07f113e842f60
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:ruby` - linux; amd64

```console
$ docker pull unit@sha256:956602c398b9f70c86add7421abf3c9cc2d2d2a5cff956bb5e88e8fd7302d344
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **364.3 MB (364275696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3213b761cda6d5ab61d82cffa6ccb864a779fd8d19fe7dd1c5e2b75e19fb987d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 04:55:51 GMT
ADD file:85db4f4c5016f51f7112a5d09cb7d4620f565a1379ae4b8a03c5ffc23886a876 in / 
# Wed, 20 Sep 2023 04:55:51 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:22:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:22:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:23:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 04:11:30 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 21 Sep 2023 04:11:30 GMT
ENV LANG=C.UTF-8
# Thu, 21 Sep 2023 04:18:56 GMT
ENV RUBY_MAJOR=3.2
# Thu, 21 Sep 2023 04:18:56 GMT
ENV RUBY_VERSION=3.2.2
# Thu, 21 Sep 2023 04:18:56 GMT
ENV RUBY_DOWNLOAD_SHA256=4b352d0f7ec384e332e3e44cdbfdcd5ff2d594af3c8296b5636c710975149e23
# Thu, 21 Sep 2023 04:21:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		rustArch=; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		'amd64') rustArch='x86_64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/x86_64-unknown-linux-gnu/rustup-init'; rustupSha256='5cc9ffd1026e82e7fb2eec2121ad71f4b0f044e88bca39207b3f6b769aaa799c' ;; 		'arm64') rustArch='aarch64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/aarch64-unknown-linux-gnu/rustup-init'; rustupSha256='e189948e396d47254103a49c987e7fb0e5dd8e34b200aa4481ecc4b8e41fb929' ;; 	esac; 		if [ -n "$rustArch" ]; then 		mkdir -p /tmp/rust; 				wget -O /tmp/rust/rustup-init "$rustupUrl"; 		echo "$rustupSha256 */tmp/rust/rustup-init" | sha256sum --check --strict; 		chmod +x /tmp/rust/rustup-init; 				export RUSTUP_HOME='/tmp/rust/rustup' CARGO_HOME='/tmp/rust/cargo'; 		export PATH="$CARGO_HOME/bin:$PATH"; 		/tmp/rust/rustup-init -y --no-modify-path --profile minimal --default-toolchain '1.66.0' --default-host "$rustArch"; 				rustc --version; 		cargo --version; 	fi; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 		${rustArch:+--enable-yjit} 	; 	make -j "$(nproc)"; 	make install; 		rm -rf /tmp/rust; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 21 Sep 2023 04:21:13 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 21 Sep 2023 04:21:13 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 21 Sep 2023 04:21:13 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 21 Sep 2023 04:21:13 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 21 Sep 2023 04:21:14 GMT
CMD ["irb"]
# Thu, 21 Sep 2023 09:01:40 GMT
LABEL org.opencontainers.image.title=Unit (ruby3.2)
# Thu, 21 Sep 2023 09:01:40 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Thu, 21 Sep 2023 09:01:40 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Thu, 21 Sep 2023 09:01:40 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Thu, 21 Sep 2023 09:01:40 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Thu, 21 Sep 2023 09:01:41 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Thu, 21 Sep 2023 09:01:41 GMT
LABEL org.opencontainers.image.version=1.31.0
# Thu, 21 Sep 2023 09:02:33 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure ruby     && make -j $NCPU ruby-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure ruby     && make -j $NCPU ruby-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && gem install rack && rm -rf /root/.local     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Thu, 21 Sep 2023 09:02:33 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Thu, 21 Sep 2023 09:02:33 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Thu, 21 Sep 2023 09:02:33 GMT
STOPSIGNAL SIGTERM
# Thu, 21 Sep 2023 09:02:33 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 21 Sep 2023 09:02:34 GMT
EXPOSE 80
# Thu, 21 Sep 2023 09:02:34 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:ddf874abf16cc990e0fd75a154a34ca0a03ee310ad895a18fb62ae15bf4171fb`  
		Last Modified: Wed, 20 Sep 2023 05:00:41 GMT  
		Size: 55.1 MB (55056714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1459d3ab8b5e46ac1a0a00134fe2f7b693474eb6d75ace97ecbe811a6f5b0e`  
		Last Modified: Wed, 20 Sep 2023 09:31:06 GMT  
		Size: 15.8 MB (15760408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab00e7798a04602c3f6e2dc445a994d75e96c45533cd44701f58509982a8c5`  
		Last Modified: Wed, 20 Sep 2023 09:31:23 GMT  
		Size: 54.6 MB (54584790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7883a473306cf6632abe7e913e0f1a21ac2fed038a4116473b25738b8b88b294`  
		Last Modified: Wed, 20 Sep 2023 09:31:55 GMT  
		Size: 196.8 MB (196842512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fdcd138618aab34068d5f25a76b9f52fd31968b0ac18bb7d07712e2dfb218da`  
		Last Modified: Thu, 21 Sep 2023 04:31:31 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a1c513a65f8aa3521e033b2594828b7458e09a64b409ae0c845fa78f54dbee`  
		Last Modified: Thu, 21 Sep 2023 04:32:15 GMT  
		Size: 34.6 MB (34555434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef736a5e310922df2e0ec8fea9b8cb6e82f6e05b6728246464e80cbd3323463`  
		Last Modified: Thu, 21 Sep 2023 04:32:12 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852f8560c08590962b1223b1b4098e276106212ed51b79cce0f8c8cc3c7ecf03`  
		Last Modified: Thu, 21 Sep 2023 09:03:59 GMT  
		Size: 7.5 MB (7472725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:355dd321857fb6ccef83d972ba26481615db92cda9272569c448f690bd3caaba`  
		Last Modified: Thu, 21 Sep 2023 09:03:57 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539417e59f1725542c24856f19c2f2a3348df4e315ef3336ff577fa9e163a913`  
		Last Modified: Thu, 21 Sep 2023 09:03:57 GMT  
		Size: 1.5 KB (1464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:ruby` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:dffefd84552257cf59dee4bbe3e0bb6c1d278ea4149b15d4e9839dddd4e1dd05
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.7 MB (355686533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d01d684dd22e47a20187d814ce3077e56cffccc53f1a3681e112e1e6dd9c68e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:20 GMT
ADD file:46dcdcde338d2c01fed5db3fac9041736d9305145d8fc2039dd5b3714d38ede8 in / 
# Wed, 20 Sep 2023 02:44:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:24:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:25:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:26:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 17:00:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 20 Sep 2023 17:00:09 GMT
ENV LANG=C.UTF-8
# Wed, 20 Sep 2023 17:12:43 GMT
ENV RUBY_MAJOR=3.2
# Wed, 20 Sep 2023 17:12:43 GMT
ENV RUBY_VERSION=3.2.2
# Wed, 20 Sep 2023 17:12:43 GMT
ENV RUBY_DOWNLOAD_SHA256=4b352d0f7ec384e332e3e44cdbfdcd5ff2d594af3c8296b5636c710975149e23
# Wed, 20 Sep 2023 17:14:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		rustArch=; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		'amd64') rustArch='x86_64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/x86_64-unknown-linux-gnu/rustup-init'; rustupSha256='5cc9ffd1026e82e7fb2eec2121ad71f4b0f044e88bca39207b3f6b769aaa799c' ;; 		'arm64') rustArch='aarch64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/aarch64-unknown-linux-gnu/rustup-init'; rustupSha256='e189948e396d47254103a49c987e7fb0e5dd8e34b200aa4481ecc4b8e41fb929' ;; 	esac; 		if [ -n "$rustArch" ]; then 		mkdir -p /tmp/rust; 				wget -O /tmp/rust/rustup-init "$rustupUrl"; 		echo "$rustupSha256 */tmp/rust/rustup-init" | sha256sum --check --strict; 		chmod +x /tmp/rust/rustup-init; 				export RUSTUP_HOME='/tmp/rust/rustup' CARGO_HOME='/tmp/rust/cargo'; 		export PATH="$CARGO_HOME/bin:$PATH"; 		/tmp/rust/rustup-init -y --no-modify-path --profile minimal --default-toolchain '1.66.0' --default-host "$rustArch"; 				rustc --version; 		cargo --version; 	fi; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 		${rustArch:+--enable-yjit} 	; 	make -j "$(nproc)"; 	make install; 		rm -rf /tmp/rust; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 20 Sep 2023 17:14:28 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 20 Sep 2023 17:14:28 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 20 Sep 2023 17:14:28 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Sep 2023 17:14:28 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Wed, 20 Sep 2023 17:14:29 GMT
CMD ["irb"]
# Thu, 21 Sep 2023 03:27:09 GMT
LABEL org.opencontainers.image.title=Unit (ruby3.2)
# Thu, 21 Sep 2023 03:27:09 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Thu, 21 Sep 2023 03:27:09 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Thu, 21 Sep 2023 03:27:09 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Thu, 21 Sep 2023 03:27:09 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Thu, 21 Sep 2023 03:27:09 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Thu, 21 Sep 2023 03:27:10 GMT
LABEL org.opencontainers.image.version=1.31.0
# Thu, 21 Sep 2023 03:27:51 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure ruby     && make -j $NCPU ruby-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure ruby     && make -j $NCPU ruby-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && gem install rack && rm -rf /root/.local     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Thu, 21 Sep 2023 03:27:51 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Thu, 21 Sep 2023 03:27:51 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Thu, 21 Sep 2023 03:27:51 GMT
STOPSIGNAL SIGTERM
# Thu, 21 Sep 2023 03:27:51 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 21 Sep 2023 03:27:51 GMT
EXPOSE 80
# Thu, 21 Sep 2023 03:27:51 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:31f5dc1f52c865588c43d8ec718f14d430e149b28f0b28232da825da7ae28f76`  
		Last Modified: Wed, 20 Sep 2023 02:47:53 GMT  
		Size: 53.7 MB (53704892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb60045eb75c62e890b95d28e4893132a6c7d61ec9979104ee4ff6e86c4badee`  
		Last Modified: Wed, 20 Sep 2023 09:33:11 GMT  
		Size: 15.7 MB (15746671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292737ab468ef80c6f78bdde4896157b8953d1e5556e1e526f40aeadcb547573`  
		Last Modified: Wed, 20 Sep 2023 09:33:26 GMT  
		Size: 54.7 MB (54676309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d93979d624211374be152eee1c99ed4ca9e6bae68694135fc440ab6c8fd2044`  
		Last Modified: Wed, 20 Sep 2023 09:33:51 GMT  
		Size: 189.8 MB (189778334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b301519822ecf9e91a1d73928dcd311c4bca39d7dc3c8312271a3a87192b6fad`  
		Last Modified: Wed, 20 Sep 2023 17:32:40 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83bd254efa556fb8118a65fd122dfaebb9beb925b07e4bce5dab0753adfe612b`  
		Last Modified: Wed, 20 Sep 2023 17:33:59 GMT  
		Size: 34.4 MB (34432616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf0bf0364fef8b7d14832a31609b05b197fc4cd485098cba635e2dcc48c3a18`  
		Last Modified: Wed, 20 Sep 2023 17:33:56 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddcc516d1030a5cfc66d59f54ada76bc9df6bbc565d4b0e7d2f5f0b7dfcdc755`  
		Last Modified: Thu, 21 Sep 2023 03:29:08 GMT  
		Size: 7.3 MB (7344596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3698a78d8a3fbcff7cc1793bf3bae553dfb607bc4135436e5699d758d6b3b7`  
		Last Modified: Thu, 21 Sep 2023 03:29:07 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7a2e346b9c5a6b73c465209726bfa46af845b73807df32c3a5ac350195ab35`  
		Last Modified: Thu, 21 Sep 2023 03:29:07 GMT  
		Size: 1.5 KB (1469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `unit:ruby3`

```console
$ docker pull unit@sha256:a5e6024510f124beb927b8856bbb21d3b41fc416478cf5a804c07f113e842f60
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:ruby3` - linux; amd64

```console
$ docker pull unit@sha256:956602c398b9f70c86add7421abf3c9cc2d2d2a5cff956bb5e88e8fd7302d344
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **364.3 MB (364275696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3213b761cda6d5ab61d82cffa6ccb864a779fd8d19fe7dd1c5e2b75e19fb987d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 04:55:51 GMT
ADD file:85db4f4c5016f51f7112a5d09cb7d4620f565a1379ae4b8a03c5ffc23886a876 in / 
# Wed, 20 Sep 2023 04:55:51 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:22:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:22:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:23:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 04:11:30 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 21 Sep 2023 04:11:30 GMT
ENV LANG=C.UTF-8
# Thu, 21 Sep 2023 04:18:56 GMT
ENV RUBY_MAJOR=3.2
# Thu, 21 Sep 2023 04:18:56 GMT
ENV RUBY_VERSION=3.2.2
# Thu, 21 Sep 2023 04:18:56 GMT
ENV RUBY_DOWNLOAD_SHA256=4b352d0f7ec384e332e3e44cdbfdcd5ff2d594af3c8296b5636c710975149e23
# Thu, 21 Sep 2023 04:21:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		rustArch=; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		'amd64') rustArch='x86_64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/x86_64-unknown-linux-gnu/rustup-init'; rustupSha256='5cc9ffd1026e82e7fb2eec2121ad71f4b0f044e88bca39207b3f6b769aaa799c' ;; 		'arm64') rustArch='aarch64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/aarch64-unknown-linux-gnu/rustup-init'; rustupSha256='e189948e396d47254103a49c987e7fb0e5dd8e34b200aa4481ecc4b8e41fb929' ;; 	esac; 		if [ -n "$rustArch" ]; then 		mkdir -p /tmp/rust; 				wget -O /tmp/rust/rustup-init "$rustupUrl"; 		echo "$rustupSha256 */tmp/rust/rustup-init" | sha256sum --check --strict; 		chmod +x /tmp/rust/rustup-init; 				export RUSTUP_HOME='/tmp/rust/rustup' CARGO_HOME='/tmp/rust/cargo'; 		export PATH="$CARGO_HOME/bin:$PATH"; 		/tmp/rust/rustup-init -y --no-modify-path --profile minimal --default-toolchain '1.66.0' --default-host "$rustArch"; 				rustc --version; 		cargo --version; 	fi; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 		${rustArch:+--enable-yjit} 	; 	make -j "$(nproc)"; 	make install; 		rm -rf /tmp/rust; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 21 Sep 2023 04:21:13 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 21 Sep 2023 04:21:13 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 21 Sep 2023 04:21:13 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 21 Sep 2023 04:21:13 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 21 Sep 2023 04:21:14 GMT
CMD ["irb"]
# Thu, 21 Sep 2023 09:01:40 GMT
LABEL org.opencontainers.image.title=Unit (ruby3.2)
# Thu, 21 Sep 2023 09:01:40 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Thu, 21 Sep 2023 09:01:40 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Thu, 21 Sep 2023 09:01:40 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Thu, 21 Sep 2023 09:01:40 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Thu, 21 Sep 2023 09:01:41 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Thu, 21 Sep 2023 09:01:41 GMT
LABEL org.opencontainers.image.version=1.31.0
# Thu, 21 Sep 2023 09:02:33 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure ruby     && make -j $NCPU ruby-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure ruby     && make -j $NCPU ruby-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && gem install rack && rm -rf /root/.local     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Thu, 21 Sep 2023 09:02:33 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Thu, 21 Sep 2023 09:02:33 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Thu, 21 Sep 2023 09:02:33 GMT
STOPSIGNAL SIGTERM
# Thu, 21 Sep 2023 09:02:33 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 21 Sep 2023 09:02:34 GMT
EXPOSE 80
# Thu, 21 Sep 2023 09:02:34 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:ddf874abf16cc990e0fd75a154a34ca0a03ee310ad895a18fb62ae15bf4171fb`  
		Last Modified: Wed, 20 Sep 2023 05:00:41 GMT  
		Size: 55.1 MB (55056714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1459d3ab8b5e46ac1a0a00134fe2f7b693474eb6d75ace97ecbe811a6f5b0e`  
		Last Modified: Wed, 20 Sep 2023 09:31:06 GMT  
		Size: 15.8 MB (15760408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab00e7798a04602c3f6e2dc445a994d75e96c45533cd44701f58509982a8c5`  
		Last Modified: Wed, 20 Sep 2023 09:31:23 GMT  
		Size: 54.6 MB (54584790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7883a473306cf6632abe7e913e0f1a21ac2fed038a4116473b25738b8b88b294`  
		Last Modified: Wed, 20 Sep 2023 09:31:55 GMT  
		Size: 196.8 MB (196842512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fdcd138618aab34068d5f25a76b9f52fd31968b0ac18bb7d07712e2dfb218da`  
		Last Modified: Thu, 21 Sep 2023 04:31:31 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a1c513a65f8aa3521e033b2594828b7458e09a64b409ae0c845fa78f54dbee`  
		Last Modified: Thu, 21 Sep 2023 04:32:15 GMT  
		Size: 34.6 MB (34555434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef736a5e310922df2e0ec8fea9b8cb6e82f6e05b6728246464e80cbd3323463`  
		Last Modified: Thu, 21 Sep 2023 04:32:12 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852f8560c08590962b1223b1b4098e276106212ed51b79cce0f8c8cc3c7ecf03`  
		Last Modified: Thu, 21 Sep 2023 09:03:59 GMT  
		Size: 7.5 MB (7472725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:355dd321857fb6ccef83d972ba26481615db92cda9272569c448f690bd3caaba`  
		Last Modified: Thu, 21 Sep 2023 09:03:57 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539417e59f1725542c24856f19c2f2a3348df4e315ef3336ff577fa9e163a913`  
		Last Modified: Thu, 21 Sep 2023 09:03:57 GMT  
		Size: 1.5 KB (1464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:ruby3` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:dffefd84552257cf59dee4bbe3e0bb6c1d278ea4149b15d4e9839dddd4e1dd05
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.7 MB (355686533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d01d684dd22e47a20187d814ce3077e56cffccc53f1a3681e112e1e6dd9c68e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:20 GMT
ADD file:46dcdcde338d2c01fed5db3fac9041736d9305145d8fc2039dd5b3714d38ede8 in / 
# Wed, 20 Sep 2023 02:44:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:24:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:25:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:26:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 17:00:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 20 Sep 2023 17:00:09 GMT
ENV LANG=C.UTF-8
# Wed, 20 Sep 2023 17:12:43 GMT
ENV RUBY_MAJOR=3.2
# Wed, 20 Sep 2023 17:12:43 GMT
ENV RUBY_VERSION=3.2.2
# Wed, 20 Sep 2023 17:12:43 GMT
ENV RUBY_DOWNLOAD_SHA256=4b352d0f7ec384e332e3e44cdbfdcd5ff2d594af3c8296b5636c710975149e23
# Wed, 20 Sep 2023 17:14:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		rustArch=; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		'amd64') rustArch='x86_64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/x86_64-unknown-linux-gnu/rustup-init'; rustupSha256='5cc9ffd1026e82e7fb2eec2121ad71f4b0f044e88bca39207b3f6b769aaa799c' ;; 		'arm64') rustArch='aarch64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/aarch64-unknown-linux-gnu/rustup-init'; rustupSha256='e189948e396d47254103a49c987e7fb0e5dd8e34b200aa4481ecc4b8e41fb929' ;; 	esac; 		if [ -n "$rustArch" ]; then 		mkdir -p /tmp/rust; 				wget -O /tmp/rust/rustup-init "$rustupUrl"; 		echo "$rustupSha256 */tmp/rust/rustup-init" | sha256sum --check --strict; 		chmod +x /tmp/rust/rustup-init; 				export RUSTUP_HOME='/tmp/rust/rustup' CARGO_HOME='/tmp/rust/cargo'; 		export PATH="$CARGO_HOME/bin:$PATH"; 		/tmp/rust/rustup-init -y --no-modify-path --profile minimal --default-toolchain '1.66.0' --default-host "$rustArch"; 				rustc --version; 		cargo --version; 	fi; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 		${rustArch:+--enable-yjit} 	; 	make -j "$(nproc)"; 	make install; 		rm -rf /tmp/rust; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 20 Sep 2023 17:14:28 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 20 Sep 2023 17:14:28 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 20 Sep 2023 17:14:28 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Sep 2023 17:14:28 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Wed, 20 Sep 2023 17:14:29 GMT
CMD ["irb"]
# Thu, 21 Sep 2023 03:27:09 GMT
LABEL org.opencontainers.image.title=Unit (ruby3.2)
# Thu, 21 Sep 2023 03:27:09 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Thu, 21 Sep 2023 03:27:09 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Thu, 21 Sep 2023 03:27:09 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Thu, 21 Sep 2023 03:27:09 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Thu, 21 Sep 2023 03:27:09 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Thu, 21 Sep 2023 03:27:10 GMT
LABEL org.opencontainers.image.version=1.31.0
# Thu, 21 Sep 2023 03:27:51 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure ruby     && make -j $NCPU ruby-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure ruby     && make -j $NCPU ruby-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && gem install rack && rm -rf /root/.local     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Thu, 21 Sep 2023 03:27:51 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Thu, 21 Sep 2023 03:27:51 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Thu, 21 Sep 2023 03:27:51 GMT
STOPSIGNAL SIGTERM
# Thu, 21 Sep 2023 03:27:51 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 21 Sep 2023 03:27:51 GMT
EXPOSE 80
# Thu, 21 Sep 2023 03:27:51 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:31f5dc1f52c865588c43d8ec718f14d430e149b28f0b28232da825da7ae28f76`  
		Last Modified: Wed, 20 Sep 2023 02:47:53 GMT  
		Size: 53.7 MB (53704892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb60045eb75c62e890b95d28e4893132a6c7d61ec9979104ee4ff6e86c4badee`  
		Last Modified: Wed, 20 Sep 2023 09:33:11 GMT  
		Size: 15.7 MB (15746671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292737ab468ef80c6f78bdde4896157b8953d1e5556e1e526f40aeadcb547573`  
		Last Modified: Wed, 20 Sep 2023 09:33:26 GMT  
		Size: 54.7 MB (54676309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d93979d624211374be152eee1c99ed4ca9e6bae68694135fc440ab6c8fd2044`  
		Last Modified: Wed, 20 Sep 2023 09:33:51 GMT  
		Size: 189.8 MB (189778334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b301519822ecf9e91a1d73928dcd311c4bca39d7dc3c8312271a3a87192b6fad`  
		Last Modified: Wed, 20 Sep 2023 17:32:40 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83bd254efa556fb8118a65fd122dfaebb9beb925b07e4bce5dab0753adfe612b`  
		Last Modified: Wed, 20 Sep 2023 17:33:59 GMT  
		Size: 34.4 MB (34432616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf0bf0364fef8b7d14832a31609b05b197fc4cd485098cba635e2dcc48c3a18`  
		Last Modified: Wed, 20 Sep 2023 17:33:56 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddcc516d1030a5cfc66d59f54ada76bc9df6bbc565d4b0e7d2f5f0b7dfcdc755`  
		Last Modified: Thu, 21 Sep 2023 03:29:08 GMT  
		Size: 7.3 MB (7344596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3698a78d8a3fbcff7cc1793bf3bae553dfb607bc4135436e5699d758d6b3b7`  
		Last Modified: Thu, 21 Sep 2023 03:29:07 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7a2e346b9c5a6b73c465209726bfa46af845b73807df32c3a5ac350195ab35`  
		Last Modified: Thu, 21 Sep 2023 03:29:07 GMT  
		Size: 1.5 KB (1469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `unit:ruby3.2`

```console
$ docker pull unit@sha256:a5e6024510f124beb927b8856bbb21d3b41fc416478cf5a804c07f113e842f60
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:ruby3.2` - linux; amd64

```console
$ docker pull unit@sha256:956602c398b9f70c86add7421abf3c9cc2d2d2a5cff956bb5e88e8fd7302d344
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **364.3 MB (364275696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3213b761cda6d5ab61d82cffa6ccb864a779fd8d19fe7dd1c5e2b75e19fb987d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 04:55:51 GMT
ADD file:85db4f4c5016f51f7112a5d09cb7d4620f565a1379ae4b8a03c5ffc23886a876 in / 
# Wed, 20 Sep 2023 04:55:51 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:22:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:22:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:23:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 04:11:30 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 21 Sep 2023 04:11:30 GMT
ENV LANG=C.UTF-8
# Thu, 21 Sep 2023 04:18:56 GMT
ENV RUBY_MAJOR=3.2
# Thu, 21 Sep 2023 04:18:56 GMT
ENV RUBY_VERSION=3.2.2
# Thu, 21 Sep 2023 04:18:56 GMT
ENV RUBY_DOWNLOAD_SHA256=4b352d0f7ec384e332e3e44cdbfdcd5ff2d594af3c8296b5636c710975149e23
# Thu, 21 Sep 2023 04:21:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		rustArch=; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		'amd64') rustArch='x86_64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/x86_64-unknown-linux-gnu/rustup-init'; rustupSha256='5cc9ffd1026e82e7fb2eec2121ad71f4b0f044e88bca39207b3f6b769aaa799c' ;; 		'arm64') rustArch='aarch64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/aarch64-unknown-linux-gnu/rustup-init'; rustupSha256='e189948e396d47254103a49c987e7fb0e5dd8e34b200aa4481ecc4b8e41fb929' ;; 	esac; 		if [ -n "$rustArch" ]; then 		mkdir -p /tmp/rust; 				wget -O /tmp/rust/rustup-init "$rustupUrl"; 		echo "$rustupSha256 */tmp/rust/rustup-init" | sha256sum --check --strict; 		chmod +x /tmp/rust/rustup-init; 				export RUSTUP_HOME='/tmp/rust/rustup' CARGO_HOME='/tmp/rust/cargo'; 		export PATH="$CARGO_HOME/bin:$PATH"; 		/tmp/rust/rustup-init -y --no-modify-path --profile minimal --default-toolchain '1.66.0' --default-host "$rustArch"; 				rustc --version; 		cargo --version; 	fi; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 		${rustArch:+--enable-yjit} 	; 	make -j "$(nproc)"; 	make install; 		rm -rf /tmp/rust; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 21 Sep 2023 04:21:13 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 21 Sep 2023 04:21:13 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 21 Sep 2023 04:21:13 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 21 Sep 2023 04:21:13 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 21 Sep 2023 04:21:14 GMT
CMD ["irb"]
# Thu, 21 Sep 2023 09:01:40 GMT
LABEL org.opencontainers.image.title=Unit (ruby3.2)
# Thu, 21 Sep 2023 09:01:40 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Thu, 21 Sep 2023 09:01:40 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Thu, 21 Sep 2023 09:01:40 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Thu, 21 Sep 2023 09:01:40 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Thu, 21 Sep 2023 09:01:41 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Thu, 21 Sep 2023 09:01:41 GMT
LABEL org.opencontainers.image.version=1.31.0
# Thu, 21 Sep 2023 09:02:33 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure ruby     && make -j $NCPU ruby-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure ruby     && make -j $NCPU ruby-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && gem install rack && rm -rf /root/.local     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Thu, 21 Sep 2023 09:02:33 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Thu, 21 Sep 2023 09:02:33 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Thu, 21 Sep 2023 09:02:33 GMT
STOPSIGNAL SIGTERM
# Thu, 21 Sep 2023 09:02:33 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 21 Sep 2023 09:02:34 GMT
EXPOSE 80
# Thu, 21 Sep 2023 09:02:34 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:ddf874abf16cc990e0fd75a154a34ca0a03ee310ad895a18fb62ae15bf4171fb`  
		Last Modified: Wed, 20 Sep 2023 05:00:41 GMT  
		Size: 55.1 MB (55056714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1459d3ab8b5e46ac1a0a00134fe2f7b693474eb6d75ace97ecbe811a6f5b0e`  
		Last Modified: Wed, 20 Sep 2023 09:31:06 GMT  
		Size: 15.8 MB (15760408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab00e7798a04602c3f6e2dc445a994d75e96c45533cd44701f58509982a8c5`  
		Last Modified: Wed, 20 Sep 2023 09:31:23 GMT  
		Size: 54.6 MB (54584790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7883a473306cf6632abe7e913e0f1a21ac2fed038a4116473b25738b8b88b294`  
		Last Modified: Wed, 20 Sep 2023 09:31:55 GMT  
		Size: 196.8 MB (196842512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fdcd138618aab34068d5f25a76b9f52fd31968b0ac18bb7d07712e2dfb218da`  
		Last Modified: Thu, 21 Sep 2023 04:31:31 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a1c513a65f8aa3521e033b2594828b7458e09a64b409ae0c845fa78f54dbee`  
		Last Modified: Thu, 21 Sep 2023 04:32:15 GMT  
		Size: 34.6 MB (34555434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef736a5e310922df2e0ec8fea9b8cb6e82f6e05b6728246464e80cbd3323463`  
		Last Modified: Thu, 21 Sep 2023 04:32:12 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852f8560c08590962b1223b1b4098e276106212ed51b79cce0f8c8cc3c7ecf03`  
		Last Modified: Thu, 21 Sep 2023 09:03:59 GMT  
		Size: 7.5 MB (7472725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:355dd321857fb6ccef83d972ba26481615db92cda9272569c448f690bd3caaba`  
		Last Modified: Thu, 21 Sep 2023 09:03:57 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539417e59f1725542c24856f19c2f2a3348df4e315ef3336ff577fa9e163a913`  
		Last Modified: Thu, 21 Sep 2023 09:03:57 GMT  
		Size: 1.5 KB (1464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:ruby3.2` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:dffefd84552257cf59dee4bbe3e0bb6c1d278ea4149b15d4e9839dddd4e1dd05
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.7 MB (355686533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d01d684dd22e47a20187d814ce3077e56cffccc53f1a3681e112e1e6dd9c68e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:20 GMT
ADD file:46dcdcde338d2c01fed5db3fac9041736d9305145d8fc2039dd5b3714d38ede8 in / 
# Wed, 20 Sep 2023 02:44:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:24:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:25:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:26:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 17:00:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 20 Sep 2023 17:00:09 GMT
ENV LANG=C.UTF-8
# Wed, 20 Sep 2023 17:12:43 GMT
ENV RUBY_MAJOR=3.2
# Wed, 20 Sep 2023 17:12:43 GMT
ENV RUBY_VERSION=3.2.2
# Wed, 20 Sep 2023 17:12:43 GMT
ENV RUBY_DOWNLOAD_SHA256=4b352d0f7ec384e332e3e44cdbfdcd5ff2d594af3c8296b5636c710975149e23
# Wed, 20 Sep 2023 17:14:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		rustArch=; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		'amd64') rustArch='x86_64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/x86_64-unknown-linux-gnu/rustup-init'; rustupSha256='5cc9ffd1026e82e7fb2eec2121ad71f4b0f044e88bca39207b3f6b769aaa799c' ;; 		'arm64') rustArch='aarch64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/aarch64-unknown-linux-gnu/rustup-init'; rustupSha256='e189948e396d47254103a49c987e7fb0e5dd8e34b200aa4481ecc4b8e41fb929' ;; 	esac; 		if [ -n "$rustArch" ]; then 		mkdir -p /tmp/rust; 				wget -O /tmp/rust/rustup-init "$rustupUrl"; 		echo "$rustupSha256 */tmp/rust/rustup-init" | sha256sum --check --strict; 		chmod +x /tmp/rust/rustup-init; 				export RUSTUP_HOME='/tmp/rust/rustup' CARGO_HOME='/tmp/rust/cargo'; 		export PATH="$CARGO_HOME/bin:$PATH"; 		/tmp/rust/rustup-init -y --no-modify-path --profile minimal --default-toolchain '1.66.0' --default-host "$rustArch"; 				rustc --version; 		cargo --version; 	fi; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 		${rustArch:+--enable-yjit} 	; 	make -j "$(nproc)"; 	make install; 		rm -rf /tmp/rust; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 20 Sep 2023 17:14:28 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 20 Sep 2023 17:14:28 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 20 Sep 2023 17:14:28 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Sep 2023 17:14:28 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Wed, 20 Sep 2023 17:14:29 GMT
CMD ["irb"]
# Thu, 21 Sep 2023 03:27:09 GMT
LABEL org.opencontainers.image.title=Unit (ruby3.2)
# Thu, 21 Sep 2023 03:27:09 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Thu, 21 Sep 2023 03:27:09 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Thu, 21 Sep 2023 03:27:09 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Thu, 21 Sep 2023 03:27:09 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Thu, 21 Sep 2023 03:27:09 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Thu, 21 Sep 2023 03:27:10 GMT
LABEL org.opencontainers.image.version=1.31.0
# Thu, 21 Sep 2023 03:27:51 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && /bin/true     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure ruby     && make -j $NCPU ruby-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure ruby     && make -j $NCPU ruby-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && gem install rack && rm -rf /root/.local     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Thu, 21 Sep 2023 03:27:51 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Thu, 21 Sep 2023 03:27:51 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Thu, 21 Sep 2023 03:27:51 GMT
STOPSIGNAL SIGTERM
# Thu, 21 Sep 2023 03:27:51 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 21 Sep 2023 03:27:51 GMT
EXPOSE 80
# Thu, 21 Sep 2023 03:27:51 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:31f5dc1f52c865588c43d8ec718f14d430e149b28f0b28232da825da7ae28f76`  
		Last Modified: Wed, 20 Sep 2023 02:47:53 GMT  
		Size: 53.7 MB (53704892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb60045eb75c62e890b95d28e4893132a6c7d61ec9979104ee4ff6e86c4badee`  
		Last Modified: Wed, 20 Sep 2023 09:33:11 GMT  
		Size: 15.7 MB (15746671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292737ab468ef80c6f78bdde4896157b8953d1e5556e1e526f40aeadcb547573`  
		Last Modified: Wed, 20 Sep 2023 09:33:26 GMT  
		Size: 54.7 MB (54676309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d93979d624211374be152eee1c99ed4ca9e6bae68694135fc440ab6c8fd2044`  
		Last Modified: Wed, 20 Sep 2023 09:33:51 GMT  
		Size: 189.8 MB (189778334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b301519822ecf9e91a1d73928dcd311c4bca39d7dc3c8312271a3a87192b6fad`  
		Last Modified: Wed, 20 Sep 2023 17:32:40 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83bd254efa556fb8118a65fd122dfaebb9beb925b07e4bce5dab0753adfe612b`  
		Last Modified: Wed, 20 Sep 2023 17:33:59 GMT  
		Size: 34.4 MB (34432616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf0bf0364fef8b7d14832a31609b05b197fc4cd485098cba635e2dcc48c3a18`  
		Last Modified: Wed, 20 Sep 2023 17:33:56 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddcc516d1030a5cfc66d59f54ada76bc9df6bbc565d4b0e7d2f5f0b7dfcdc755`  
		Last Modified: Thu, 21 Sep 2023 03:29:08 GMT  
		Size: 7.3 MB (7344596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3698a78d8a3fbcff7cc1793bf3bae553dfb607bc4135436e5699d758d6b3b7`  
		Last Modified: Thu, 21 Sep 2023 03:29:07 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7a2e346b9c5a6b73c465209726bfa46af845b73807df32c3a5ac350195ab35`  
		Last Modified: Thu, 21 Sep 2023 03:29:07 GMT  
		Size: 1.5 KB (1469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `unit:wasm`

```console
$ docker pull unit@sha256:d2890c56bd6ed1c9cf1aca41dbca04209c01a40d85a244061b4ebb9a920c9953
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:wasm` - linux; amd64

```console
$ docker pull unit@sha256:7845aa107eff2617b276695e1df86a4761833df366dc4bb223ba13933d9bfd60
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.6 MB (46636244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc633f872efe837e4e06cf567ac808a1e1112294f079c42992cb2c64228fbb2c`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:53:19 GMT
LABEL org.opencontainers.image.title=Unit (wasm)
# Wed, 11 Oct 2023 19:53:19 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Wed, 11 Oct 2023 19:53:19 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Wed, 11 Oct 2023 19:53:19 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Wed, 11 Oct 2023 19:53:19 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Wed, 11 Oct 2023 19:53:19 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 11 Oct 2023 19:53:19 GMT
LABEL org.opencontainers.image.version=1.31.0
# Wed, 11 Oct 2023 19:56:46 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && export RUST_VERSION=1.71.0     && export RUSTUP_HOME=/usr/src/unit/rustup     && export CARGO_HOME=/usr/src/unit/cargo     && export PATH=/usr/src/unit/cargo/bin:$PATH     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in        amd64) rustArch="x86_64-unknown-linux-gnu"; rustupSha256="0b2f6c8f85a3d02fde2efc0ced4657869d73fccfce59defb4e8d29233116e6db" ;;        arm64) rustArch="aarch64-unknown-linux-gnu"; rustupSha256="673e336c81c65e6b16dcdede33f4cc9ed0f08bde1dbe7a935f113605292dc800" ;;        *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac     && url="https://static.rust-lang.org/rustup/archive/1.26.0/${rustArch}/rustup-init"     && curl -L -O "$url"     && echo "${rustupSha256} *rustup-init" | sha256sum -c -     && chmod +x rustup-init     && ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch}     && rm rustup-init     && rustup --version     && cargo --version     && rustc --version     && make -C pkg/contrib .wasmtime     && install -pm 755 pkg/contrib/wasmtime/target/release/libwasmtime.so /usr/lib/$(dpkg-architecture -q DEB_HOST_MULTIARCH)/     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure wasm --include-path=`pwd`/pkg/contrib/wasmtime/crates/c-api/include --lib-path=/usr/lib/$(dpkg-architecture -q DEB_HOST_MULTIARCH)/     && make -j $NCPU wasm-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure wasm --include-path=`pwd`/pkg/contrib/wasmtime/crates/c-api/include --lib-path=/usr/lib/$(dpkg-architecture -q DEB_HOST_MULTIARCH)/     && make -j $NCPU wasm-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Wed, 11 Oct 2023 19:56:47 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Wed, 11 Oct 2023 19:56:47 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Wed, 11 Oct 2023 19:56:47 GMT
STOPSIGNAL SIGTERM
# Wed, 11 Oct 2023 19:56:47 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Wed, 11 Oct 2023 19:56:47 GMT
EXPOSE 80
# Wed, 11 Oct 2023 19:56:47 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9141e09d044816697e52a2955dde172af5396e3c8c1b71153d67f668fa2454`  
		Last Modified: Wed, 11 Oct 2023 19:59:04 GMT  
		Size: 15.2 MB (15215650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5496485089c9075d6a558dcb20d3f86e3c90425b983f76abe65188304e9d4de2`  
		Last Modified: Wed, 11 Oct 2023 19:59:02 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc28d01cbfd6ee3775e414c61a1ae5f000333baff83a6a33eeae1c6bd4ae127`  
		Last Modified: Wed, 11 Oct 2023 19:59:01 GMT  
		Size: 1.5 KB (1469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:wasm` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:9102091e8f914725b06d7bf804d4ec19ac5aff70fe98b70bbbee6b756d9311fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (45044027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe1be587ad1f9b09ad9fbacb9c77ad16d6790b59be9d324f0613bb128f684bb1`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:06 GMT
ADD file:2c3e5451390c62f0b85f20139d2c88011cc54d649cdda5567084c050ad373372 in / 
# Wed, 11 Oct 2023 18:25:06 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:09:12 GMT
LABEL org.opencontainers.image.title=Unit (wasm)
# Wed, 11 Oct 2023 19:09:12 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Wed, 11 Oct 2023 19:09:12 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Wed, 11 Oct 2023 19:09:12 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Wed, 11 Oct 2023 19:09:12 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Wed, 11 Oct 2023 19:09:12 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 11 Oct 2023 19:09:12 GMT
LABEL org.opencontainers.image.version=1.31.0
# Wed, 11 Oct 2023 19:12:13 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && export RUST_VERSION=1.71.0     && export RUSTUP_HOME=/usr/src/unit/rustup     && export CARGO_HOME=/usr/src/unit/cargo     && export PATH=/usr/src/unit/cargo/bin:$PATH     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in        amd64) rustArch="x86_64-unknown-linux-gnu"; rustupSha256="0b2f6c8f85a3d02fde2efc0ced4657869d73fccfce59defb4e8d29233116e6db" ;;        arm64) rustArch="aarch64-unknown-linux-gnu"; rustupSha256="673e336c81c65e6b16dcdede33f4cc9ed0f08bde1dbe7a935f113605292dc800" ;;        *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac     && url="https://static.rust-lang.org/rustup/archive/1.26.0/${rustArch}/rustup-init"     && curl -L -O "$url"     && echo "${rustupSha256} *rustup-init" | sha256sum -c -     && chmod +x rustup-init     && ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch}     && rm rustup-init     && rustup --version     && cargo --version     && rustc --version     && make -C pkg/contrib .wasmtime     && install -pm 755 pkg/contrib/wasmtime/target/release/libwasmtime.so /usr/lib/$(dpkg-architecture -q DEB_HOST_MULTIARCH)/     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure wasm --include-path=`pwd`/pkg/contrib/wasmtime/crates/c-api/include --lib-path=/usr/lib/$(dpkg-architecture -q DEB_HOST_MULTIARCH)/     && make -j $NCPU wasm-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure wasm --include-path=`pwd`/pkg/contrib/wasmtime/crates/c-api/include --lib-path=/usr/lib/$(dpkg-architecture -q DEB_HOST_MULTIARCH)/     && make -j $NCPU wasm-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Wed, 11 Oct 2023 19:12:13 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Wed, 11 Oct 2023 19:12:13 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Wed, 11 Oct 2023 19:12:13 GMT
STOPSIGNAL SIGTERM
# Wed, 11 Oct 2023 19:12:13 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Wed, 11 Oct 2023 19:12:13 GMT
EXPOSE 80
# Wed, 11 Oct 2023 19:12:13 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:85e50d2242ceaba78c3726e059dbd2fa06f5c18e265554bd43a482d19b256d20`  
		Last Modified: Wed, 11 Oct 2023 18:29:07 GMT  
		Size: 30.1 MB (30064086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45870802cfcb84d8f28e525b07f1ab49e3705abd7690bd264c17e773986e6f2d`  
		Last Modified: Wed, 11 Oct 2023 19:14:06 GMT  
		Size: 15.0 MB (14977210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956d6f6dc5a165b604bdd1af481715ae8e2c40783e5ef4dfaf6780a8c91d0d45`  
		Last Modified: Wed, 11 Oct 2023 19:14:04 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51670beaa1ab175b4fc1b8b985cf32289b45e63df30ec8f98eae0f51506a3c3`  
		Last Modified: Wed, 11 Oct 2023 19:14:04 GMT  
		Size: 1.5 KB (1470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
