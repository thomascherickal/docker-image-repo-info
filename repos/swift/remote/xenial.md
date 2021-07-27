## `swift:xenial`

```console
$ docker pull swift@sha256:261b3ff77a41fd5cf455d12d656a9189e291720d7b63b10287a1700b5ddeea8b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `swift:xenial` - linux; amd64

```console
$ docker pull swift@sha256:55e1f1eafa10e143a48434dcdb7e0df634fe217cf917369e822529943141c1e2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **672.5 MB (672457783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41e413a913b546484600610313d906b4c46fc9b319b1c51068f1d61911bf75e0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:22:15 GMT
ADD file:a94a87e268e99c78143fae5148bd1200bf0da90c0e7f42bd8c168bb205ccb105 in / 
# Mon, 26 Jul 2021 21:22:16 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 26 Jul 2021 21:22:17 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:22:17 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 26 Jul 2021 21:22:18 GMT
CMD ["/bin/bash"]
# Tue, 27 Jul 2021 02:18:49 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Tue, 27 Jul 2021 02:18:49 GMT
LABEL Description=Docker Container for the Swift programming language
# Tue, 27 Jul 2021 02:19:52 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl3     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython3.5     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:19:53 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Tue, 27 Jul 2021 02:19:53 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Tue, 27 Jul 2021 02:19:53 GMT
ARG SWIFT_BRANCH=swift-5.4.2-release
# Tue, 27 Jul 2021 02:19:53 GMT
ARG SWIFT_VERSION=swift-5.4.2-RELEASE
# Tue, 27 Jul 2021 02:19:54 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Tue, 27 Jul 2021 02:19:54 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-5.4.2-release SWIFT_VERSION=swift-5.4.2-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Tue, 27 Jul 2021 02:21:22 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Tue, 27 Jul 2021 02:21:27 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:52818491084148fa3469964bbcc3576686018a3b16b2e29be0407565c4c80b44`  
		Last Modified: Thu, 22 Jul 2021 16:25:00 GMT  
		Size: 46.5 MB (46497362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9df81d603d28f2a294b2f11b4f60d07b5b833b2ad7d6659a3f59b10cff2696`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636d9303bf663657be8e6796d720913bb985b5343da7949749ae1e72b54a88d8`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672b5bdcef61237567b311ad3d349f5eae18ba839ce2b204858a3083437a0a59`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386847c8a9b5fe241dfcf5f1383dad17089b6ca867f19c9a6cba8861500f7c0f`  
		Last Modified: Tue, 27 Jul 2021 03:14:27 GMT  
		Size: 112.7 MB (112669127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace6cfc0ae7d8aab16324d9797e6eccf8b485fff12941271c17e6692785436e9`  
		Last Modified: Tue, 27 Jul 2021 03:15:22 GMT  
		Size: 513.3 MB (513289743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
