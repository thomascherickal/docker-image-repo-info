## `unit:wasm`

```console
$ docker pull unit@sha256:ae4cf9f2f55c79389df28fe6e31814d71474b88883bcd52113f8cd5fd99b5beb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:wasm` - linux; amd64

```console
$ docker pull unit@sha256:34efbcd47ef4ce1de9115c06d2aa575fb548d1fc8264857e7283e0dea79c42b8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.6 MB (46638154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f19160a5084ef1579f2aad55d2bc304dd032af68839489de719d0a5169ac210`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 16:23:08 GMT
LABEL org.opencontainers.image.title=Unit (wasm)
# Wed, 01 Nov 2023 16:23:08 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Wed, 01 Nov 2023 16:23:08 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Wed, 01 Nov 2023 16:23:08 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Wed, 01 Nov 2023 16:23:08 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Wed, 01 Nov 2023 16:23:08 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 01 Nov 2023 16:23:08 GMT
LABEL org.opencontainers.image.version=1.31.1
# Wed, 01 Nov 2023 16:26:27 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.1-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && export RUST_VERSION=1.71.0     && export RUSTUP_HOME=/usr/src/unit/rustup     && export CARGO_HOME=/usr/src/unit/cargo     && export PATH=/usr/src/unit/cargo/bin:$PATH     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in        amd64) rustArch="x86_64-unknown-linux-gnu"; rustupSha256="0b2f6c8f85a3d02fde2efc0ced4657869d73fccfce59defb4e8d29233116e6db" ;;        arm64) rustArch="aarch64-unknown-linux-gnu"; rustupSha256="673e336c81c65e6b16dcdede33f4cc9ed0f08bde1dbe7a935f113605292dc800" ;;        *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac     && url="https://static.rust-lang.org/rustup/archive/1.26.0/${rustArch}/rustup-init"     && curl -L -O "$url"     && echo "${rustupSha256} *rustup-init" | sha256sum -c -     && chmod +x rustup-init     && ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch}     && rm rustup-init     && rustup --version     && cargo --version     && rustc --version     && make -C pkg/contrib .wasmtime     && install -pm 755 pkg/contrib/wasmtime/target/release/libwasmtime.so /usr/lib/$(dpkg-architecture -q DEB_HOST_MULTIARCH)/     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure wasm --include-path=`pwd`/pkg/contrib/wasmtime/crates/c-api/include --lib-path=/usr/lib/$(dpkg-architecture -q DEB_HOST_MULTIARCH)/     && make -j $NCPU wasm-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure wasm --include-path=`pwd`/pkg/contrib/wasmtime/crates/c-api/include --lib-path=/usr/lib/$(dpkg-architecture -q DEB_HOST_MULTIARCH)/     && make -j $NCPU wasm-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Wed, 01 Nov 2023 16:26:27 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Wed, 01 Nov 2023 16:26:28 GMT
COPY multi:44b909b4ee0b15a0820a0f95f866a48ec9fbcb6e3c46d6d937842c09126ebe93 in /usr/share/unit/welcome/ 
# Wed, 01 Nov 2023 16:26:28 GMT
STOPSIGNAL SIGTERM
# Wed, 01 Nov 2023 16:26:28 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 16:26:28 GMT
EXPOSE 80
# Wed, 01 Nov 2023 16:26:28 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2cae545b7987c71ade79576ec83b79dfa8bf846e1531781887ae709527d107`  
		Last Modified: Wed, 01 Nov 2023 16:30:08 GMT  
		Size: 15.2 MB (15217488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9fa4258c273137f2cc347462a434c512f4492efe704985a05b6cda679f8e876`  
		Last Modified: Wed, 01 Nov 2023 16:30:06 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7fc0c7e43132bb6060fe74e37a3a9d3b7b8fc100999e3e4d70c8e2af9a9f339`  
		Last Modified: Wed, 01 Nov 2023 16:30:06 GMT  
		Size: 1.5 KB (1486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:wasm` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:019cb367006d09c0d2384b0cd45f259cedfeb19df6b642daefaa88a3d2e7f8ef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (45048949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:216eb93e0669521a10fcd5fdf27ca830947b5f880d3a0b09d00a33a54c4d2234`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:47:41 GMT
LABEL org.opencontainers.image.title=Unit (wasm)
# Wed, 01 Nov 2023 01:47:42 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Wed, 01 Nov 2023 01:47:42 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Wed, 01 Nov 2023 01:47:42 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Wed, 01 Nov 2023 01:47:42 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Wed, 01 Nov 2023 01:47:42 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 01 Nov 2023 01:47:42 GMT
LABEL org.opencontainers.image.version=1.31.1
# Wed, 01 Nov 2023 01:50:52 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && mkdir -p /usr/src/unit     && cd /usr/src/unit     && hg clone -u 1.31.1-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --runstatedir=/var/run                 --pid=/var/run/unit.pid                 --logdir=/var/log                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && export RUST_VERSION=1.71.0     && export RUSTUP_HOME=/usr/src/unit/rustup     && export CARGO_HOME=/usr/src/unit/cargo     && export PATH=/usr/src/unit/cargo/bin:$PATH     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in        amd64) rustArch="x86_64-unknown-linux-gnu"; rustupSha256="0b2f6c8f85a3d02fde2efc0ced4657869d73fccfce59defb4e8d29233116e6db" ;;        arm64) rustArch="aarch64-unknown-linux-gnu"; rustupSha256="673e336c81c65e6b16dcdede33f4cc9ed0f08bde1dbe7a935f113605292dc800" ;;        *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac     && url="https://static.rust-lang.org/rustup/archive/1.26.0/${rustArch}/rustup-init"     && curl -L -O "$url"     && echo "${rustupSha256} *rustup-init" | sha256sum -c -     && chmod +x rustup-init     && ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch}     && rm rustup-init     && rustup --version     && cargo --version     && rustc --version     && make -C pkg/contrib .wasmtime     && install -pm 755 pkg/contrib/wasmtime/target/release/libwasmtime.so /usr/lib/$(dpkg-architecture -q DEB_HOST_MULTIARCH)/     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure wasm --include-path=`pwd`/pkg/contrib/wasmtime/crates/c-api/include --lib-path=/usr/lib/$(dpkg-architecture -q DEB_HOST_MULTIARCH)/     && make -j $NCPU wasm-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure wasm --include-path=`pwd`/pkg/contrib/wasmtime/crates/c-api/include --lib-path=/usr/lib/$(dpkg-architecture -q DEB_HOST_MULTIARCH)/     && make -j $NCPU wasm-install     && cd     && rm -rf /usr/src/unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && /bin/true     && mkdir -p /var/lib/unit/     && mkdir -p /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove build-essential     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Wed, 01 Nov 2023 01:50:52 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Wed, 01 Nov 2023 01:50:52 GMT
COPY multi:44b909b4ee0b15a0820a0f95f866a48ec9fbcb6e3c46d6d937842c09126ebe93 in /usr/share/unit/welcome/ 
# Wed, 01 Nov 2023 01:50:52 GMT
STOPSIGNAL SIGTERM
# Wed, 01 Nov 2023 01:50:52 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 01:50:52 GMT
EXPOSE 80
# Wed, 01 Nov 2023 01:50:52 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673c75c8612dbb1d7b8ce6dbd55637b773e5f58345d84b578b14bc1f53de9bf0`  
		Last Modified: Wed, 01 Nov 2023 01:52:49 GMT  
		Size: 15.0 MB (14982301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76a030cc4496cca6e19f0e401f78f4c2a43dae6b81a71a3138e93dcc46409815`  
		Last Modified: Wed, 01 Nov 2023 01:52:47 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9956585b8b007e8ca80b5fcf0d36e9e34bf203ce0d9ed1170943e0cc255d7c7`  
		Last Modified: Wed, 01 Nov 2023 01:52:47 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
