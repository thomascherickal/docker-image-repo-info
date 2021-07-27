## `swift:xenial-slim`

```console
$ docker pull swift@sha256:2316bdae1ae00e24ab1d40b4c104e5242a7b2503e9a022a15c670198bed4e9e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `swift:xenial-slim` - linux; amd64

```console
$ docker pull swift@sha256:8541b223c40f0ca467ecfd73e471fdf71e5a9be18ccdf9cceb84c6a699d0859b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.7 MB (106668131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8781b821ff93611a9cc8815b10a136f8e15370f4ecca0cf32db19ace79b72631`
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
# Tue, 27 Jul 2021 02:23:35 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl3     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:23:36 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Tue, 27 Jul 2021 02:23:36 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Tue, 27 Jul 2021 02:23:36 GMT
ARG SWIFT_BRANCH=swift-5.4.2-release
# Tue, 27 Jul 2021 02:23:36 GMT
ARG SWIFT_VERSION=swift-5.4.2-RELEASE
# Tue, 27 Jul 2021 02:23:36 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Tue, 27 Jul 2021 02:23:37 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-5.4.2-release SWIFT_VERSION=swift-5.4.2-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Tue, 27 Jul 2021 02:24:55 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
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
	-	`sha256:b7d8fb2ed1d89f34b9d7bc04929518bea677451638ce555e889b9b3cc5bef4db`  
		Last Modified: Tue, 27 Jul 2021 03:16:08 GMT  
		Size: 20.9 MB (20854689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7243dd9d2eb7183271f5120d80a2785aab5709088d12e9edd2c38b6b430e4875`  
		Last Modified: Tue, 27 Jul 2021 03:16:10 GMT  
		Size: 39.3 MB (39314529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
