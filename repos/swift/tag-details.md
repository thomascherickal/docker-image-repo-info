<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `swift`

-	[`swift:4`](#swift4)
-	[`swift:4.0`](#swift40)
-	[`swift:4.0.3`](#swift403)
-	[`swift:4.1`](#swift41)
-	[`swift:4.1.3`](#swift413)
-	[`swift:4.2`](#swift42)
-	[`swift:4.2.4`](#swift424)
-	[`swift:5.0`](#swift50)
-	[`swift:5.0.3`](#swift503)
-	[`swift:5.0.3-bionic`](#swift503-bionic)
-	[`swift:5.0.3-bionic-slim`](#swift503-bionic-slim)
-	[`swift:5.0.3-slim`](#swift503-slim)
-	[`swift:5.0.3-xenial`](#swift503-xenial)
-	[`swift:5.0.3-xenial-slim`](#swift503-xenial-slim)
-	[`swift:5.0-bionic`](#swift50-bionic)
-	[`swift:5.0-bionic-slim`](#swift50-bionic-slim)
-	[`swift:5.0-slim`](#swift50-slim)
-	[`swift:5.0-xenial`](#swift50-xenial)
-	[`swift:5.0-xenial-slim`](#swift50-xenial-slim)
-	[`swift:5.1`](#swift51)
-	[`swift:5.1.5`](#swift515)
-	[`swift:5.1.5-bionic`](#swift515-bionic)
-	[`swift:5.1.5-bionic-sim`](#swift515-bionic-sim)
-	[`swift:5.1.5-slim`](#swift515-slim)
-	[`swift:5.1.5-xenial`](#swift515-xenial)
-	[`swift:5.1.5-xenial-slim`](#swift515-xenial-slim)
-	[`swift:5.1-bionic`](#swift51-bionic)
-	[`swift:5.1-bionic-slim`](#swift51-bionic-slim)
-	[`swift:5.1-slim`](#swift51-slim)
-	[`swift:5.1-xenial`](#swift51-xenial)
-	[`swift:5.1-xenial-slim`](#swift51-xenial-slim)
-	[`swift:5.2`](#swift52)
-	[`swift:5.2.4`](#swift524)
-	[`swift:5.2.4-amazonlinux2`](#swift524-amazonlinux2)
-	[`swift:5.2.4-bionic`](#swift524-bionic)
-	[`swift:5.2.4-bionic-slim`](#swift524-bionic-slim)
-	[`swift:5.2.4-centos8`](#swift524-centos8)
-	[`swift:5.2.4-focal`](#swift524-focal)
-	[`swift:5.2.4-focal-slim`](#swift524-focal-slim)
-	[`swift:5.2.4-slim`](#swift524-slim)
-	[`swift:5.2.4-xenial`](#swift524-xenial)
-	[`swift:5.2.4-xenial-slim`](#swift524-xenial-slim)
-	[`swift:5.2-amazonlinux2`](#swift52-amazonlinux2)
-	[`swift:5.2-bionic`](#swift52-bionic)
-	[`swift:5.2-bionic-slim`](#swift52-bionic-slim)
-	[`swift:5.2-centos8`](#swift52-centos8)
-	[`swift:5.2-focal`](#swift52-focal)
-	[`swift:5.2-focal-slim`](#swift52-focal-slim)
-	[`swift:5.2-slim`](#swift52-slim)
-	[`swift:5.2-xenial`](#swift52-xenial)
-	[`swift:5.2-xenial-slim`](#swift52-xenial-slim)
-	[`swift:amazonlinux2`](#swiftamazonlinux2)
-	[`swift:bionic`](#swiftbionic)
-	[`swift:bionic-slim`](#swiftbionic-slim)
-	[`swift:centos8`](#swiftcentos8)
-	[`swift:focal`](#swiftfocal)
-	[`swift:focal-slim`](#swiftfocal-slim)
-	[`swift:latest`](#swiftlatest)
-	[`swift:slim`](#swiftslim)
-	[`swift:xenial`](#swiftxenial)
-	[`swift:xenial-slim`](#swiftxenial-slim)

## `swift:4`

```console
$ docker pull swift@sha256:a01d5ab899cab508c6a79b1ce0bee06a22f4987c44ab0398ea746c93fdfea2df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:4` - linux; amd64

```console
$ docker pull swift@sha256:84dad7a26fff979130e085c16e5cfa936e9e43f95187776b29090644d67cf3d6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **496.9 MB (496906748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24fc24f760ee5da735398a4a6ef3e19194839f0a4337b3504eff513b7c1e656c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:21:26 GMT
ADD file:52af30f80ba214985a59cb0ef7073c64f8514d58396c0de48f8d7056dec2a58a in / 
# Wed, 17 Jun 2020 01:21:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:21:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:21:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:30:50 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:30:51 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:54:13 GMT
RUN apt-get -q update &&     apt-get -q install -y     make     libc6-dev     clang-3.8     curl     libedit-dev     libpython2.7     libicu-dev     libssl-dev     libxml2     tzdata     git     libcurl4-openssl-dev     pkg-config     && update-alternatives --quiet --install /usr/bin/clang clang /usr/bin/clang-3.8 100     && update-alternatives --quiet --install /usr/bin/clang++ clang++ /usr/bin/clang++-3.8 100     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:54:14 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Wed, 17 Jun 2020 02:54:14 GMT
ARG SWIFT_BRANCH=swift-4.2.4-release
# Wed, 17 Jun 2020 02:54:14 GMT
ARG SWIFT_VERSION=swift-4.2.4-RELEASE
# Wed, 17 Jun 2020 02:54:14 GMT
ENV SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-4.2.4-release SWIFT_VERSION=swift-4.2.4-RELEASE
# Wed, 17 Jun 2020 02:55:05 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           8513444E2DA36B7C1659AF4D7638F1FB2B2B08C4           A3BAFD3556A59079C06894BD63BC1CFE91D306C6           5E4DF843FB065D7F7E24FBA2EF5430F071E1B235         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
# Wed, 17 Jun 2020 02:55:06 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:b5e173e44934e01d8d2674bc8b1da00f761c4fe796e0fb2bee1bd1129d2e4ae1`  
		Last Modified: Fri, 15 May 2020 13:20:22 GMT  
		Size: 44.3 MB (44320272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29047100b0407dff554ea80b8005380d62b13a66d7fe2e2adb07b9c091b9f2c0`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 531.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15743a713c2a4033877dab08fb3989280f8c856234227158a4011811c7991372`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6bc9e2987763aa991b7dfd742be04c7b3bb04448982ffe88e58d55c93b76d4`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b125f8d2d0441dacd4e9a55e8fcecad38c3ad8e553de763ff44f657815044815`  
		Last Modified: Wed, 17 Jun 2020 03:08:10 GMT  
		Size: 224.4 MB (224418762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04526488707dd74c733137847f6d0006a8dc6904ba27ca5343656fed5bc04cd`  
		Last Modified: Wed, 17 Jun 2020 03:08:10 GMT  
		Size: 228.2 MB (228166158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:4.0`

```console
$ docker pull swift@sha256:785332ccf720db48a19fd51ebb36da7538cdcb6a2cdab431e29d33aa02547f5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:4.0` - linux; amd64

```console
$ docker pull swift@sha256:a2b16e3b71c5a2b4290f6d22bb369762f3f0a771bc7208de6dc2ce3d030386fe
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **439.4 MB (439377926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f6984f85056f6fe22da098d6cab41af9e89e73e1c45c02aef21aa76ff7554fe`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:21:26 GMT
ADD file:52af30f80ba214985a59cb0ef7073c64f8514d58396c0de48f8d7056dec2a58a in / 
# Wed, 17 Jun 2020 01:21:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:21:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:21:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:55:23 GMT
LABEL maintainer=Haris Amin <aminharis7@gmail.com>
# Wed, 17 Jun 2020 02:55:23 GMT
LABEL Description=Docker Container for the Apple's Swift programming language
# Wed, 17 Jun 2020 02:56:07 GMT
RUN apt-get -q update &&     apt-get -q install -y     make     libc6-dev     clang-3.8     curl     libedit-dev     libpython2.7     libicu-dev     libssl-dev     libxml2     tzdata     git     libcurl4-openssl-dev     pkg-config     && update-alternatives --quiet --install /usr/bin/clang clang /usr/bin/clang-3.8 100     && update-alternatives --quiet --install /usr/bin/clang++ clang++ /usr/bin/clang++-3.8 100     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:56:08 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Wed, 17 Jun 2020 02:56:53 GMT
ARG SWIFT_BRANCH=swift-4.0.3-release
# Wed, 17 Jun 2020 02:56:54 GMT
ARG SWIFT_VERSION=swift-4.0.3-RELEASE
# Wed, 17 Jun 2020 02:56:54 GMT
ENV SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-4.0.3-release SWIFT_VERSION=swift-4.0.3-RELEASE
# Wed, 17 Jun 2020 02:57:27 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           8513444E2DA36B7C1659AF4D7638F1FB2B2B08C4           A3BAFD3556A59079C06894BD63BC1CFE91D306C6           5E4DF843FB065D7F7E24FBA2EF5430F071E1B235         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
# Wed, 17 Jun 2020 02:57:28 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:b5e173e44934e01d8d2674bc8b1da00f761c4fe796e0fb2bee1bd1129d2e4ae1`  
		Last Modified: Fri, 15 May 2020 13:20:22 GMT  
		Size: 44.3 MB (44320272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29047100b0407dff554ea80b8005380d62b13a66d7fe2e2adb07b9c091b9f2c0`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 531.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15743a713c2a4033877dab08fb3989280f8c856234227158a4011811c7991372`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6bc9e2987763aa991b7dfd742be04c7b3bb04448982ffe88e58d55c93b76d4`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa46eca315d5b3d72dfb876acd26740b6cef733b8627370d5725a6c6b08d8dd`  
		Last Modified: Wed, 17 Jun 2020 03:09:04 GMT  
		Size: 224.4 MB (224418162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50aa96607c0151ca128cff35b2be1f7e7384a57c07d1ee68bc380e94393d902`  
		Last Modified: Wed, 17 Jun 2020 03:09:40 GMT  
		Size: 170.6 MB (170637936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:4.0.3`

```console
$ docker pull swift@sha256:785332ccf720db48a19fd51ebb36da7538cdcb6a2cdab431e29d33aa02547f5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:4.0.3` - linux; amd64

```console
$ docker pull swift@sha256:a2b16e3b71c5a2b4290f6d22bb369762f3f0a771bc7208de6dc2ce3d030386fe
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **439.4 MB (439377926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f6984f85056f6fe22da098d6cab41af9e89e73e1c45c02aef21aa76ff7554fe`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:21:26 GMT
ADD file:52af30f80ba214985a59cb0ef7073c64f8514d58396c0de48f8d7056dec2a58a in / 
# Wed, 17 Jun 2020 01:21:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:21:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:21:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:55:23 GMT
LABEL maintainer=Haris Amin <aminharis7@gmail.com>
# Wed, 17 Jun 2020 02:55:23 GMT
LABEL Description=Docker Container for the Apple's Swift programming language
# Wed, 17 Jun 2020 02:56:07 GMT
RUN apt-get -q update &&     apt-get -q install -y     make     libc6-dev     clang-3.8     curl     libedit-dev     libpython2.7     libicu-dev     libssl-dev     libxml2     tzdata     git     libcurl4-openssl-dev     pkg-config     && update-alternatives --quiet --install /usr/bin/clang clang /usr/bin/clang-3.8 100     && update-alternatives --quiet --install /usr/bin/clang++ clang++ /usr/bin/clang++-3.8 100     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:56:08 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Wed, 17 Jun 2020 02:56:53 GMT
ARG SWIFT_BRANCH=swift-4.0.3-release
# Wed, 17 Jun 2020 02:56:54 GMT
ARG SWIFT_VERSION=swift-4.0.3-RELEASE
# Wed, 17 Jun 2020 02:56:54 GMT
ENV SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-4.0.3-release SWIFT_VERSION=swift-4.0.3-RELEASE
# Wed, 17 Jun 2020 02:57:27 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           8513444E2DA36B7C1659AF4D7638F1FB2B2B08C4           A3BAFD3556A59079C06894BD63BC1CFE91D306C6           5E4DF843FB065D7F7E24FBA2EF5430F071E1B235         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
# Wed, 17 Jun 2020 02:57:28 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:b5e173e44934e01d8d2674bc8b1da00f761c4fe796e0fb2bee1bd1129d2e4ae1`  
		Last Modified: Fri, 15 May 2020 13:20:22 GMT  
		Size: 44.3 MB (44320272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29047100b0407dff554ea80b8005380d62b13a66d7fe2e2adb07b9c091b9f2c0`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 531.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15743a713c2a4033877dab08fb3989280f8c856234227158a4011811c7991372`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6bc9e2987763aa991b7dfd742be04c7b3bb04448982ffe88e58d55c93b76d4`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa46eca315d5b3d72dfb876acd26740b6cef733b8627370d5725a6c6b08d8dd`  
		Last Modified: Wed, 17 Jun 2020 03:09:04 GMT  
		Size: 224.4 MB (224418162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50aa96607c0151ca128cff35b2be1f7e7384a57c07d1ee68bc380e94393d902`  
		Last Modified: Wed, 17 Jun 2020 03:09:40 GMT  
		Size: 170.6 MB (170637936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:4.1`

```console
$ docker pull swift@sha256:bf0dd3ba35a0c96ca2a7b1948900ebb18c9d92d67c606d1469bc800225e6027e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:4.1` - linux; amd64

```console
$ docker pull swift@sha256:f58c5f06dd22b1088c3b257a1be06c1fc97ff668a55be176f81df16d99387cd0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **452.0 MB (451972258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e76bce7f413fd5797fe204ee7a24766c040534ecc642614d03a7572e71d1f98e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:21:26 GMT
ADD file:52af30f80ba214985a59cb0ef7073c64f8514d58396c0de48f8d7056dec2a58a in / 
# Wed, 17 Jun 2020 01:21:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:21:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:21:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:55:23 GMT
LABEL maintainer=Haris Amin <aminharis7@gmail.com>
# Wed, 17 Jun 2020 02:55:23 GMT
LABEL Description=Docker Container for the Apple's Swift programming language
# Wed, 17 Jun 2020 02:56:07 GMT
RUN apt-get -q update &&     apt-get -q install -y     make     libc6-dev     clang-3.8     curl     libedit-dev     libpython2.7     libicu-dev     libssl-dev     libxml2     tzdata     git     libcurl4-openssl-dev     pkg-config     && update-alternatives --quiet --install /usr/bin/clang clang /usr/bin/clang-3.8 100     && update-alternatives --quiet --install /usr/bin/clang++ clang++ /usr/bin/clang++-3.8 100     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:56:08 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Wed, 17 Jun 2020 02:56:08 GMT
ARG SWIFT_BRANCH=swift-4.1.3-release
# Wed, 17 Jun 2020 02:56:08 GMT
ARG SWIFT_VERSION=swift-4.1.3-RELEASE
# Wed, 17 Jun 2020 02:56:09 GMT
ENV SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-4.1.3-release SWIFT_VERSION=swift-4.1.3-RELEASE
# Wed, 17 Jun 2020 02:56:44 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           8513444E2DA36B7C1659AF4D7638F1FB2B2B08C4           A3BAFD3556A59079C06894BD63BC1CFE91D306C6           5E4DF843FB065D7F7E24FBA2EF5430F071E1B235         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
# Wed, 17 Jun 2020 02:56:45 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:b5e173e44934e01d8d2674bc8b1da00f761c4fe796e0fb2bee1bd1129d2e4ae1`  
		Last Modified: Fri, 15 May 2020 13:20:22 GMT  
		Size: 44.3 MB (44320272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29047100b0407dff554ea80b8005380d62b13a66d7fe2e2adb07b9c091b9f2c0`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 531.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15743a713c2a4033877dab08fb3989280f8c856234227158a4011811c7991372`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6bc9e2987763aa991b7dfd742be04c7b3bb04448982ffe88e58d55c93b76d4`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa46eca315d5b3d72dfb876acd26740b6cef733b8627370d5725a6c6b08d8dd`  
		Last Modified: Wed, 17 Jun 2020 03:09:04 GMT  
		Size: 224.4 MB (224418162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d7be5a739d1983b6d94d6aa94ce4281c6066040f6e30b57dec4f62b96de5b0`  
		Last Modified: Wed, 17 Jun 2020 03:08:55 GMT  
		Size: 183.2 MB (183232268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:4.1.3`

```console
$ docker pull swift@sha256:bf0dd3ba35a0c96ca2a7b1948900ebb18c9d92d67c606d1469bc800225e6027e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:4.1.3` - linux; amd64

```console
$ docker pull swift@sha256:f58c5f06dd22b1088c3b257a1be06c1fc97ff668a55be176f81df16d99387cd0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **452.0 MB (451972258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e76bce7f413fd5797fe204ee7a24766c040534ecc642614d03a7572e71d1f98e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:21:26 GMT
ADD file:52af30f80ba214985a59cb0ef7073c64f8514d58396c0de48f8d7056dec2a58a in / 
# Wed, 17 Jun 2020 01:21:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:21:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:21:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:55:23 GMT
LABEL maintainer=Haris Amin <aminharis7@gmail.com>
# Wed, 17 Jun 2020 02:55:23 GMT
LABEL Description=Docker Container for the Apple's Swift programming language
# Wed, 17 Jun 2020 02:56:07 GMT
RUN apt-get -q update &&     apt-get -q install -y     make     libc6-dev     clang-3.8     curl     libedit-dev     libpython2.7     libicu-dev     libssl-dev     libxml2     tzdata     git     libcurl4-openssl-dev     pkg-config     && update-alternatives --quiet --install /usr/bin/clang clang /usr/bin/clang-3.8 100     && update-alternatives --quiet --install /usr/bin/clang++ clang++ /usr/bin/clang++-3.8 100     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:56:08 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Wed, 17 Jun 2020 02:56:08 GMT
ARG SWIFT_BRANCH=swift-4.1.3-release
# Wed, 17 Jun 2020 02:56:08 GMT
ARG SWIFT_VERSION=swift-4.1.3-RELEASE
# Wed, 17 Jun 2020 02:56:09 GMT
ENV SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-4.1.3-release SWIFT_VERSION=swift-4.1.3-RELEASE
# Wed, 17 Jun 2020 02:56:44 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           8513444E2DA36B7C1659AF4D7638F1FB2B2B08C4           A3BAFD3556A59079C06894BD63BC1CFE91D306C6           5E4DF843FB065D7F7E24FBA2EF5430F071E1B235         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
# Wed, 17 Jun 2020 02:56:45 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:b5e173e44934e01d8d2674bc8b1da00f761c4fe796e0fb2bee1bd1129d2e4ae1`  
		Last Modified: Fri, 15 May 2020 13:20:22 GMT  
		Size: 44.3 MB (44320272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29047100b0407dff554ea80b8005380d62b13a66d7fe2e2adb07b9c091b9f2c0`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 531.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15743a713c2a4033877dab08fb3989280f8c856234227158a4011811c7991372`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6bc9e2987763aa991b7dfd742be04c7b3bb04448982ffe88e58d55c93b76d4`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa46eca315d5b3d72dfb876acd26740b6cef733b8627370d5725a6c6b08d8dd`  
		Last Modified: Wed, 17 Jun 2020 03:09:04 GMT  
		Size: 224.4 MB (224418162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d7be5a739d1983b6d94d6aa94ce4281c6066040f6e30b57dec4f62b96de5b0`  
		Last Modified: Wed, 17 Jun 2020 03:08:55 GMT  
		Size: 183.2 MB (183232268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:4.2`

```console
$ docker pull swift@sha256:a01d5ab899cab508c6a79b1ce0bee06a22f4987c44ab0398ea746c93fdfea2df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:4.2` - linux; amd64

```console
$ docker pull swift@sha256:84dad7a26fff979130e085c16e5cfa936e9e43f95187776b29090644d67cf3d6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **496.9 MB (496906748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24fc24f760ee5da735398a4a6ef3e19194839f0a4337b3504eff513b7c1e656c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:21:26 GMT
ADD file:52af30f80ba214985a59cb0ef7073c64f8514d58396c0de48f8d7056dec2a58a in / 
# Wed, 17 Jun 2020 01:21:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:21:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:21:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:30:50 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:30:51 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:54:13 GMT
RUN apt-get -q update &&     apt-get -q install -y     make     libc6-dev     clang-3.8     curl     libedit-dev     libpython2.7     libicu-dev     libssl-dev     libxml2     tzdata     git     libcurl4-openssl-dev     pkg-config     && update-alternatives --quiet --install /usr/bin/clang clang /usr/bin/clang-3.8 100     && update-alternatives --quiet --install /usr/bin/clang++ clang++ /usr/bin/clang++-3.8 100     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:54:14 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Wed, 17 Jun 2020 02:54:14 GMT
ARG SWIFT_BRANCH=swift-4.2.4-release
# Wed, 17 Jun 2020 02:54:14 GMT
ARG SWIFT_VERSION=swift-4.2.4-RELEASE
# Wed, 17 Jun 2020 02:54:14 GMT
ENV SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-4.2.4-release SWIFT_VERSION=swift-4.2.4-RELEASE
# Wed, 17 Jun 2020 02:55:05 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           8513444E2DA36B7C1659AF4D7638F1FB2B2B08C4           A3BAFD3556A59079C06894BD63BC1CFE91D306C6           5E4DF843FB065D7F7E24FBA2EF5430F071E1B235         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
# Wed, 17 Jun 2020 02:55:06 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:b5e173e44934e01d8d2674bc8b1da00f761c4fe796e0fb2bee1bd1129d2e4ae1`  
		Last Modified: Fri, 15 May 2020 13:20:22 GMT  
		Size: 44.3 MB (44320272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29047100b0407dff554ea80b8005380d62b13a66d7fe2e2adb07b9c091b9f2c0`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 531.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15743a713c2a4033877dab08fb3989280f8c856234227158a4011811c7991372`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6bc9e2987763aa991b7dfd742be04c7b3bb04448982ffe88e58d55c93b76d4`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b125f8d2d0441dacd4e9a55e8fcecad38c3ad8e553de763ff44f657815044815`  
		Last Modified: Wed, 17 Jun 2020 03:08:10 GMT  
		Size: 224.4 MB (224418762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04526488707dd74c733137847f6d0006a8dc6904ba27ca5343656fed5bc04cd`  
		Last Modified: Wed, 17 Jun 2020 03:08:10 GMT  
		Size: 228.2 MB (228166158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:4.2.4`

```console
$ docker pull swift@sha256:a01d5ab899cab508c6a79b1ce0bee06a22f4987c44ab0398ea746c93fdfea2df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:4.2.4` - linux; amd64

```console
$ docker pull swift@sha256:84dad7a26fff979130e085c16e5cfa936e9e43f95187776b29090644d67cf3d6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **496.9 MB (496906748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24fc24f760ee5da735398a4a6ef3e19194839f0a4337b3504eff513b7c1e656c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:21:26 GMT
ADD file:52af30f80ba214985a59cb0ef7073c64f8514d58396c0de48f8d7056dec2a58a in / 
# Wed, 17 Jun 2020 01:21:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:21:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:21:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:30:50 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:30:51 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:54:13 GMT
RUN apt-get -q update &&     apt-get -q install -y     make     libc6-dev     clang-3.8     curl     libedit-dev     libpython2.7     libicu-dev     libssl-dev     libxml2     tzdata     git     libcurl4-openssl-dev     pkg-config     && update-alternatives --quiet --install /usr/bin/clang clang /usr/bin/clang-3.8 100     && update-alternatives --quiet --install /usr/bin/clang++ clang++ /usr/bin/clang++-3.8 100     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:54:14 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Wed, 17 Jun 2020 02:54:14 GMT
ARG SWIFT_BRANCH=swift-4.2.4-release
# Wed, 17 Jun 2020 02:54:14 GMT
ARG SWIFT_VERSION=swift-4.2.4-RELEASE
# Wed, 17 Jun 2020 02:54:14 GMT
ENV SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-4.2.4-release SWIFT_VERSION=swift-4.2.4-RELEASE
# Wed, 17 Jun 2020 02:55:05 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           8513444E2DA36B7C1659AF4D7638F1FB2B2B08C4           A3BAFD3556A59079C06894BD63BC1CFE91D306C6           5E4DF843FB065D7F7E24FBA2EF5430F071E1B235         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
# Wed, 17 Jun 2020 02:55:06 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:b5e173e44934e01d8d2674bc8b1da00f761c4fe796e0fb2bee1bd1129d2e4ae1`  
		Last Modified: Fri, 15 May 2020 13:20:22 GMT  
		Size: 44.3 MB (44320272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29047100b0407dff554ea80b8005380d62b13a66d7fe2e2adb07b9c091b9f2c0`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 531.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15743a713c2a4033877dab08fb3989280f8c856234227158a4011811c7991372`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6bc9e2987763aa991b7dfd742be04c7b3bb04448982ffe88e58d55c93b76d4`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b125f8d2d0441dacd4e9a55e8fcecad38c3ad8e553de763ff44f657815044815`  
		Last Modified: Wed, 17 Jun 2020 03:08:10 GMT  
		Size: 224.4 MB (224418762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04526488707dd74c733137847f6d0006a8dc6904ba27ca5343656fed5bc04cd`  
		Last Modified: Wed, 17 Jun 2020 03:08:10 GMT  
		Size: 228.2 MB (228166158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.0`

```console
$ docker pull swift@sha256:fcbb57d5f041306c825e8a3d0e35475c747642573609d42a77be3c34679758c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.0` - linux; amd64

```console
$ docker pull swift@sha256:ffad55b23e4866ac3a7e72ae3ff17c34eb4056a3b3349dfd69a8a20960584fcc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **470.4 MB (470447298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6acacdb106c3c8e4debbfdf57475a2b70a4211089b8696a79e4ff54cb40260a9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:20:29 GMT
ADD file:1e8d02626176dc8141df3c0a1365774ce73d79934654fe24a4b1e7f173108232 in / 
# Wed, 17 Jun 2020 01:20:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:20:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:20:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:20:32 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:46:51 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libbsd0     libcurl4     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:46:52 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Wed, 17 Jun 2020 02:46:52 GMT
ARG SWIFT_BRANCH=swift-5.0.3-release
# Wed, 17 Jun 2020 02:46:52 GMT
ARG SWIFT_VERSION=swift-5.0.3-RELEASE
# Wed, 17 Jun 2020 02:46:52 GMT
ENV SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.0.3-release SWIFT_VERSION=swift-5.0.3-RELEASE
# Wed, 17 Jun 2020 02:48:01 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && apt-get update     && apt-get install -y curl     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && apt-get purge -y curl     && apt-get -y autoremove     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           A62AE125BBBFBB96A6E042EC925CC1CCED3D1561         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
# Wed, 17 Jun 2020 02:48:02 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:d7c3167c320d7a820935f54cf4290890ea19567da496ecf774e8773b35d5f065`  
		Last Modified: Wed, 27 May 2020 12:21:15 GMT  
		Size: 26.7 MB (26688718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131f805ec7fd68d45a887e2ef82de61de0247b4eb934ab03b7c933650e854baa`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 35.4 KB (35369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322ed380e680a77f30528ba013e3a802a7b44948a0609c7d1d732dd46a9a310d`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac240b130982ad1c3ba3188abbf18ba4e54bdd9e504ce2d5c2eff6d3e86b8dd`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d5bd2a2852e46257a1879a29eedf76cb544f697e8d2c7f141336844381aedc`  
		Last Modified: Wed, 17 Jun 2020 03:05:21 GMT  
		Size: 123.9 MB (123946294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24ea156cf8eff7b3a1510b38b4655d885b8756fd057e5e97968615e462a09513`  
		Last Modified: Wed, 17 Jun 2020 03:05:50 GMT  
		Size: 319.8 MB (319775910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.0.3`

```console
$ docker pull swift@sha256:fcbb57d5f041306c825e8a3d0e35475c747642573609d42a77be3c34679758c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.0.3` - linux; amd64

```console
$ docker pull swift@sha256:ffad55b23e4866ac3a7e72ae3ff17c34eb4056a3b3349dfd69a8a20960584fcc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **470.4 MB (470447298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6acacdb106c3c8e4debbfdf57475a2b70a4211089b8696a79e4ff54cb40260a9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:20:29 GMT
ADD file:1e8d02626176dc8141df3c0a1365774ce73d79934654fe24a4b1e7f173108232 in / 
# Wed, 17 Jun 2020 01:20:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:20:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:20:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:20:32 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:46:51 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libbsd0     libcurl4     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:46:52 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Wed, 17 Jun 2020 02:46:52 GMT
ARG SWIFT_BRANCH=swift-5.0.3-release
# Wed, 17 Jun 2020 02:46:52 GMT
ARG SWIFT_VERSION=swift-5.0.3-RELEASE
# Wed, 17 Jun 2020 02:46:52 GMT
ENV SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.0.3-release SWIFT_VERSION=swift-5.0.3-RELEASE
# Wed, 17 Jun 2020 02:48:01 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && apt-get update     && apt-get install -y curl     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && apt-get purge -y curl     && apt-get -y autoremove     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           A62AE125BBBFBB96A6E042EC925CC1CCED3D1561         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
# Wed, 17 Jun 2020 02:48:02 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:d7c3167c320d7a820935f54cf4290890ea19567da496ecf774e8773b35d5f065`  
		Last Modified: Wed, 27 May 2020 12:21:15 GMT  
		Size: 26.7 MB (26688718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131f805ec7fd68d45a887e2ef82de61de0247b4eb934ab03b7c933650e854baa`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 35.4 KB (35369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322ed380e680a77f30528ba013e3a802a7b44948a0609c7d1d732dd46a9a310d`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac240b130982ad1c3ba3188abbf18ba4e54bdd9e504ce2d5c2eff6d3e86b8dd`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d5bd2a2852e46257a1879a29eedf76cb544f697e8d2c7f141336844381aedc`  
		Last Modified: Wed, 17 Jun 2020 03:05:21 GMT  
		Size: 123.9 MB (123946294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24ea156cf8eff7b3a1510b38b4655d885b8756fd057e5e97968615e462a09513`  
		Last Modified: Wed, 17 Jun 2020 03:05:50 GMT  
		Size: 319.8 MB (319775910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.0.3-bionic`

```console
$ docker pull swift@sha256:fcbb57d5f041306c825e8a3d0e35475c747642573609d42a77be3c34679758c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.0.3-bionic` - linux; amd64

```console
$ docker pull swift@sha256:ffad55b23e4866ac3a7e72ae3ff17c34eb4056a3b3349dfd69a8a20960584fcc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **470.4 MB (470447298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6acacdb106c3c8e4debbfdf57475a2b70a4211089b8696a79e4ff54cb40260a9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:20:29 GMT
ADD file:1e8d02626176dc8141df3c0a1365774ce73d79934654fe24a4b1e7f173108232 in / 
# Wed, 17 Jun 2020 01:20:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:20:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:20:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:20:32 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:46:51 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libbsd0     libcurl4     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:46:52 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Wed, 17 Jun 2020 02:46:52 GMT
ARG SWIFT_BRANCH=swift-5.0.3-release
# Wed, 17 Jun 2020 02:46:52 GMT
ARG SWIFT_VERSION=swift-5.0.3-RELEASE
# Wed, 17 Jun 2020 02:46:52 GMT
ENV SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.0.3-release SWIFT_VERSION=swift-5.0.3-RELEASE
# Wed, 17 Jun 2020 02:48:01 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && apt-get update     && apt-get install -y curl     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && apt-get purge -y curl     && apt-get -y autoremove     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           A62AE125BBBFBB96A6E042EC925CC1CCED3D1561         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
# Wed, 17 Jun 2020 02:48:02 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:d7c3167c320d7a820935f54cf4290890ea19567da496ecf774e8773b35d5f065`  
		Last Modified: Wed, 27 May 2020 12:21:15 GMT  
		Size: 26.7 MB (26688718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131f805ec7fd68d45a887e2ef82de61de0247b4eb934ab03b7c933650e854baa`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 35.4 KB (35369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322ed380e680a77f30528ba013e3a802a7b44948a0609c7d1d732dd46a9a310d`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac240b130982ad1c3ba3188abbf18ba4e54bdd9e504ce2d5c2eff6d3e86b8dd`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d5bd2a2852e46257a1879a29eedf76cb544f697e8d2c7f141336844381aedc`  
		Last Modified: Wed, 17 Jun 2020 03:05:21 GMT  
		Size: 123.9 MB (123946294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24ea156cf8eff7b3a1510b38b4655d885b8756fd057e5e97968615e462a09513`  
		Last Modified: Wed, 17 Jun 2020 03:05:50 GMT  
		Size: 319.8 MB (319775910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.0.3-bionic-slim`

```console
$ docker pull swift@sha256:8b5a3b5950e15ac68b1fb16cb4d5494f40527f02b731f0a2d8b435848ecd2b8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.0.3-bionic-slim` - linux; amd64

```console
$ docker pull swift@sha256:7aaa4c4411d45159adf8a2c07b960463e55f71f0ac3ac5968a781a88fc6f1f31
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75145843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cd9c24d13a9eac5e43de15759e48e9b2f77cd87d5a043471e22c166443d43be`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:20:29 GMT
ADD file:1e8d02626176dc8141df3c0a1365774ce73d79934654fe24a4b1e7f173108232 in / 
# Wed, 17 Jun 2020 01:20:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:20:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:20:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:20:32 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:50:41 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libbsd0     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:50:41 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Wed, 17 Jun 2020 02:50:41 GMT
ARG SWIFT_BRANCH=swift-5.0.3-release
# Wed, 17 Jun 2020 02:50:41 GMT
ARG SWIFT_VERSION=swift-5.0.3-RELEASE
# Wed, 17 Jun 2020 02:50:42 GMT
ENV SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.0.3-release SWIFT_VERSION=swift-5.0.3-RELEASE
# Wed, 17 Jun 2020 02:51:42 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && apt-get update     && apt-get install -y curl gpg     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           A62AE125BBBFBB96A6E042EC925CC1CCED3D1561         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && apt-get purge -y curl gpg     && apt-get -y autoremove     && rm -r /var/lib/apt/lists/*     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
```

-	Layers:
	-	`sha256:d7c3167c320d7a820935f54cf4290890ea19567da496ecf774e8773b35d5f065`  
		Last Modified: Wed, 27 May 2020 12:21:15 GMT  
		Size: 26.7 MB (26688718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131f805ec7fd68d45a887e2ef82de61de0247b4eb934ab03b7c933650e854baa`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 35.4 KB (35369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322ed380e680a77f30528ba013e3a802a7b44948a0609c7d1d732dd46a9a310d`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac240b130982ad1c3ba3188abbf18ba4e54bdd9e504ce2d5c2eff6d3e86b8dd`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06e94088f921d6e0a7c41d12e2374cd0283085d37dab8f41f8ca519a96c3a43`  
		Last Modified: Wed, 17 Jun 2020 03:07:06 GMT  
		Size: 20.5 MB (20522167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa700d52e3d06446f2d1a157577ab997482e883b2c3d22663597236c8c41a93c`  
		Last Modified: Wed, 17 Jun 2020 03:07:07 GMT  
		Size: 27.9 MB (27898582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.0.3-slim`

```console
$ docker pull swift@sha256:8b5a3b5950e15ac68b1fb16cb4d5494f40527f02b731f0a2d8b435848ecd2b8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.0.3-slim` - linux; amd64

```console
$ docker pull swift@sha256:7aaa4c4411d45159adf8a2c07b960463e55f71f0ac3ac5968a781a88fc6f1f31
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75145843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cd9c24d13a9eac5e43de15759e48e9b2f77cd87d5a043471e22c166443d43be`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:20:29 GMT
ADD file:1e8d02626176dc8141df3c0a1365774ce73d79934654fe24a4b1e7f173108232 in / 
# Wed, 17 Jun 2020 01:20:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:20:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:20:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:20:32 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:50:41 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libbsd0     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:50:41 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Wed, 17 Jun 2020 02:50:41 GMT
ARG SWIFT_BRANCH=swift-5.0.3-release
# Wed, 17 Jun 2020 02:50:41 GMT
ARG SWIFT_VERSION=swift-5.0.3-RELEASE
# Wed, 17 Jun 2020 02:50:42 GMT
ENV SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.0.3-release SWIFT_VERSION=swift-5.0.3-RELEASE
# Wed, 17 Jun 2020 02:51:42 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && apt-get update     && apt-get install -y curl gpg     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           A62AE125BBBFBB96A6E042EC925CC1CCED3D1561         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && apt-get purge -y curl gpg     && apt-get -y autoremove     && rm -r /var/lib/apt/lists/*     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
```

-	Layers:
	-	`sha256:d7c3167c320d7a820935f54cf4290890ea19567da496ecf774e8773b35d5f065`  
		Last Modified: Wed, 27 May 2020 12:21:15 GMT  
		Size: 26.7 MB (26688718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131f805ec7fd68d45a887e2ef82de61de0247b4eb934ab03b7c933650e854baa`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 35.4 KB (35369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322ed380e680a77f30528ba013e3a802a7b44948a0609c7d1d732dd46a9a310d`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac240b130982ad1c3ba3188abbf18ba4e54bdd9e504ce2d5c2eff6d3e86b8dd`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06e94088f921d6e0a7c41d12e2374cd0283085d37dab8f41f8ca519a96c3a43`  
		Last Modified: Wed, 17 Jun 2020 03:07:06 GMT  
		Size: 20.5 MB (20522167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa700d52e3d06446f2d1a157577ab997482e883b2c3d22663597236c8c41a93c`  
		Last Modified: Wed, 17 Jun 2020 03:07:07 GMT  
		Size: 27.9 MB (27898582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.0.3-xenial`

```console
$ docker pull swift@sha256:80b328f0b71a0935b7653df7caa815e78565a5fb578ee794aaa99c726bb9483d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.0.3-xenial` - linux; amd64

```console
$ docker pull swift@sha256:a6d7807d100f124109dcd8c620be6bd0e8a0f45e529afc78f94f2b0921b494d4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **478.3 MB (478337129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1cfbbdf77db915eebc860e6ee63aaff30b35ade8f9bdeca14aafcfdf910dadf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:21:26 GMT
ADD file:52af30f80ba214985a59cb0ef7073c64f8514d58396c0de48f8d7056dec2a58a in / 
# Wed, 17 Jun 2020 01:21:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:21:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:21:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:30:50 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:30:51 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:48:56 GMT
RUN apt-get -q update &&     apt-get -q install -y     libatomic1     libbsd0     libcurl3     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:48:56 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Wed, 17 Jun 2020 02:48:56 GMT
ARG SWIFT_BRANCH=swift-5.0.3-release
# Wed, 17 Jun 2020 02:48:57 GMT
ARG SWIFT_VERSION=swift-5.0.3-RELEASE
# Wed, 17 Jun 2020 02:48:57 GMT
ENV SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-5.0.3-release SWIFT_VERSION=swift-5.0.3-RELEASE
# Wed, 17 Jun 2020 02:50:01 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && apt-get -q update     && apt-get -q install -y curl     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && apt-get purge -y curl     && apt-get -y autoremove     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           A62AE125BBBFBB96A6E042EC925CC1CCED3D1561         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
# Wed, 17 Jun 2020 02:50:04 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:b5e173e44934e01d8d2674bc8b1da00f761c4fe796e0fb2bee1bd1129d2e4ae1`  
		Last Modified: Fri, 15 May 2020 13:20:22 GMT  
		Size: 44.3 MB (44320272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29047100b0407dff554ea80b8005380d62b13a66d7fe2e2adb07b9c091b9f2c0`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 531.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15743a713c2a4033877dab08fb3989280f8c856234227158a4011811c7991372`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6bc9e2987763aa991b7dfd742be04c7b3bb04448982ffe88e58d55c93b76d4`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb1d6b003531517a0c0096bfcbf73e6636885d38a1f75af70896c2d786ae911`  
		Last Modified: Wed, 17 Jun 2020 03:06:21 GMT  
		Size: 111.3 MB (111348097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc021e908c8ee75b84c8eba32a83d102593f0dc9835cedd61ec08de98984c00`  
		Last Modified: Wed, 17 Jun 2020 03:06:53 GMT  
		Size: 322.7 MB (322667204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.0.3-xenial-slim`

```console
$ docker pull swift@sha256:227f307b3b436fbee4bb856b12c64503650c5388ba9f4fe238013283e736e240
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.0.3-xenial-slim` - linux; amd64

```console
$ docker pull swift@sha256:849eefc95164130e886d795e248937e00886b7626d011b344c308d338f853a74
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.0 MB (92997459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5bba6dc476f0282e519a1cc98b04d518b3d0897ab4fc8f99da7d333e44ae458`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:21:26 GMT
ADD file:52af30f80ba214985a59cb0ef7073c64f8514d58396c0de48f8d7056dec2a58a in / 
# Wed, 17 Jun 2020 01:21:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:21:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:21:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:30:50 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:30:51 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:52:03 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libbsd0     libcurl3     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:52:03 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Wed, 17 Jun 2020 02:52:04 GMT
ARG SWIFT_BRANCH=swift-5.0.3-release
# Wed, 17 Jun 2020 02:52:04 GMT
ARG SWIFT_VERSION=swift-5.0.3-RELEASE
# Wed, 17 Jun 2020 02:52:04 GMT
ENV SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-5.0.3-release SWIFT_VERSION=swift-5.0.3-RELEASE
# Wed, 17 Jun 2020 02:53:14 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && apt-get update     && apt-get install -y curl     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           A62AE125BBBFBB96A6E042EC925CC1CCED3D1561         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && apt-get purge -y curl     && apt-get -y autoremove     && rm -r /var/lib/apt/lists/*     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
```

-	Layers:
	-	`sha256:b5e173e44934e01d8d2674bc8b1da00f761c4fe796e0fb2bee1bd1129d2e4ae1`  
		Last Modified: Fri, 15 May 2020 13:20:22 GMT  
		Size: 44.3 MB (44320272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29047100b0407dff554ea80b8005380d62b13a66d7fe2e2adb07b9c091b9f2c0`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 531.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15743a713c2a4033877dab08fb3989280f8c856234227158a4011811c7991372`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6bc9e2987763aa991b7dfd742be04c7b3bb04448982ffe88e58d55c93b76d4`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c750646be99df81decf4de4bc96e74e510f705da522d4673d7cf3cf021fe7dc`  
		Last Modified: Wed, 17 Jun 2020 03:07:17 GMT  
		Size: 20.9 MB (20890211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45da07476c09730e022f6a1cbb1c646bb9d7a120eb2e11d38fce06c27376a980`  
		Last Modified: Wed, 17 Jun 2020 03:07:19 GMT  
		Size: 27.8 MB (27785420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.0-bionic`

```console
$ docker pull swift@sha256:fcbb57d5f041306c825e8a3d0e35475c747642573609d42a77be3c34679758c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.0-bionic` - linux; amd64

```console
$ docker pull swift@sha256:ffad55b23e4866ac3a7e72ae3ff17c34eb4056a3b3349dfd69a8a20960584fcc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **470.4 MB (470447298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6acacdb106c3c8e4debbfdf57475a2b70a4211089b8696a79e4ff54cb40260a9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:20:29 GMT
ADD file:1e8d02626176dc8141df3c0a1365774ce73d79934654fe24a4b1e7f173108232 in / 
# Wed, 17 Jun 2020 01:20:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:20:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:20:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:20:32 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:46:51 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libbsd0     libcurl4     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:46:52 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Wed, 17 Jun 2020 02:46:52 GMT
ARG SWIFT_BRANCH=swift-5.0.3-release
# Wed, 17 Jun 2020 02:46:52 GMT
ARG SWIFT_VERSION=swift-5.0.3-RELEASE
# Wed, 17 Jun 2020 02:46:52 GMT
ENV SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.0.3-release SWIFT_VERSION=swift-5.0.3-RELEASE
# Wed, 17 Jun 2020 02:48:01 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && apt-get update     && apt-get install -y curl     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && apt-get purge -y curl     && apt-get -y autoremove     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           A62AE125BBBFBB96A6E042EC925CC1CCED3D1561         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
# Wed, 17 Jun 2020 02:48:02 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:d7c3167c320d7a820935f54cf4290890ea19567da496ecf774e8773b35d5f065`  
		Last Modified: Wed, 27 May 2020 12:21:15 GMT  
		Size: 26.7 MB (26688718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131f805ec7fd68d45a887e2ef82de61de0247b4eb934ab03b7c933650e854baa`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 35.4 KB (35369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322ed380e680a77f30528ba013e3a802a7b44948a0609c7d1d732dd46a9a310d`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac240b130982ad1c3ba3188abbf18ba4e54bdd9e504ce2d5c2eff6d3e86b8dd`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d5bd2a2852e46257a1879a29eedf76cb544f697e8d2c7f141336844381aedc`  
		Last Modified: Wed, 17 Jun 2020 03:05:21 GMT  
		Size: 123.9 MB (123946294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24ea156cf8eff7b3a1510b38b4655d885b8756fd057e5e97968615e462a09513`  
		Last Modified: Wed, 17 Jun 2020 03:05:50 GMT  
		Size: 319.8 MB (319775910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.0-bionic-slim`

```console
$ docker pull swift@sha256:8b5a3b5950e15ac68b1fb16cb4d5494f40527f02b731f0a2d8b435848ecd2b8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.0-bionic-slim` - linux; amd64

```console
$ docker pull swift@sha256:7aaa4c4411d45159adf8a2c07b960463e55f71f0ac3ac5968a781a88fc6f1f31
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75145843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cd9c24d13a9eac5e43de15759e48e9b2f77cd87d5a043471e22c166443d43be`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:20:29 GMT
ADD file:1e8d02626176dc8141df3c0a1365774ce73d79934654fe24a4b1e7f173108232 in / 
# Wed, 17 Jun 2020 01:20:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:20:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:20:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:20:32 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:50:41 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libbsd0     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:50:41 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Wed, 17 Jun 2020 02:50:41 GMT
ARG SWIFT_BRANCH=swift-5.0.3-release
# Wed, 17 Jun 2020 02:50:41 GMT
ARG SWIFT_VERSION=swift-5.0.3-RELEASE
# Wed, 17 Jun 2020 02:50:42 GMT
ENV SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.0.3-release SWIFT_VERSION=swift-5.0.3-RELEASE
# Wed, 17 Jun 2020 02:51:42 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && apt-get update     && apt-get install -y curl gpg     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           A62AE125BBBFBB96A6E042EC925CC1CCED3D1561         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && apt-get purge -y curl gpg     && apt-get -y autoremove     && rm -r /var/lib/apt/lists/*     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
```

-	Layers:
	-	`sha256:d7c3167c320d7a820935f54cf4290890ea19567da496ecf774e8773b35d5f065`  
		Last Modified: Wed, 27 May 2020 12:21:15 GMT  
		Size: 26.7 MB (26688718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131f805ec7fd68d45a887e2ef82de61de0247b4eb934ab03b7c933650e854baa`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 35.4 KB (35369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322ed380e680a77f30528ba013e3a802a7b44948a0609c7d1d732dd46a9a310d`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac240b130982ad1c3ba3188abbf18ba4e54bdd9e504ce2d5c2eff6d3e86b8dd`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06e94088f921d6e0a7c41d12e2374cd0283085d37dab8f41f8ca519a96c3a43`  
		Last Modified: Wed, 17 Jun 2020 03:07:06 GMT  
		Size: 20.5 MB (20522167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa700d52e3d06446f2d1a157577ab997482e883b2c3d22663597236c8c41a93c`  
		Last Modified: Wed, 17 Jun 2020 03:07:07 GMT  
		Size: 27.9 MB (27898582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.0-slim`

```console
$ docker pull swift@sha256:8b5a3b5950e15ac68b1fb16cb4d5494f40527f02b731f0a2d8b435848ecd2b8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.0-slim` - linux; amd64

```console
$ docker pull swift@sha256:7aaa4c4411d45159adf8a2c07b960463e55f71f0ac3ac5968a781a88fc6f1f31
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75145843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cd9c24d13a9eac5e43de15759e48e9b2f77cd87d5a043471e22c166443d43be`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:20:29 GMT
ADD file:1e8d02626176dc8141df3c0a1365774ce73d79934654fe24a4b1e7f173108232 in / 
# Wed, 17 Jun 2020 01:20:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:20:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:20:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:20:32 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:50:41 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libbsd0     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:50:41 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Wed, 17 Jun 2020 02:50:41 GMT
ARG SWIFT_BRANCH=swift-5.0.3-release
# Wed, 17 Jun 2020 02:50:41 GMT
ARG SWIFT_VERSION=swift-5.0.3-RELEASE
# Wed, 17 Jun 2020 02:50:42 GMT
ENV SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.0.3-release SWIFT_VERSION=swift-5.0.3-RELEASE
# Wed, 17 Jun 2020 02:51:42 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && apt-get update     && apt-get install -y curl gpg     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           A62AE125BBBFBB96A6E042EC925CC1CCED3D1561         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && apt-get purge -y curl gpg     && apt-get -y autoremove     && rm -r /var/lib/apt/lists/*     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
```

-	Layers:
	-	`sha256:d7c3167c320d7a820935f54cf4290890ea19567da496ecf774e8773b35d5f065`  
		Last Modified: Wed, 27 May 2020 12:21:15 GMT  
		Size: 26.7 MB (26688718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131f805ec7fd68d45a887e2ef82de61de0247b4eb934ab03b7c933650e854baa`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 35.4 KB (35369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322ed380e680a77f30528ba013e3a802a7b44948a0609c7d1d732dd46a9a310d`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac240b130982ad1c3ba3188abbf18ba4e54bdd9e504ce2d5c2eff6d3e86b8dd`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06e94088f921d6e0a7c41d12e2374cd0283085d37dab8f41f8ca519a96c3a43`  
		Last Modified: Wed, 17 Jun 2020 03:07:06 GMT  
		Size: 20.5 MB (20522167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa700d52e3d06446f2d1a157577ab997482e883b2c3d22663597236c8c41a93c`  
		Last Modified: Wed, 17 Jun 2020 03:07:07 GMT  
		Size: 27.9 MB (27898582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.0-xenial`

```console
$ docker pull swift@sha256:80b328f0b71a0935b7653df7caa815e78565a5fb578ee794aaa99c726bb9483d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.0-xenial` - linux; amd64

```console
$ docker pull swift@sha256:a6d7807d100f124109dcd8c620be6bd0e8a0f45e529afc78f94f2b0921b494d4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **478.3 MB (478337129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1cfbbdf77db915eebc860e6ee63aaff30b35ade8f9bdeca14aafcfdf910dadf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:21:26 GMT
ADD file:52af30f80ba214985a59cb0ef7073c64f8514d58396c0de48f8d7056dec2a58a in / 
# Wed, 17 Jun 2020 01:21:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:21:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:21:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:30:50 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:30:51 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:48:56 GMT
RUN apt-get -q update &&     apt-get -q install -y     libatomic1     libbsd0     libcurl3     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:48:56 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Wed, 17 Jun 2020 02:48:56 GMT
ARG SWIFT_BRANCH=swift-5.0.3-release
# Wed, 17 Jun 2020 02:48:57 GMT
ARG SWIFT_VERSION=swift-5.0.3-RELEASE
# Wed, 17 Jun 2020 02:48:57 GMT
ENV SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-5.0.3-release SWIFT_VERSION=swift-5.0.3-RELEASE
# Wed, 17 Jun 2020 02:50:01 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && apt-get -q update     && apt-get -q install -y curl     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && apt-get purge -y curl     && apt-get -y autoremove     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           A62AE125BBBFBB96A6E042EC925CC1CCED3D1561         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
# Wed, 17 Jun 2020 02:50:04 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:b5e173e44934e01d8d2674bc8b1da00f761c4fe796e0fb2bee1bd1129d2e4ae1`  
		Last Modified: Fri, 15 May 2020 13:20:22 GMT  
		Size: 44.3 MB (44320272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29047100b0407dff554ea80b8005380d62b13a66d7fe2e2adb07b9c091b9f2c0`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 531.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15743a713c2a4033877dab08fb3989280f8c856234227158a4011811c7991372`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6bc9e2987763aa991b7dfd742be04c7b3bb04448982ffe88e58d55c93b76d4`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb1d6b003531517a0c0096bfcbf73e6636885d38a1f75af70896c2d786ae911`  
		Last Modified: Wed, 17 Jun 2020 03:06:21 GMT  
		Size: 111.3 MB (111348097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc021e908c8ee75b84c8eba32a83d102593f0dc9835cedd61ec08de98984c00`  
		Last Modified: Wed, 17 Jun 2020 03:06:53 GMT  
		Size: 322.7 MB (322667204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.0-xenial-slim`

```console
$ docker pull swift@sha256:227f307b3b436fbee4bb856b12c64503650c5388ba9f4fe238013283e736e240
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.0-xenial-slim` - linux; amd64

```console
$ docker pull swift@sha256:849eefc95164130e886d795e248937e00886b7626d011b344c308d338f853a74
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.0 MB (92997459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5bba6dc476f0282e519a1cc98b04d518b3d0897ab4fc8f99da7d333e44ae458`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:21:26 GMT
ADD file:52af30f80ba214985a59cb0ef7073c64f8514d58396c0de48f8d7056dec2a58a in / 
# Wed, 17 Jun 2020 01:21:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:21:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:21:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:30:50 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:30:51 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:52:03 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libbsd0     libcurl3     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:52:03 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Wed, 17 Jun 2020 02:52:04 GMT
ARG SWIFT_BRANCH=swift-5.0.3-release
# Wed, 17 Jun 2020 02:52:04 GMT
ARG SWIFT_VERSION=swift-5.0.3-RELEASE
# Wed, 17 Jun 2020 02:52:04 GMT
ENV SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-5.0.3-release SWIFT_VERSION=swift-5.0.3-RELEASE
# Wed, 17 Jun 2020 02:53:14 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && apt-get update     && apt-get install -y curl     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           A62AE125BBBFBB96A6E042EC925CC1CCED3D1561         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && apt-get purge -y curl     && apt-get -y autoremove     && rm -r /var/lib/apt/lists/*     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
```

-	Layers:
	-	`sha256:b5e173e44934e01d8d2674bc8b1da00f761c4fe796e0fb2bee1bd1129d2e4ae1`  
		Last Modified: Fri, 15 May 2020 13:20:22 GMT  
		Size: 44.3 MB (44320272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29047100b0407dff554ea80b8005380d62b13a66d7fe2e2adb07b9c091b9f2c0`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 531.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15743a713c2a4033877dab08fb3989280f8c856234227158a4011811c7991372`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6bc9e2987763aa991b7dfd742be04c7b3bb04448982ffe88e58d55c93b76d4`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c750646be99df81decf4de4bc96e74e510f705da522d4673d7cf3cf021fe7dc`  
		Last Modified: Wed, 17 Jun 2020 03:07:17 GMT  
		Size: 20.9 MB (20890211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45da07476c09730e022f6a1cbb1c646bb9d7a120eb2e11d38fce06c27376a980`  
		Last Modified: Wed, 17 Jun 2020 03:07:19 GMT  
		Size: 27.8 MB (27785420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.1`

```console
$ docker pull swift@sha256:7764d8043034901fa585d3d1093cac9c20af39cd05cdee54b8777591dfc113cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.1` - linux; amd64

```console
$ docker pull swift@sha256:7b05c665aa1857a8ccb971ba3c9e0b874a7d9beac4c3aac44393109174e295c3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **495.9 MB (495944434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb9689095c7488fdb3f59688234eda1f6f1a23cfa2241b10a791c60408e06220`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:20:29 GMT
ADD file:1e8d02626176dc8141df3c0a1365774ce73d79934654fe24a4b1e7f173108232 in / 
# Wed, 17 Jun 2020 01:20:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:20:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:20:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:20:32 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:29:10 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:29:10 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 17 Jun 2020 02:29:11 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Wed, 17 Jun 2020 02:40:46 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Wed, 17 Jun 2020 02:40:47 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Wed, 17 Jun 2020 02:40:47 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:40:47 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:42:08 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Wed, 17 Jun 2020 02:42:11 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:d7c3167c320d7a820935f54cf4290890ea19567da496ecf774e8773b35d5f065`  
		Last Modified: Wed, 27 May 2020 12:21:15 GMT  
		Size: 26.7 MB (26688718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131f805ec7fd68d45a887e2ef82de61de0247b4eb934ab03b7c933650e854baa`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 35.4 KB (35369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322ed380e680a77f30528ba013e3a802a7b44948a0609c7d1d732dd46a9a310d`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac240b130982ad1c3ba3188abbf18ba4e54bdd9e504ce2d5c2eff6d3e86b8dd`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459101facad87c08bc7770f59f7ce58838101b487f08e56534d241b1637ea11f`  
		Last Modified: Wed, 17 Jun 2020 02:58:20 GMT  
		Size: 124.1 MB (124051844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6857d0fd3a7a85202dfef410b6aeccd5b91834aa1e619fe2dd7e37862bef843a`  
		Last Modified: Wed, 17 Jun 2020 03:03:15 GMT  
		Size: 345.2 MB (345167496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.1.5`

```console
$ docker pull swift@sha256:7764d8043034901fa585d3d1093cac9c20af39cd05cdee54b8777591dfc113cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.1.5` - linux; amd64

```console
$ docker pull swift@sha256:7b05c665aa1857a8ccb971ba3c9e0b874a7d9beac4c3aac44393109174e295c3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **495.9 MB (495944434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb9689095c7488fdb3f59688234eda1f6f1a23cfa2241b10a791c60408e06220`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:20:29 GMT
ADD file:1e8d02626176dc8141df3c0a1365774ce73d79934654fe24a4b1e7f173108232 in / 
# Wed, 17 Jun 2020 01:20:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:20:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:20:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:20:32 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:29:10 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:29:10 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 17 Jun 2020 02:29:11 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Wed, 17 Jun 2020 02:40:46 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Wed, 17 Jun 2020 02:40:47 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Wed, 17 Jun 2020 02:40:47 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:40:47 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:42:08 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Wed, 17 Jun 2020 02:42:11 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:d7c3167c320d7a820935f54cf4290890ea19567da496ecf774e8773b35d5f065`  
		Last Modified: Wed, 27 May 2020 12:21:15 GMT  
		Size: 26.7 MB (26688718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131f805ec7fd68d45a887e2ef82de61de0247b4eb934ab03b7c933650e854baa`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 35.4 KB (35369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322ed380e680a77f30528ba013e3a802a7b44948a0609c7d1d732dd46a9a310d`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac240b130982ad1c3ba3188abbf18ba4e54bdd9e504ce2d5c2eff6d3e86b8dd`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459101facad87c08bc7770f59f7ce58838101b487f08e56534d241b1637ea11f`  
		Last Modified: Wed, 17 Jun 2020 02:58:20 GMT  
		Size: 124.1 MB (124051844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6857d0fd3a7a85202dfef410b6aeccd5b91834aa1e619fe2dd7e37862bef843a`  
		Last Modified: Wed, 17 Jun 2020 03:03:15 GMT  
		Size: 345.2 MB (345167496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.1.5-bionic`

```console
$ docker pull swift@sha256:7764d8043034901fa585d3d1093cac9c20af39cd05cdee54b8777591dfc113cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.1.5-bionic` - linux; amd64

```console
$ docker pull swift@sha256:7b05c665aa1857a8ccb971ba3c9e0b874a7d9beac4c3aac44393109174e295c3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **495.9 MB (495944434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb9689095c7488fdb3f59688234eda1f6f1a23cfa2241b10a791c60408e06220`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:20:29 GMT
ADD file:1e8d02626176dc8141df3c0a1365774ce73d79934654fe24a4b1e7f173108232 in / 
# Wed, 17 Jun 2020 01:20:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:20:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:20:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:20:32 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:29:10 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:29:10 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 17 Jun 2020 02:29:11 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Wed, 17 Jun 2020 02:40:46 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Wed, 17 Jun 2020 02:40:47 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Wed, 17 Jun 2020 02:40:47 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:40:47 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:42:08 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Wed, 17 Jun 2020 02:42:11 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:d7c3167c320d7a820935f54cf4290890ea19567da496ecf774e8773b35d5f065`  
		Last Modified: Wed, 27 May 2020 12:21:15 GMT  
		Size: 26.7 MB (26688718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131f805ec7fd68d45a887e2ef82de61de0247b4eb934ab03b7c933650e854baa`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 35.4 KB (35369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322ed380e680a77f30528ba013e3a802a7b44948a0609c7d1d732dd46a9a310d`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac240b130982ad1c3ba3188abbf18ba4e54bdd9e504ce2d5c2eff6d3e86b8dd`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459101facad87c08bc7770f59f7ce58838101b487f08e56534d241b1637ea11f`  
		Last Modified: Wed, 17 Jun 2020 02:58:20 GMT  
		Size: 124.1 MB (124051844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6857d0fd3a7a85202dfef410b6aeccd5b91834aa1e619fe2dd7e37862bef843a`  
		Last Modified: Wed, 17 Jun 2020 03:03:15 GMT  
		Size: 345.2 MB (345167496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.1.5-bionic-sim`

```console
$ docker pull swift@sha256:c4146dea1cb982be993c2fda6d750a461f871fad47edd838910f2599ab529eca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.1.5-bionic-sim` - linux; amd64

```console
$ docker pull swift@sha256:725f6808874492ea1a1ad38c11c28196ddeb01abd41fa5c3c3eaa2655e1336d3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78279628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:550bb76939d0422ee624fac8bfc01e1c7426df1fc576670df9aa1237ab5434a4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:20:29 GMT
ADD file:1e8d02626176dc8141df3c0a1365774ce73d79934654fe24a4b1e7f173108232 in / 
# Wed, 17 Jun 2020 01:20:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:20:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:20:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:20:32 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:33:54 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:33:54 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 17 Jun 2020 02:33:55 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Wed, 17 Jun 2020 02:43:50 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Wed, 17 Jun 2020 02:43:50 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Wed, 17 Jun 2020 02:43:50 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:43:50 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:44:57 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl gnupg && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl gnupg
```

-	Layers:
	-	`sha256:d7c3167c320d7a820935f54cf4290890ea19567da496ecf774e8773b35d5f065`  
		Last Modified: Wed, 27 May 2020 12:21:15 GMT  
		Size: 26.7 MB (26688718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131f805ec7fd68d45a887e2ef82de61de0247b4eb934ab03b7c933650e854baa`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 35.4 KB (35369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322ed380e680a77f30528ba013e3a802a7b44948a0609c7d1d732dd46a9a310d`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac240b130982ad1c3ba3188abbf18ba4e54bdd9e504ce2d5c2eff6d3e86b8dd`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be976c7c6b240f9e676229be402cd77dde5ddbf2fd331b3bfa7b9ee1099456e`  
		Last Modified: Wed, 17 Jun 2020 03:00:32 GMT  
		Size: 20.5 MB (20471960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e00a5688786d8ce5a3479b38a3dda1581778276baadc4bfcf4018c80b6405f`  
		Last Modified: Wed, 17 Jun 2020 03:04:33 GMT  
		Size: 31.1 MB (31082574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.1.5-slim`

```console
$ docker pull swift@sha256:c4146dea1cb982be993c2fda6d750a461f871fad47edd838910f2599ab529eca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.1.5-slim` - linux; amd64

```console
$ docker pull swift@sha256:725f6808874492ea1a1ad38c11c28196ddeb01abd41fa5c3c3eaa2655e1336d3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78279628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:550bb76939d0422ee624fac8bfc01e1c7426df1fc576670df9aa1237ab5434a4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:20:29 GMT
ADD file:1e8d02626176dc8141df3c0a1365774ce73d79934654fe24a4b1e7f173108232 in / 
# Wed, 17 Jun 2020 01:20:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:20:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:20:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:20:32 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:33:54 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:33:54 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 17 Jun 2020 02:33:55 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Wed, 17 Jun 2020 02:43:50 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Wed, 17 Jun 2020 02:43:50 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Wed, 17 Jun 2020 02:43:50 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:43:50 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:44:57 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl gnupg && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl gnupg
```

-	Layers:
	-	`sha256:d7c3167c320d7a820935f54cf4290890ea19567da496ecf774e8773b35d5f065`  
		Last Modified: Wed, 27 May 2020 12:21:15 GMT  
		Size: 26.7 MB (26688718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131f805ec7fd68d45a887e2ef82de61de0247b4eb934ab03b7c933650e854baa`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 35.4 KB (35369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322ed380e680a77f30528ba013e3a802a7b44948a0609c7d1d732dd46a9a310d`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac240b130982ad1c3ba3188abbf18ba4e54bdd9e504ce2d5c2eff6d3e86b8dd`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be976c7c6b240f9e676229be402cd77dde5ddbf2fd331b3bfa7b9ee1099456e`  
		Last Modified: Wed, 17 Jun 2020 03:00:32 GMT  
		Size: 20.5 MB (20471960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e00a5688786d8ce5a3479b38a3dda1581778276baadc4bfcf4018c80b6405f`  
		Last Modified: Wed, 17 Jun 2020 03:04:33 GMT  
		Size: 31.1 MB (31082574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.1.5-xenial`

```console
$ docker pull swift@sha256:5fa5415ba0ce26adfbcb91746c836f9a46e5ee3f456dfcdb43d5f685dfbec7b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.1.5-xenial` - linux; amd64

```console
$ docker pull swift@sha256:b14699138c385daea671c2ffb4431356e23cb08bacfa280acab798b677f106c9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **507.3 MB (507331249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a4028b0bae9526420a01c8190d03606516e971184529352d018cf352542ac32`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:21:26 GMT
ADD file:52af30f80ba214985a59cb0ef7073c64f8514d58396c0de48f8d7056dec2a58a in / 
# Wed, 17 Jun 2020 01:21:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:21:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:21:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:30:50 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:30:51 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:31:47 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl3     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:31:47 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 17 Jun 2020 02:31:48 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Wed, 17 Jun 2020 02:42:17 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Wed, 17 Jun 2020 02:42:17 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Wed, 17 Jun 2020 02:42:17 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:42:17 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:43:35 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Wed, 17 Jun 2020 02:43:36 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:b5e173e44934e01d8d2674bc8b1da00f761c4fe796e0fb2bee1bd1129d2e4ae1`  
		Last Modified: Fri, 15 May 2020 13:20:22 GMT  
		Size: 44.3 MB (44320272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29047100b0407dff554ea80b8005380d62b13a66d7fe2e2adb07b9c091b9f2c0`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 531.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15743a713c2a4033877dab08fb3989280f8c856234227158a4011811c7991372`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6bc9e2987763aa991b7dfd742be04c7b3bb04448982ffe88e58d55c93b76d4`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11426dc469ff356e2be300a91a31d297702f5754f463aaa564ca00b9a37b1ea2`  
		Last Modified: Wed, 17 Jun 2020 02:59:31 GMT  
		Size: 111.5 MB (111534848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3729d059f49fdc753c1b0d3ceda2aca772e9a59f53c064c3d6d90d49993365a1`  
		Last Modified: Wed, 17 Jun 2020 03:04:22 GMT  
		Size: 351.5 MB (351474573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.1.5-xenial-slim`

```console
$ docker pull swift@sha256:24d792b53a59a3e312bc3c5382c3d5785cc09d1049621d272fc0c8ea87321176
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.1.5-xenial-slim` - linux; amd64

```console
$ docker pull swift@sha256:d7da6d34f0eb0f1e4957ef1f63abd385a5e897f7140f1c1fa05689810667a235
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.1 MB (96120187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4bcd36d3f681de6487aef094750f0b9bf19de448b6dbe0098e75e46e04ee880`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:21:26 GMT
ADD file:52af30f80ba214985a59cb0ef7073c64f8514d58396c0de48f8d7056dec2a58a in / 
# Wed, 17 Jun 2020 01:21:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:21:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:21:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:30:50 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:30:51 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:35:35 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl3     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:35:35 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 17 Jun 2020 02:35:36 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Wed, 17 Jun 2020 02:45:03 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Wed, 17 Jun 2020 02:45:03 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Wed, 17 Jun 2020 02:45:03 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:45:04 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:46:08 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
```

-	Layers:
	-	`sha256:b5e173e44934e01d8d2674bc8b1da00f761c4fe796e0fb2bee1bd1129d2e4ae1`  
		Last Modified: Fri, 15 May 2020 13:20:22 GMT  
		Size: 44.3 MB (44320272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29047100b0407dff554ea80b8005380d62b13a66d7fe2e2adb07b9c091b9f2c0`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 531.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15743a713c2a4033877dab08fb3989280f8c856234227158a4011811c7991372`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6bc9e2987763aa991b7dfd742be04c7b3bb04448982ffe88e58d55c93b76d4`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da1f8178404835f2182a23ff9eb65d65ff3015da8d71433f43db492410a3129d`  
		Last Modified: Wed, 17 Jun 2020 03:00:45 GMT  
		Size: 20.8 MB (20845087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6debc65f38c536ec4c3ca49ba47b7482b005ba87d60f1f8539e02d0a7fd4745`  
		Last Modified: Wed, 17 Jun 2020 03:04:48 GMT  
		Size: 31.0 MB (30953272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.1-bionic`

```console
$ docker pull swift@sha256:7764d8043034901fa585d3d1093cac9c20af39cd05cdee54b8777591dfc113cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.1-bionic` - linux; amd64

```console
$ docker pull swift@sha256:7b05c665aa1857a8ccb971ba3c9e0b874a7d9beac4c3aac44393109174e295c3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **495.9 MB (495944434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb9689095c7488fdb3f59688234eda1f6f1a23cfa2241b10a791c60408e06220`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:20:29 GMT
ADD file:1e8d02626176dc8141df3c0a1365774ce73d79934654fe24a4b1e7f173108232 in / 
# Wed, 17 Jun 2020 01:20:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:20:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:20:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:20:32 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:29:10 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:29:10 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 17 Jun 2020 02:29:11 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Wed, 17 Jun 2020 02:40:46 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Wed, 17 Jun 2020 02:40:47 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Wed, 17 Jun 2020 02:40:47 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:40:47 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:42:08 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Wed, 17 Jun 2020 02:42:11 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:d7c3167c320d7a820935f54cf4290890ea19567da496ecf774e8773b35d5f065`  
		Last Modified: Wed, 27 May 2020 12:21:15 GMT  
		Size: 26.7 MB (26688718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131f805ec7fd68d45a887e2ef82de61de0247b4eb934ab03b7c933650e854baa`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 35.4 KB (35369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322ed380e680a77f30528ba013e3a802a7b44948a0609c7d1d732dd46a9a310d`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac240b130982ad1c3ba3188abbf18ba4e54bdd9e504ce2d5c2eff6d3e86b8dd`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459101facad87c08bc7770f59f7ce58838101b487f08e56534d241b1637ea11f`  
		Last Modified: Wed, 17 Jun 2020 02:58:20 GMT  
		Size: 124.1 MB (124051844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6857d0fd3a7a85202dfef410b6aeccd5b91834aa1e619fe2dd7e37862bef843a`  
		Last Modified: Wed, 17 Jun 2020 03:03:15 GMT  
		Size: 345.2 MB (345167496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.1-bionic-slim`

```console
$ docker pull swift@sha256:c4146dea1cb982be993c2fda6d750a461f871fad47edd838910f2599ab529eca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.1-bionic-slim` - linux; amd64

```console
$ docker pull swift@sha256:725f6808874492ea1a1ad38c11c28196ddeb01abd41fa5c3c3eaa2655e1336d3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78279628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:550bb76939d0422ee624fac8bfc01e1c7426df1fc576670df9aa1237ab5434a4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:20:29 GMT
ADD file:1e8d02626176dc8141df3c0a1365774ce73d79934654fe24a4b1e7f173108232 in / 
# Wed, 17 Jun 2020 01:20:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:20:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:20:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:20:32 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:33:54 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:33:54 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 17 Jun 2020 02:33:55 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Wed, 17 Jun 2020 02:43:50 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Wed, 17 Jun 2020 02:43:50 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Wed, 17 Jun 2020 02:43:50 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:43:50 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:44:57 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl gnupg && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl gnupg
```

-	Layers:
	-	`sha256:d7c3167c320d7a820935f54cf4290890ea19567da496ecf774e8773b35d5f065`  
		Last Modified: Wed, 27 May 2020 12:21:15 GMT  
		Size: 26.7 MB (26688718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131f805ec7fd68d45a887e2ef82de61de0247b4eb934ab03b7c933650e854baa`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 35.4 KB (35369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322ed380e680a77f30528ba013e3a802a7b44948a0609c7d1d732dd46a9a310d`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac240b130982ad1c3ba3188abbf18ba4e54bdd9e504ce2d5c2eff6d3e86b8dd`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be976c7c6b240f9e676229be402cd77dde5ddbf2fd331b3bfa7b9ee1099456e`  
		Last Modified: Wed, 17 Jun 2020 03:00:32 GMT  
		Size: 20.5 MB (20471960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e00a5688786d8ce5a3479b38a3dda1581778276baadc4bfcf4018c80b6405f`  
		Last Modified: Wed, 17 Jun 2020 03:04:33 GMT  
		Size: 31.1 MB (31082574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.1-slim`

```console
$ docker pull swift@sha256:c4146dea1cb982be993c2fda6d750a461f871fad47edd838910f2599ab529eca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.1-slim` - linux; amd64

```console
$ docker pull swift@sha256:725f6808874492ea1a1ad38c11c28196ddeb01abd41fa5c3c3eaa2655e1336d3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78279628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:550bb76939d0422ee624fac8bfc01e1c7426df1fc576670df9aa1237ab5434a4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:20:29 GMT
ADD file:1e8d02626176dc8141df3c0a1365774ce73d79934654fe24a4b1e7f173108232 in / 
# Wed, 17 Jun 2020 01:20:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:20:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:20:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:20:32 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:33:54 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:33:54 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 17 Jun 2020 02:33:55 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Wed, 17 Jun 2020 02:43:50 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Wed, 17 Jun 2020 02:43:50 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Wed, 17 Jun 2020 02:43:50 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:43:50 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:44:57 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl gnupg && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl gnupg
```

-	Layers:
	-	`sha256:d7c3167c320d7a820935f54cf4290890ea19567da496ecf774e8773b35d5f065`  
		Last Modified: Wed, 27 May 2020 12:21:15 GMT  
		Size: 26.7 MB (26688718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131f805ec7fd68d45a887e2ef82de61de0247b4eb934ab03b7c933650e854baa`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 35.4 KB (35369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322ed380e680a77f30528ba013e3a802a7b44948a0609c7d1d732dd46a9a310d`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac240b130982ad1c3ba3188abbf18ba4e54bdd9e504ce2d5c2eff6d3e86b8dd`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be976c7c6b240f9e676229be402cd77dde5ddbf2fd331b3bfa7b9ee1099456e`  
		Last Modified: Wed, 17 Jun 2020 03:00:32 GMT  
		Size: 20.5 MB (20471960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e00a5688786d8ce5a3479b38a3dda1581778276baadc4bfcf4018c80b6405f`  
		Last Modified: Wed, 17 Jun 2020 03:04:33 GMT  
		Size: 31.1 MB (31082574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.1-xenial`

```console
$ docker pull swift@sha256:5fa5415ba0ce26adfbcb91746c836f9a46e5ee3f456dfcdb43d5f685dfbec7b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.1-xenial` - linux; amd64

```console
$ docker pull swift@sha256:b14699138c385daea671c2ffb4431356e23cb08bacfa280acab798b677f106c9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **507.3 MB (507331249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a4028b0bae9526420a01c8190d03606516e971184529352d018cf352542ac32`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:21:26 GMT
ADD file:52af30f80ba214985a59cb0ef7073c64f8514d58396c0de48f8d7056dec2a58a in / 
# Wed, 17 Jun 2020 01:21:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:21:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:21:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:30:50 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:30:51 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:31:47 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl3     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:31:47 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 17 Jun 2020 02:31:48 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Wed, 17 Jun 2020 02:42:17 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Wed, 17 Jun 2020 02:42:17 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Wed, 17 Jun 2020 02:42:17 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:42:17 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:43:35 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Wed, 17 Jun 2020 02:43:36 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:b5e173e44934e01d8d2674bc8b1da00f761c4fe796e0fb2bee1bd1129d2e4ae1`  
		Last Modified: Fri, 15 May 2020 13:20:22 GMT  
		Size: 44.3 MB (44320272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29047100b0407dff554ea80b8005380d62b13a66d7fe2e2adb07b9c091b9f2c0`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 531.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15743a713c2a4033877dab08fb3989280f8c856234227158a4011811c7991372`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6bc9e2987763aa991b7dfd742be04c7b3bb04448982ffe88e58d55c93b76d4`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11426dc469ff356e2be300a91a31d297702f5754f463aaa564ca00b9a37b1ea2`  
		Last Modified: Wed, 17 Jun 2020 02:59:31 GMT  
		Size: 111.5 MB (111534848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3729d059f49fdc753c1b0d3ceda2aca772e9a59f53c064c3d6d90d49993365a1`  
		Last Modified: Wed, 17 Jun 2020 03:04:22 GMT  
		Size: 351.5 MB (351474573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.1-xenial-slim`

```console
$ docker pull swift@sha256:24d792b53a59a3e312bc3c5382c3d5785cc09d1049621d272fc0c8ea87321176
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.1-xenial-slim` - linux; amd64

```console
$ docker pull swift@sha256:d7da6d34f0eb0f1e4957ef1f63abd385a5e897f7140f1c1fa05689810667a235
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.1 MB (96120187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4bcd36d3f681de6487aef094750f0b9bf19de448b6dbe0098e75e46e04ee880`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:21:26 GMT
ADD file:52af30f80ba214985a59cb0ef7073c64f8514d58396c0de48f8d7056dec2a58a in / 
# Wed, 17 Jun 2020 01:21:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:21:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:21:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:30:50 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:30:51 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:35:35 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl3     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:35:35 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 17 Jun 2020 02:35:36 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Wed, 17 Jun 2020 02:45:03 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Wed, 17 Jun 2020 02:45:03 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Wed, 17 Jun 2020 02:45:03 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:45:04 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:46:08 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
```

-	Layers:
	-	`sha256:b5e173e44934e01d8d2674bc8b1da00f761c4fe796e0fb2bee1bd1129d2e4ae1`  
		Last Modified: Fri, 15 May 2020 13:20:22 GMT  
		Size: 44.3 MB (44320272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29047100b0407dff554ea80b8005380d62b13a66d7fe2e2adb07b9c091b9f2c0`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 531.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15743a713c2a4033877dab08fb3989280f8c856234227158a4011811c7991372`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6bc9e2987763aa991b7dfd742be04c7b3bb04448982ffe88e58d55c93b76d4`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da1f8178404835f2182a23ff9eb65d65ff3015da8d71433f43db492410a3129d`  
		Last Modified: Wed, 17 Jun 2020 03:00:45 GMT  
		Size: 20.8 MB (20845087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6debc65f38c536ec4c3ca49ba47b7482b005ba87d60f1f8539e02d0a7fd4745`  
		Last Modified: Wed, 17 Jun 2020 03:04:48 GMT  
		Size: 31.0 MB (30953272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.2`

```console
$ docker pull swift@sha256:b1e98d1807bd6df4a7b8431d0ddb0a2ed5f9ce119d0db113451dd30e5d57740c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.2` - linux; amd64

```console
$ docker pull swift@sha256:087c8e19d8b53e3442f6ebbd1c2d4bac57098ddcff3b3db12fc38572cb82b75c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **537.5 MB (537509085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bef395c099c7e6e27dd068ba2e66d6bf929e31e5c1c44c216629e3a5de39fcb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:20:29 GMT
ADD file:1e8d02626176dc8141df3c0a1365774ce73d79934654fe24a4b1e7f173108232 in / 
# Wed, 17 Jun 2020 01:20:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:20:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:20:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:20:32 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:29:10 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:29:10 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 17 Jun 2020 02:29:11 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Wed, 17 Jun 2020 02:29:11 GMT
ARG SWIFT_BRANCH=swift-5.2.4-release
# Wed, 17 Jun 2020 02:29:12 GMT
ARG SWIFT_VERSION=swift-5.2.4-RELEASE
# Wed, 17 Jun 2020 02:29:12 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:29:12 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.2.4-release SWIFT_VERSION=swift-5.2.4-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:30:41 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Wed, 17 Jun 2020 02:30:43 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:d7c3167c320d7a820935f54cf4290890ea19567da496ecf774e8773b35d5f065`  
		Last Modified: Wed, 27 May 2020 12:21:15 GMT  
		Size: 26.7 MB (26688718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131f805ec7fd68d45a887e2ef82de61de0247b4eb934ab03b7c933650e854baa`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 35.4 KB (35369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322ed380e680a77f30528ba013e3a802a7b44948a0609c7d1d732dd46a9a310d`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac240b130982ad1c3ba3188abbf18ba4e54bdd9e504ce2d5c2eff6d3e86b8dd`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459101facad87c08bc7770f59f7ce58838101b487f08e56534d241b1637ea11f`  
		Last Modified: Wed, 17 Jun 2020 02:58:20 GMT  
		Size: 124.1 MB (124051844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1061d32da7815faf492e182f868761c28abd0fbc6abcf84bc52c29b7d396bf`  
		Last Modified: Wed, 17 Jun 2020 02:59:01 GMT  
		Size: 386.7 MB (386732147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.2.4`

```console
$ docker pull swift@sha256:b1e98d1807bd6df4a7b8431d0ddb0a2ed5f9ce119d0db113451dd30e5d57740c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.2.4` - linux; amd64

```console
$ docker pull swift@sha256:087c8e19d8b53e3442f6ebbd1c2d4bac57098ddcff3b3db12fc38572cb82b75c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **537.5 MB (537509085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bef395c099c7e6e27dd068ba2e66d6bf929e31e5c1c44c216629e3a5de39fcb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:20:29 GMT
ADD file:1e8d02626176dc8141df3c0a1365774ce73d79934654fe24a4b1e7f173108232 in / 
# Wed, 17 Jun 2020 01:20:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:20:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:20:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:20:32 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:29:10 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:29:10 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 17 Jun 2020 02:29:11 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Wed, 17 Jun 2020 02:29:11 GMT
ARG SWIFT_BRANCH=swift-5.2.4-release
# Wed, 17 Jun 2020 02:29:12 GMT
ARG SWIFT_VERSION=swift-5.2.4-RELEASE
# Wed, 17 Jun 2020 02:29:12 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:29:12 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.2.4-release SWIFT_VERSION=swift-5.2.4-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:30:41 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Wed, 17 Jun 2020 02:30:43 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:d7c3167c320d7a820935f54cf4290890ea19567da496ecf774e8773b35d5f065`  
		Last Modified: Wed, 27 May 2020 12:21:15 GMT  
		Size: 26.7 MB (26688718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131f805ec7fd68d45a887e2ef82de61de0247b4eb934ab03b7c933650e854baa`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 35.4 KB (35369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322ed380e680a77f30528ba013e3a802a7b44948a0609c7d1d732dd46a9a310d`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac240b130982ad1c3ba3188abbf18ba4e54bdd9e504ce2d5c2eff6d3e86b8dd`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459101facad87c08bc7770f59f7ce58838101b487f08e56534d241b1637ea11f`  
		Last Modified: Wed, 17 Jun 2020 02:58:20 GMT  
		Size: 124.1 MB (124051844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1061d32da7815faf492e182f868761c28abd0fbc6abcf84bc52c29b7d396bf`  
		Last Modified: Wed, 17 Jun 2020 02:59:01 GMT  
		Size: 386.7 MB (386732147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.2.4-amazonlinux2`

```console
$ docker pull swift@sha256:223ea1eefa3f0dfecd195fd29e6f4f098d8ac4a77eaf16eff779044a4184c999
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.2.4-amazonlinux2` - linux; amd64

```console
$ docker pull swift@sha256:2d30f58a12d1cb089a2f788bb35aa100c786b3b8ae5efda45e993d708a427893
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **685.0 MB (685037474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f19e4f405c699a3280d7c63980f8f99c4b66e3c641c8ceaaf15b153acc614aba`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Jun 2020 20:20:04 GMT
ADD file:788af9048b1c163347d7a8349f8ecf5721b4d8b63395ec8c6ca6d0732f57acdd in / 
# Tue, 30 Jun 2020 20:20:05 GMT
CMD ["/bin/bash"]
# Tue, 30 Jun 2020 20:57:47 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Tue, 30 Jun 2020 20:57:47 GMT
LABEL description=Docker Container for the Swift programming language
# Tue, 30 Jun 2020 21:00:01 GMT
RUN yum -y update && yum -y install   binutils   gcc   git   glibc-static   gzip   libbsd   libcurl   libedit   libicu   libsqlite   libstdc++-static   libuuid   libxml2   tar   tzdata   zlib-devel
# Tue, 30 Jun 2020 21:00:02 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Tue, 30 Jun 2020 21:00:02 GMT
ARG SWIFT_PLATFORM=amazonlinux2
# Tue, 30 Jun 2020 21:00:02 GMT
ARG SWIFT_BRANCH=swift-5.2.4-release
# Tue, 30 Jun 2020 21:00:02 GMT
ARG SWIFT_VERSION=swift-5.2.4-RELEASE
# Tue, 30 Jun 2020 21:00:02 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Tue, 30 Jun 2020 21:00:03 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=amazonlinux2 SWIFT_BRANCH=swift-5.2.4-release SWIFT_VERSION=swift-5.2.4-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Tue, 30 Jun 2020 21:01:32 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz
# Tue, 30 Jun 2020 21:01:33 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:3d24604292f287c31563b1f563e83307e7915909506659401fb07c1c3e6e164c`  
		Last Modified: Tue, 30 Jun 2020 20:21:31 GMT  
		Size: 61.7 MB (61684682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea50e5b47eb33e6b56eb394bef851b8cbe7627ceb40460d4f3d654fcbb0a676`  
		Last Modified: Tue, 30 Jun 2020 21:04:44 GMT  
		Size: 234.4 MB (234382905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec95769a775463f018621e30a9b7bce62c5db31569f165e7162c5f67216dd938`  
		Last Modified: Tue, 30 Jun 2020 21:05:36 GMT  
		Size: 389.0 MB (388969887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.2.4-bionic`

```console
$ docker pull swift@sha256:b1e98d1807bd6df4a7b8431d0ddb0a2ed5f9ce119d0db113451dd30e5d57740c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.2.4-bionic` - linux; amd64

```console
$ docker pull swift@sha256:087c8e19d8b53e3442f6ebbd1c2d4bac57098ddcff3b3db12fc38572cb82b75c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **537.5 MB (537509085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bef395c099c7e6e27dd068ba2e66d6bf929e31e5c1c44c216629e3a5de39fcb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:20:29 GMT
ADD file:1e8d02626176dc8141df3c0a1365774ce73d79934654fe24a4b1e7f173108232 in / 
# Wed, 17 Jun 2020 01:20:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:20:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:20:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:20:32 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:29:10 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:29:10 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 17 Jun 2020 02:29:11 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Wed, 17 Jun 2020 02:29:11 GMT
ARG SWIFT_BRANCH=swift-5.2.4-release
# Wed, 17 Jun 2020 02:29:12 GMT
ARG SWIFT_VERSION=swift-5.2.4-RELEASE
# Wed, 17 Jun 2020 02:29:12 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:29:12 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.2.4-release SWIFT_VERSION=swift-5.2.4-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:30:41 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Wed, 17 Jun 2020 02:30:43 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:d7c3167c320d7a820935f54cf4290890ea19567da496ecf774e8773b35d5f065`  
		Last Modified: Wed, 27 May 2020 12:21:15 GMT  
		Size: 26.7 MB (26688718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131f805ec7fd68d45a887e2ef82de61de0247b4eb934ab03b7c933650e854baa`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 35.4 KB (35369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322ed380e680a77f30528ba013e3a802a7b44948a0609c7d1d732dd46a9a310d`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac240b130982ad1c3ba3188abbf18ba4e54bdd9e504ce2d5c2eff6d3e86b8dd`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459101facad87c08bc7770f59f7ce58838101b487f08e56534d241b1637ea11f`  
		Last Modified: Wed, 17 Jun 2020 02:58:20 GMT  
		Size: 124.1 MB (124051844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1061d32da7815faf492e182f868761c28abd0fbc6abcf84bc52c29b7d396bf`  
		Last Modified: Wed, 17 Jun 2020 02:59:01 GMT  
		Size: 386.7 MB (386732147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.2.4-bionic-slim`

```console
$ docker pull swift@sha256:6be4635b0b8b3708a3ae8b6c9c30371283a513c25f3e8f6aa6af03803f60ee13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.2.4-bionic-slim` - linux; amd64

```console
$ docker pull swift@sha256:e1f25d8ce666f4a4205f6264f05f12d0cab03323126a50067e7e8ccb739e0984
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79656583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6feb0c96ff84c71e02cb5f7a45bdc3df7606cea92f2c576b6ea1dc1efa92b833`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:20:29 GMT
ADD file:1e8d02626176dc8141df3c0a1365774ce73d79934654fe24a4b1e7f173108232 in / 
# Wed, 17 Jun 2020 01:20:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:20:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:20:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:20:32 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:33:54 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:33:54 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 17 Jun 2020 02:33:55 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Wed, 17 Jun 2020 02:33:55 GMT
ARG SWIFT_BRANCH=swift-5.2.4-release
# Wed, 17 Jun 2020 02:33:55 GMT
ARG SWIFT_VERSION=swift-5.2.4-RELEASE
# Wed, 17 Jun 2020 02:33:56 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:33:56 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.2.4-release SWIFT_VERSION=swift-5.2.4-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:35:12 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl gnupg && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl gnupg
```

-	Layers:
	-	`sha256:d7c3167c320d7a820935f54cf4290890ea19567da496ecf774e8773b35d5f065`  
		Last Modified: Wed, 27 May 2020 12:21:15 GMT  
		Size: 26.7 MB (26688718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131f805ec7fd68d45a887e2ef82de61de0247b4eb934ab03b7c933650e854baa`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 35.4 KB (35369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322ed380e680a77f30528ba013e3a802a7b44948a0609c7d1d732dd46a9a310d`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac240b130982ad1c3ba3188abbf18ba4e54bdd9e504ce2d5c2eff6d3e86b8dd`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be976c7c6b240f9e676229be402cd77dde5ddbf2fd331b3bfa7b9ee1099456e`  
		Last Modified: Wed, 17 Jun 2020 03:00:32 GMT  
		Size: 20.5 MB (20471960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8286c2d75be4187ec9a12110bdc196beaed37a383866af8009ab333012a17a37`  
		Last Modified: Wed, 17 Jun 2020 03:00:33 GMT  
		Size: 32.5 MB (32459529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.2.4-centos8`

```console
$ docker pull swift@sha256:6343f107c590e305973893809591cd6ea3ed31cbdaa996dce36dcc9787b382b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.2.4-centos8` - linux; amd64

```console
$ docker pull swift@sha256:209d86ff24e0843b84c683840df6a1aec9788a2b7e6675ca452c051a9b84d22c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **628.3 MB (628290894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3678c629101e3b6c922738049111e92c8fa40d10a322d4625aeac7f1a17b3762`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 00:22:24 GMT
ADD file:84700c11fcc969ac08ef25f115513d76c7b72a4118c01fbc86ef0a6056fdebeb in / 
# Wed, 17 Jun 2020 00:22:25 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200611
# Wed, 17 Jun 2020 00:22:25 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 00:46:24 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 00:46:24 GMT
LABEL description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 00:46:29 GMT
RUN yum install -y https://dl.fedoraproject.org/pub/epel/epel-release-latest-8.noarch.rpm
# Wed, 17 Jun 2020 00:47:01 GMT
RUN yum -y update && yum install --enablerepo=PowerTools -y   binutils   gcc   git   glibc-static   libbsd-devel   libedit   libedit-devel   libicu-devel   libstdc++-static   pkg-config   python2   sqlite   zlib-devel
# Wed, 17 Jun 2020 00:47:02 GMT
RUN ln -s /usr/bin/python2 /usr/bin/python
# Wed, 17 Jun 2020 00:47:02 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 17 Jun 2020 00:47:02 GMT
ARG SWIFT_PLATFORM=centos8
# Wed, 17 Jun 2020 00:47:03 GMT
ARG SWIFT_BRANCH=swift-5.2.4-release
# Wed, 17 Jun 2020 00:47:03 GMT
ARG SWIFT_VERSION=swift-5.2.4-RELEASE
# Wed, 17 Jun 2020 00:47:03 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 00:47:03 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=centos8 SWIFT_BRANCH=swift-5.2.4-release SWIFT_VERSION=swift-5.2.4-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 00:48:20 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz
# Wed, 17 Jun 2020 00:48:22 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:6910e5a164f725142d77994b247ba20040477fbab49a721bdbe8d61cf855ac23`  
		Last Modified: Wed, 17 Jun 2020 00:23:52 GMT  
		Size: 74.9 MB (74866818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25c5181aa902d0b68a772ff8e20440647e871f794439c373f247e767e6eda27`  
		Last Modified: Wed, 17 Jun 2020 00:49:44 GMT  
		Size: 18.4 MB (18386404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a75d228738821afda2ed880b6196234987ea752ed7c0ac05d6ae66217a976d7`  
		Last Modified: Wed, 17 Jun 2020 00:50:09 GMT  
		Size: 146.7 MB (146701694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f4f2ea37f9d8633debbd6c006f56912bb9b0df660c0e63bd3d5fc46b76b478`  
		Last Modified: Wed, 17 Jun 2020 00:49:42 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd08af79dd11a734b52c6712cbbf524b0ed1b8905ea7c6561a7cf87628b35566`  
		Last Modified: Wed, 17 Jun 2020 00:50:58 GMT  
		Size: 388.3 MB (388335825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.2.4-focal`

```console
$ docker pull swift@sha256:a958e3eb9c1041f280a42e5a5b026f519f62150dd87469fbc10d9f21700d14da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.2.4-focal` - linux; amd64

```console
$ docker pull swift@sha256:cb3959bdf578d26f7f3a4c1e510f398aa9c239ad0cc6fd652be5ebbf94994e10
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **509.0 MB (509035668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48809fb5ee4c86af95d0ac0143f4015c0ec32ca66332fc0c7fbd3dae190e142e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:20:53 GMT
ADD file:b2342c7e6665d5ff3850d4f04e2521d1851eb2054f9a8d56fcf4e7c314b9f20e in / 
# Wed, 17 Jun 2020 01:20:54 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:20:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:20:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:20:56 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:37:08 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:37:08 GMT
LABEL description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:39:10 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     binutils     git     gnupg2     libc6-dev     libcurl4     libedit2     libgcc-9-dev     libpython2.7     libsqlite3-0     libstdc++-9-dev     libxml2     libz3-dev     pkg-config     tzdata     zlib1g-dev     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:39:10 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 17 Jun 2020 02:39:11 GMT
ARG SWIFT_PLATFORM=ubuntu20.04
# Wed, 17 Jun 2020 02:39:11 GMT
ARG SWIFT_BRANCH=swift-5.2.4-release
# Wed, 17 Jun 2020 02:39:11 GMT
ARG SWIFT_VERSION=swift-5.2.4-RELEASE
# Wed, 17 Jun 2020 02:39:11 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:39:11 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu20.04 SWIFT_BRANCH=swift-5.2.4-release SWIFT_VERSION=swift-5.2.4-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:40:31 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Wed, 17 Jun 2020 02:40:33 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:a4a2a29f9ba48efd3d2075f395538b2eec56fb1bedfb7aecf5e54174446f9e2a`  
		Last Modified: Sat, 06 Jun 2020 15:19:59 GMT  
		Size: 28.6 MB (28556492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127c9761dcbaa288abc58fc56437c2f2ffbe611b9f7f30e0b5b43cd348bb2094`  
		Last Modified: Wed, 17 Jun 2020 01:22:02 GMT  
		Size: 32.3 KB (32317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13bf203e905463e64d89b14509aafa983fb8baf7c1931fe0a65652aeb6c838f`  
		Last Modified: Wed, 17 Jun 2020 01:22:01 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4039240d2e0b4bcb42ccbce75bc54570e471ad81457478de35fbeef63536e9c0`  
		Last Modified: Wed, 17 Jun 2020 01:22:02 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b80c06486cbec0481f48d39da79eacaf873f3c3c4427e7e8207a3823a2edaf`  
		Last Modified: Wed, 17 Jun 2020 03:01:26 GMT  
		Size: 93.6 MB (93569449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cf548f128817483083eecb82910c032f5ba0e2131fbb62fe308de466244849`  
		Last Modified: Wed, 17 Jun 2020 03:02:12 GMT  
		Size: 386.9 MB (386876405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.2.4-focal-slim`

```console
$ docker pull swift@sha256:db4dc7ea4b23dd19d412dfc53ea4a41398ebab18e67911e55734cacf4e0e2057
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.2.4-focal-slim` - linux; amd64

```console
$ docker pull swift@sha256:808a617b894f102c4eb7b5c1bb88ae2c677e1eb6e29274638d88fa865417e9f5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.3 MB (83298389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92095e8734294fb793dd79492fbf1722ae8d8f8abd440121bd1053373f172754`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:20:53 GMT
ADD file:b2342c7e6665d5ff3850d4f04e2521d1851eb2054f9a8d56fcf4e7c314b9f20e in / 
# Wed, 17 Jun 2020 01:20:54 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:20:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:20:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:20:56 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:37:08 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:37:08 GMT
LABEL description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:37:20 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:37:20 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 17 Jun 2020 02:37:20 GMT
ARG SWIFT_PLATFORM=ubuntu20.04
# Wed, 17 Jun 2020 02:37:20 GMT
ARG SWIFT_BRANCH=swift-5.2.4-release
# Wed, 17 Jun 2020 02:37:21 GMT
ARG SWIFT_VERSION=swift-5.2.4-RELEASE
# Wed, 17 Jun 2020 02:37:21 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:37:21 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu20.04 SWIFT_BRANCH=swift-5.2.4-release SWIFT_VERSION=swift-5.2.4-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:38:33 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl gnupg && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl gnupg
```

-	Layers:
	-	`sha256:a4a2a29f9ba48efd3d2075f395538b2eec56fb1bedfb7aecf5e54174446f9e2a`  
		Last Modified: Sat, 06 Jun 2020 15:19:59 GMT  
		Size: 28.6 MB (28556492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127c9761dcbaa288abc58fc56437c2f2ffbe611b9f7f30e0b5b43cd348bb2094`  
		Last Modified: Wed, 17 Jun 2020 01:22:02 GMT  
		Size: 32.3 KB (32317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13bf203e905463e64d89b14509aafa983fb8baf7c1931fe0a65652aeb6c838f`  
		Last Modified: Wed, 17 Jun 2020 01:22:01 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4039240d2e0b4bcb42ccbce75bc54570e471ad81457478de35fbeef63536e9c0`  
		Last Modified: Wed, 17 Jun 2020 01:22:02 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd287c1f1dc0268bbff81424af64f947ec7ce2ac383a579ddb0f687cf73df67a`  
		Last Modified: Wed, 17 Jun 2020 03:00:57 GMT  
		Size: 22.2 MB (22241328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c2c728627fbd9713ebca4f546a7cb38fdcdbcda29b3e71980135ba0e0feac4`  
		Last Modified: Wed, 17 Jun 2020 03:00:58 GMT  
		Size: 32.5 MB (32467247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.2.4-slim`

```console
$ docker pull swift@sha256:6be4635b0b8b3708a3ae8b6c9c30371283a513c25f3e8f6aa6af03803f60ee13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.2.4-slim` - linux; amd64

```console
$ docker pull swift@sha256:e1f25d8ce666f4a4205f6264f05f12d0cab03323126a50067e7e8ccb739e0984
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79656583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6feb0c96ff84c71e02cb5f7a45bdc3df7606cea92f2c576b6ea1dc1efa92b833`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:20:29 GMT
ADD file:1e8d02626176dc8141df3c0a1365774ce73d79934654fe24a4b1e7f173108232 in / 
# Wed, 17 Jun 2020 01:20:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:20:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:20:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:20:32 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:33:54 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:33:54 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 17 Jun 2020 02:33:55 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Wed, 17 Jun 2020 02:33:55 GMT
ARG SWIFT_BRANCH=swift-5.2.4-release
# Wed, 17 Jun 2020 02:33:55 GMT
ARG SWIFT_VERSION=swift-5.2.4-RELEASE
# Wed, 17 Jun 2020 02:33:56 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:33:56 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.2.4-release SWIFT_VERSION=swift-5.2.4-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:35:12 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl gnupg && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl gnupg
```

-	Layers:
	-	`sha256:d7c3167c320d7a820935f54cf4290890ea19567da496ecf774e8773b35d5f065`  
		Last Modified: Wed, 27 May 2020 12:21:15 GMT  
		Size: 26.7 MB (26688718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131f805ec7fd68d45a887e2ef82de61de0247b4eb934ab03b7c933650e854baa`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 35.4 KB (35369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322ed380e680a77f30528ba013e3a802a7b44948a0609c7d1d732dd46a9a310d`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac240b130982ad1c3ba3188abbf18ba4e54bdd9e504ce2d5c2eff6d3e86b8dd`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be976c7c6b240f9e676229be402cd77dde5ddbf2fd331b3bfa7b9ee1099456e`  
		Last Modified: Wed, 17 Jun 2020 03:00:32 GMT  
		Size: 20.5 MB (20471960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8286c2d75be4187ec9a12110bdc196beaed37a383866af8009ab333012a17a37`  
		Last Modified: Wed, 17 Jun 2020 03:00:33 GMT  
		Size: 32.5 MB (32459529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.2.4-xenial`

```console
$ docker pull swift@sha256:e5d21afd43717807a9df19dfc0fa7859899894460a18ffb36240de0112580e18
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.2.4-xenial` - linux; amd64

```console
$ docker pull swift@sha256:692333469a7fc90442ed6165c9de9ce7b9de4c6ea60d4c8248db7f38c9fe4167
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **549.6 MB (549629701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2480ab93016ba0ca44bc7dda935d209946c06b39e0d1f95c8a6fbc7a7cb19f95`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:21:26 GMT
ADD file:52af30f80ba214985a59cb0ef7073c64f8514d58396c0de48f8d7056dec2a58a in / 
# Wed, 17 Jun 2020 01:21:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:21:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:21:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:30:50 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:30:51 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:31:47 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl3     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:31:47 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 17 Jun 2020 02:31:48 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Wed, 17 Jun 2020 02:31:48 GMT
ARG SWIFT_BRANCH=swift-5.2.4-release
# Wed, 17 Jun 2020 02:31:48 GMT
ARG SWIFT_VERSION=swift-5.2.4-RELEASE
# Wed, 17 Jun 2020 02:31:49 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:31:49 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-5.2.4-release SWIFT_VERSION=swift-5.2.4-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:33:20 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Wed, 17 Jun 2020 02:33:22 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:b5e173e44934e01d8d2674bc8b1da00f761c4fe796e0fb2bee1bd1129d2e4ae1`  
		Last Modified: Fri, 15 May 2020 13:20:22 GMT  
		Size: 44.3 MB (44320272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29047100b0407dff554ea80b8005380d62b13a66d7fe2e2adb07b9c091b9f2c0`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 531.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15743a713c2a4033877dab08fb3989280f8c856234227158a4011811c7991372`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6bc9e2987763aa991b7dfd742be04c7b3bb04448982ffe88e58d55c93b76d4`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11426dc469ff356e2be300a91a31d297702f5754f463aaa564ca00b9a37b1ea2`  
		Last Modified: Wed, 17 Jun 2020 02:59:31 GMT  
		Size: 111.5 MB (111534848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba73bfd6b863e49120e0da4ead85b0017b6c8c8389746dbc1ff26bfc02524b9`  
		Last Modified: Wed, 17 Jun 2020 03:00:17 GMT  
		Size: 393.8 MB (393773025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.2.4-xenial-slim`

```console
$ docker pull swift@sha256:4c6a9e0f040e42a94f0fc63d99d0a6a652f2a1371e73cd5b560a8ae82a4cef48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.2.4-xenial-slim` - linux; amd64

```console
$ docker pull swift@sha256:77af1fb0305217aaa904a20c4266bb37465ae9ed3e18dae70ca48f3191a638b3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.5 MB (97538700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c756b51ad5ff62a291e5d1911ecc48634d899d1bde88ff69f8ddbabdb6c91238`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:21:26 GMT
ADD file:52af30f80ba214985a59cb0ef7073c64f8514d58396c0de48f8d7056dec2a58a in / 
# Wed, 17 Jun 2020 01:21:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:21:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:21:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:30:50 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:30:51 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:35:35 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl3     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:35:35 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 17 Jun 2020 02:35:36 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Wed, 17 Jun 2020 02:35:36 GMT
ARG SWIFT_BRANCH=swift-5.2.4-release
# Wed, 17 Jun 2020 02:35:36 GMT
ARG SWIFT_VERSION=swift-5.2.4-RELEASE
# Wed, 17 Jun 2020 02:35:36 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:35:37 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-5.2.4-release SWIFT_VERSION=swift-5.2.4-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:36:50 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
```

-	Layers:
	-	`sha256:b5e173e44934e01d8d2674bc8b1da00f761c4fe796e0fb2bee1bd1129d2e4ae1`  
		Last Modified: Fri, 15 May 2020 13:20:22 GMT  
		Size: 44.3 MB (44320272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29047100b0407dff554ea80b8005380d62b13a66d7fe2e2adb07b9c091b9f2c0`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 531.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15743a713c2a4033877dab08fb3989280f8c856234227158a4011811c7991372`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6bc9e2987763aa991b7dfd742be04c7b3bb04448982ffe88e58d55c93b76d4`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da1f8178404835f2182a23ff9eb65d65ff3015da8d71433f43db492410a3129d`  
		Last Modified: Wed, 17 Jun 2020 03:00:45 GMT  
		Size: 20.8 MB (20845087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a2dadc5cb2bea665f3846de4ac7f09e7458df26fcd0ff3befbc73a28528e3b2`  
		Last Modified: Wed, 17 Jun 2020 03:00:46 GMT  
		Size: 32.4 MB (32371785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.2-amazonlinux2`

```console
$ docker pull swift@sha256:223ea1eefa3f0dfecd195fd29e6f4f098d8ac4a77eaf16eff779044a4184c999
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.2-amazonlinux2` - linux; amd64

```console
$ docker pull swift@sha256:2d30f58a12d1cb089a2f788bb35aa100c786b3b8ae5efda45e993d708a427893
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **685.0 MB (685037474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f19e4f405c699a3280d7c63980f8f99c4b66e3c641c8ceaaf15b153acc614aba`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Jun 2020 20:20:04 GMT
ADD file:788af9048b1c163347d7a8349f8ecf5721b4d8b63395ec8c6ca6d0732f57acdd in / 
# Tue, 30 Jun 2020 20:20:05 GMT
CMD ["/bin/bash"]
# Tue, 30 Jun 2020 20:57:47 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Tue, 30 Jun 2020 20:57:47 GMT
LABEL description=Docker Container for the Swift programming language
# Tue, 30 Jun 2020 21:00:01 GMT
RUN yum -y update && yum -y install   binutils   gcc   git   glibc-static   gzip   libbsd   libcurl   libedit   libicu   libsqlite   libstdc++-static   libuuid   libxml2   tar   tzdata   zlib-devel
# Tue, 30 Jun 2020 21:00:02 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Tue, 30 Jun 2020 21:00:02 GMT
ARG SWIFT_PLATFORM=amazonlinux2
# Tue, 30 Jun 2020 21:00:02 GMT
ARG SWIFT_BRANCH=swift-5.2.4-release
# Tue, 30 Jun 2020 21:00:02 GMT
ARG SWIFT_VERSION=swift-5.2.4-RELEASE
# Tue, 30 Jun 2020 21:00:02 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Tue, 30 Jun 2020 21:00:03 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=amazonlinux2 SWIFT_BRANCH=swift-5.2.4-release SWIFT_VERSION=swift-5.2.4-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Tue, 30 Jun 2020 21:01:32 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz
# Tue, 30 Jun 2020 21:01:33 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:3d24604292f287c31563b1f563e83307e7915909506659401fb07c1c3e6e164c`  
		Last Modified: Tue, 30 Jun 2020 20:21:31 GMT  
		Size: 61.7 MB (61684682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea50e5b47eb33e6b56eb394bef851b8cbe7627ceb40460d4f3d654fcbb0a676`  
		Last Modified: Tue, 30 Jun 2020 21:04:44 GMT  
		Size: 234.4 MB (234382905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec95769a775463f018621e30a9b7bce62c5db31569f165e7162c5f67216dd938`  
		Last Modified: Tue, 30 Jun 2020 21:05:36 GMT  
		Size: 389.0 MB (388969887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.2-bionic`

```console
$ docker pull swift@sha256:b1e98d1807bd6df4a7b8431d0ddb0a2ed5f9ce119d0db113451dd30e5d57740c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.2-bionic` - linux; amd64

```console
$ docker pull swift@sha256:087c8e19d8b53e3442f6ebbd1c2d4bac57098ddcff3b3db12fc38572cb82b75c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **537.5 MB (537509085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bef395c099c7e6e27dd068ba2e66d6bf929e31e5c1c44c216629e3a5de39fcb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:20:29 GMT
ADD file:1e8d02626176dc8141df3c0a1365774ce73d79934654fe24a4b1e7f173108232 in / 
# Wed, 17 Jun 2020 01:20:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:20:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:20:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:20:32 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:29:10 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:29:10 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 17 Jun 2020 02:29:11 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Wed, 17 Jun 2020 02:29:11 GMT
ARG SWIFT_BRANCH=swift-5.2.4-release
# Wed, 17 Jun 2020 02:29:12 GMT
ARG SWIFT_VERSION=swift-5.2.4-RELEASE
# Wed, 17 Jun 2020 02:29:12 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:29:12 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.2.4-release SWIFT_VERSION=swift-5.2.4-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:30:41 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Wed, 17 Jun 2020 02:30:43 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:d7c3167c320d7a820935f54cf4290890ea19567da496ecf774e8773b35d5f065`  
		Last Modified: Wed, 27 May 2020 12:21:15 GMT  
		Size: 26.7 MB (26688718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131f805ec7fd68d45a887e2ef82de61de0247b4eb934ab03b7c933650e854baa`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 35.4 KB (35369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322ed380e680a77f30528ba013e3a802a7b44948a0609c7d1d732dd46a9a310d`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac240b130982ad1c3ba3188abbf18ba4e54bdd9e504ce2d5c2eff6d3e86b8dd`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459101facad87c08bc7770f59f7ce58838101b487f08e56534d241b1637ea11f`  
		Last Modified: Wed, 17 Jun 2020 02:58:20 GMT  
		Size: 124.1 MB (124051844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1061d32da7815faf492e182f868761c28abd0fbc6abcf84bc52c29b7d396bf`  
		Last Modified: Wed, 17 Jun 2020 02:59:01 GMT  
		Size: 386.7 MB (386732147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.2-bionic-slim`

```console
$ docker pull swift@sha256:6be4635b0b8b3708a3ae8b6c9c30371283a513c25f3e8f6aa6af03803f60ee13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.2-bionic-slim` - linux; amd64

```console
$ docker pull swift@sha256:e1f25d8ce666f4a4205f6264f05f12d0cab03323126a50067e7e8ccb739e0984
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79656583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6feb0c96ff84c71e02cb5f7a45bdc3df7606cea92f2c576b6ea1dc1efa92b833`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:20:29 GMT
ADD file:1e8d02626176dc8141df3c0a1365774ce73d79934654fe24a4b1e7f173108232 in / 
# Wed, 17 Jun 2020 01:20:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:20:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:20:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:20:32 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:33:54 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:33:54 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 17 Jun 2020 02:33:55 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Wed, 17 Jun 2020 02:33:55 GMT
ARG SWIFT_BRANCH=swift-5.2.4-release
# Wed, 17 Jun 2020 02:33:55 GMT
ARG SWIFT_VERSION=swift-5.2.4-RELEASE
# Wed, 17 Jun 2020 02:33:56 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:33:56 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.2.4-release SWIFT_VERSION=swift-5.2.4-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:35:12 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl gnupg && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl gnupg
```

-	Layers:
	-	`sha256:d7c3167c320d7a820935f54cf4290890ea19567da496ecf774e8773b35d5f065`  
		Last Modified: Wed, 27 May 2020 12:21:15 GMT  
		Size: 26.7 MB (26688718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131f805ec7fd68d45a887e2ef82de61de0247b4eb934ab03b7c933650e854baa`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 35.4 KB (35369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322ed380e680a77f30528ba013e3a802a7b44948a0609c7d1d732dd46a9a310d`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac240b130982ad1c3ba3188abbf18ba4e54bdd9e504ce2d5c2eff6d3e86b8dd`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be976c7c6b240f9e676229be402cd77dde5ddbf2fd331b3bfa7b9ee1099456e`  
		Last Modified: Wed, 17 Jun 2020 03:00:32 GMT  
		Size: 20.5 MB (20471960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8286c2d75be4187ec9a12110bdc196beaed37a383866af8009ab333012a17a37`  
		Last Modified: Wed, 17 Jun 2020 03:00:33 GMT  
		Size: 32.5 MB (32459529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.2-centos8`

```console
$ docker pull swift@sha256:6343f107c590e305973893809591cd6ea3ed31cbdaa996dce36dcc9787b382b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.2-centos8` - linux; amd64

```console
$ docker pull swift@sha256:209d86ff24e0843b84c683840df6a1aec9788a2b7e6675ca452c051a9b84d22c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **628.3 MB (628290894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3678c629101e3b6c922738049111e92c8fa40d10a322d4625aeac7f1a17b3762`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 00:22:24 GMT
ADD file:84700c11fcc969ac08ef25f115513d76c7b72a4118c01fbc86ef0a6056fdebeb in / 
# Wed, 17 Jun 2020 00:22:25 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200611
# Wed, 17 Jun 2020 00:22:25 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 00:46:24 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 00:46:24 GMT
LABEL description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 00:46:29 GMT
RUN yum install -y https://dl.fedoraproject.org/pub/epel/epel-release-latest-8.noarch.rpm
# Wed, 17 Jun 2020 00:47:01 GMT
RUN yum -y update && yum install --enablerepo=PowerTools -y   binutils   gcc   git   glibc-static   libbsd-devel   libedit   libedit-devel   libicu-devel   libstdc++-static   pkg-config   python2   sqlite   zlib-devel
# Wed, 17 Jun 2020 00:47:02 GMT
RUN ln -s /usr/bin/python2 /usr/bin/python
# Wed, 17 Jun 2020 00:47:02 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 17 Jun 2020 00:47:02 GMT
ARG SWIFT_PLATFORM=centos8
# Wed, 17 Jun 2020 00:47:03 GMT
ARG SWIFT_BRANCH=swift-5.2.4-release
# Wed, 17 Jun 2020 00:47:03 GMT
ARG SWIFT_VERSION=swift-5.2.4-RELEASE
# Wed, 17 Jun 2020 00:47:03 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 00:47:03 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=centos8 SWIFT_BRANCH=swift-5.2.4-release SWIFT_VERSION=swift-5.2.4-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 00:48:20 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz
# Wed, 17 Jun 2020 00:48:22 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:6910e5a164f725142d77994b247ba20040477fbab49a721bdbe8d61cf855ac23`  
		Last Modified: Wed, 17 Jun 2020 00:23:52 GMT  
		Size: 74.9 MB (74866818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25c5181aa902d0b68a772ff8e20440647e871f794439c373f247e767e6eda27`  
		Last Modified: Wed, 17 Jun 2020 00:49:44 GMT  
		Size: 18.4 MB (18386404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a75d228738821afda2ed880b6196234987ea752ed7c0ac05d6ae66217a976d7`  
		Last Modified: Wed, 17 Jun 2020 00:50:09 GMT  
		Size: 146.7 MB (146701694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f4f2ea37f9d8633debbd6c006f56912bb9b0df660c0e63bd3d5fc46b76b478`  
		Last Modified: Wed, 17 Jun 2020 00:49:42 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd08af79dd11a734b52c6712cbbf524b0ed1b8905ea7c6561a7cf87628b35566`  
		Last Modified: Wed, 17 Jun 2020 00:50:58 GMT  
		Size: 388.3 MB (388335825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.2-focal`

```console
$ docker pull swift@sha256:a958e3eb9c1041f280a42e5a5b026f519f62150dd87469fbc10d9f21700d14da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.2-focal` - linux; amd64

```console
$ docker pull swift@sha256:cb3959bdf578d26f7f3a4c1e510f398aa9c239ad0cc6fd652be5ebbf94994e10
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **509.0 MB (509035668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48809fb5ee4c86af95d0ac0143f4015c0ec32ca66332fc0c7fbd3dae190e142e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:20:53 GMT
ADD file:b2342c7e6665d5ff3850d4f04e2521d1851eb2054f9a8d56fcf4e7c314b9f20e in / 
# Wed, 17 Jun 2020 01:20:54 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:20:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:20:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:20:56 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:37:08 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:37:08 GMT
LABEL description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:39:10 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     binutils     git     gnupg2     libc6-dev     libcurl4     libedit2     libgcc-9-dev     libpython2.7     libsqlite3-0     libstdc++-9-dev     libxml2     libz3-dev     pkg-config     tzdata     zlib1g-dev     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:39:10 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 17 Jun 2020 02:39:11 GMT
ARG SWIFT_PLATFORM=ubuntu20.04
# Wed, 17 Jun 2020 02:39:11 GMT
ARG SWIFT_BRANCH=swift-5.2.4-release
# Wed, 17 Jun 2020 02:39:11 GMT
ARG SWIFT_VERSION=swift-5.2.4-RELEASE
# Wed, 17 Jun 2020 02:39:11 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:39:11 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu20.04 SWIFT_BRANCH=swift-5.2.4-release SWIFT_VERSION=swift-5.2.4-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:40:31 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Wed, 17 Jun 2020 02:40:33 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:a4a2a29f9ba48efd3d2075f395538b2eec56fb1bedfb7aecf5e54174446f9e2a`  
		Last Modified: Sat, 06 Jun 2020 15:19:59 GMT  
		Size: 28.6 MB (28556492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127c9761dcbaa288abc58fc56437c2f2ffbe611b9f7f30e0b5b43cd348bb2094`  
		Last Modified: Wed, 17 Jun 2020 01:22:02 GMT  
		Size: 32.3 KB (32317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13bf203e905463e64d89b14509aafa983fb8baf7c1931fe0a65652aeb6c838f`  
		Last Modified: Wed, 17 Jun 2020 01:22:01 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4039240d2e0b4bcb42ccbce75bc54570e471ad81457478de35fbeef63536e9c0`  
		Last Modified: Wed, 17 Jun 2020 01:22:02 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b80c06486cbec0481f48d39da79eacaf873f3c3c4427e7e8207a3823a2edaf`  
		Last Modified: Wed, 17 Jun 2020 03:01:26 GMT  
		Size: 93.6 MB (93569449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cf548f128817483083eecb82910c032f5ba0e2131fbb62fe308de466244849`  
		Last Modified: Wed, 17 Jun 2020 03:02:12 GMT  
		Size: 386.9 MB (386876405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.2-focal-slim`

```console
$ docker pull swift@sha256:db4dc7ea4b23dd19d412dfc53ea4a41398ebab18e67911e55734cacf4e0e2057
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.2-focal-slim` - linux; amd64

```console
$ docker pull swift@sha256:808a617b894f102c4eb7b5c1bb88ae2c677e1eb6e29274638d88fa865417e9f5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.3 MB (83298389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92095e8734294fb793dd79492fbf1722ae8d8f8abd440121bd1053373f172754`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:20:53 GMT
ADD file:b2342c7e6665d5ff3850d4f04e2521d1851eb2054f9a8d56fcf4e7c314b9f20e in / 
# Wed, 17 Jun 2020 01:20:54 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:20:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:20:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:20:56 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:37:08 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:37:08 GMT
LABEL description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:37:20 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:37:20 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 17 Jun 2020 02:37:20 GMT
ARG SWIFT_PLATFORM=ubuntu20.04
# Wed, 17 Jun 2020 02:37:20 GMT
ARG SWIFT_BRANCH=swift-5.2.4-release
# Wed, 17 Jun 2020 02:37:21 GMT
ARG SWIFT_VERSION=swift-5.2.4-RELEASE
# Wed, 17 Jun 2020 02:37:21 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:37:21 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu20.04 SWIFT_BRANCH=swift-5.2.4-release SWIFT_VERSION=swift-5.2.4-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:38:33 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl gnupg && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl gnupg
```

-	Layers:
	-	`sha256:a4a2a29f9ba48efd3d2075f395538b2eec56fb1bedfb7aecf5e54174446f9e2a`  
		Last Modified: Sat, 06 Jun 2020 15:19:59 GMT  
		Size: 28.6 MB (28556492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127c9761dcbaa288abc58fc56437c2f2ffbe611b9f7f30e0b5b43cd348bb2094`  
		Last Modified: Wed, 17 Jun 2020 01:22:02 GMT  
		Size: 32.3 KB (32317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13bf203e905463e64d89b14509aafa983fb8baf7c1931fe0a65652aeb6c838f`  
		Last Modified: Wed, 17 Jun 2020 01:22:01 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4039240d2e0b4bcb42ccbce75bc54570e471ad81457478de35fbeef63536e9c0`  
		Last Modified: Wed, 17 Jun 2020 01:22:02 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd287c1f1dc0268bbff81424af64f947ec7ce2ac383a579ddb0f687cf73df67a`  
		Last Modified: Wed, 17 Jun 2020 03:00:57 GMT  
		Size: 22.2 MB (22241328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c2c728627fbd9713ebca4f546a7cb38fdcdbcda29b3e71980135ba0e0feac4`  
		Last Modified: Wed, 17 Jun 2020 03:00:58 GMT  
		Size: 32.5 MB (32467247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.2-slim`

```console
$ docker pull swift@sha256:6be4635b0b8b3708a3ae8b6c9c30371283a513c25f3e8f6aa6af03803f60ee13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.2-slim` - linux; amd64

```console
$ docker pull swift@sha256:e1f25d8ce666f4a4205f6264f05f12d0cab03323126a50067e7e8ccb739e0984
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79656583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6feb0c96ff84c71e02cb5f7a45bdc3df7606cea92f2c576b6ea1dc1efa92b833`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:20:29 GMT
ADD file:1e8d02626176dc8141df3c0a1365774ce73d79934654fe24a4b1e7f173108232 in / 
# Wed, 17 Jun 2020 01:20:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:20:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:20:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:20:32 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:33:54 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:33:54 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 17 Jun 2020 02:33:55 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Wed, 17 Jun 2020 02:33:55 GMT
ARG SWIFT_BRANCH=swift-5.2.4-release
# Wed, 17 Jun 2020 02:33:55 GMT
ARG SWIFT_VERSION=swift-5.2.4-RELEASE
# Wed, 17 Jun 2020 02:33:56 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:33:56 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.2.4-release SWIFT_VERSION=swift-5.2.4-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:35:12 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl gnupg && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl gnupg
```

-	Layers:
	-	`sha256:d7c3167c320d7a820935f54cf4290890ea19567da496ecf774e8773b35d5f065`  
		Last Modified: Wed, 27 May 2020 12:21:15 GMT  
		Size: 26.7 MB (26688718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131f805ec7fd68d45a887e2ef82de61de0247b4eb934ab03b7c933650e854baa`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 35.4 KB (35369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322ed380e680a77f30528ba013e3a802a7b44948a0609c7d1d732dd46a9a310d`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac240b130982ad1c3ba3188abbf18ba4e54bdd9e504ce2d5c2eff6d3e86b8dd`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be976c7c6b240f9e676229be402cd77dde5ddbf2fd331b3bfa7b9ee1099456e`  
		Last Modified: Wed, 17 Jun 2020 03:00:32 GMT  
		Size: 20.5 MB (20471960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8286c2d75be4187ec9a12110bdc196beaed37a383866af8009ab333012a17a37`  
		Last Modified: Wed, 17 Jun 2020 03:00:33 GMT  
		Size: 32.5 MB (32459529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.2-xenial`

```console
$ docker pull swift@sha256:e5d21afd43717807a9df19dfc0fa7859899894460a18ffb36240de0112580e18
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.2-xenial` - linux; amd64

```console
$ docker pull swift@sha256:692333469a7fc90442ed6165c9de9ce7b9de4c6ea60d4c8248db7f38c9fe4167
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **549.6 MB (549629701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2480ab93016ba0ca44bc7dda935d209946c06b39e0d1f95c8a6fbc7a7cb19f95`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:21:26 GMT
ADD file:52af30f80ba214985a59cb0ef7073c64f8514d58396c0de48f8d7056dec2a58a in / 
# Wed, 17 Jun 2020 01:21:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:21:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:21:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:30:50 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:30:51 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:31:47 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl3     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:31:47 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 17 Jun 2020 02:31:48 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Wed, 17 Jun 2020 02:31:48 GMT
ARG SWIFT_BRANCH=swift-5.2.4-release
# Wed, 17 Jun 2020 02:31:48 GMT
ARG SWIFT_VERSION=swift-5.2.4-RELEASE
# Wed, 17 Jun 2020 02:31:49 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:31:49 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-5.2.4-release SWIFT_VERSION=swift-5.2.4-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:33:20 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Wed, 17 Jun 2020 02:33:22 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:b5e173e44934e01d8d2674bc8b1da00f761c4fe796e0fb2bee1bd1129d2e4ae1`  
		Last Modified: Fri, 15 May 2020 13:20:22 GMT  
		Size: 44.3 MB (44320272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29047100b0407dff554ea80b8005380d62b13a66d7fe2e2adb07b9c091b9f2c0`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 531.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15743a713c2a4033877dab08fb3989280f8c856234227158a4011811c7991372`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6bc9e2987763aa991b7dfd742be04c7b3bb04448982ffe88e58d55c93b76d4`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11426dc469ff356e2be300a91a31d297702f5754f463aaa564ca00b9a37b1ea2`  
		Last Modified: Wed, 17 Jun 2020 02:59:31 GMT  
		Size: 111.5 MB (111534848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba73bfd6b863e49120e0da4ead85b0017b6c8c8389746dbc1ff26bfc02524b9`  
		Last Modified: Wed, 17 Jun 2020 03:00:17 GMT  
		Size: 393.8 MB (393773025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.2-xenial-slim`

```console
$ docker pull swift@sha256:4c6a9e0f040e42a94f0fc63d99d0a6a652f2a1371e73cd5b560a8ae82a4cef48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.2-xenial-slim` - linux; amd64

```console
$ docker pull swift@sha256:77af1fb0305217aaa904a20c4266bb37465ae9ed3e18dae70ca48f3191a638b3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.5 MB (97538700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c756b51ad5ff62a291e5d1911ecc48634d899d1bde88ff69f8ddbabdb6c91238`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:21:26 GMT
ADD file:52af30f80ba214985a59cb0ef7073c64f8514d58396c0de48f8d7056dec2a58a in / 
# Wed, 17 Jun 2020 01:21:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:21:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:21:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:30:50 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:30:51 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:35:35 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl3     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:35:35 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 17 Jun 2020 02:35:36 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Wed, 17 Jun 2020 02:35:36 GMT
ARG SWIFT_BRANCH=swift-5.2.4-release
# Wed, 17 Jun 2020 02:35:36 GMT
ARG SWIFT_VERSION=swift-5.2.4-RELEASE
# Wed, 17 Jun 2020 02:35:36 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:35:37 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-5.2.4-release SWIFT_VERSION=swift-5.2.4-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:36:50 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
```

-	Layers:
	-	`sha256:b5e173e44934e01d8d2674bc8b1da00f761c4fe796e0fb2bee1bd1129d2e4ae1`  
		Last Modified: Fri, 15 May 2020 13:20:22 GMT  
		Size: 44.3 MB (44320272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29047100b0407dff554ea80b8005380d62b13a66d7fe2e2adb07b9c091b9f2c0`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 531.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15743a713c2a4033877dab08fb3989280f8c856234227158a4011811c7991372`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6bc9e2987763aa991b7dfd742be04c7b3bb04448982ffe88e58d55c93b76d4`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da1f8178404835f2182a23ff9eb65d65ff3015da8d71433f43db492410a3129d`  
		Last Modified: Wed, 17 Jun 2020 03:00:45 GMT  
		Size: 20.8 MB (20845087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a2dadc5cb2bea665f3846de4ac7f09e7458df26fcd0ff3befbc73a28528e3b2`  
		Last Modified: Wed, 17 Jun 2020 03:00:46 GMT  
		Size: 32.4 MB (32371785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:amazonlinux2`

```console
$ docker pull swift@sha256:223ea1eefa3f0dfecd195fd29e6f4f098d8ac4a77eaf16eff779044a4184c999
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:amazonlinux2` - linux; amd64

```console
$ docker pull swift@sha256:2d30f58a12d1cb089a2f788bb35aa100c786b3b8ae5efda45e993d708a427893
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **685.0 MB (685037474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f19e4f405c699a3280d7c63980f8f99c4b66e3c641c8ceaaf15b153acc614aba`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Jun 2020 20:20:04 GMT
ADD file:788af9048b1c163347d7a8349f8ecf5721b4d8b63395ec8c6ca6d0732f57acdd in / 
# Tue, 30 Jun 2020 20:20:05 GMT
CMD ["/bin/bash"]
# Tue, 30 Jun 2020 20:57:47 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Tue, 30 Jun 2020 20:57:47 GMT
LABEL description=Docker Container for the Swift programming language
# Tue, 30 Jun 2020 21:00:01 GMT
RUN yum -y update && yum -y install   binutils   gcc   git   glibc-static   gzip   libbsd   libcurl   libedit   libicu   libsqlite   libstdc++-static   libuuid   libxml2   tar   tzdata   zlib-devel
# Tue, 30 Jun 2020 21:00:02 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Tue, 30 Jun 2020 21:00:02 GMT
ARG SWIFT_PLATFORM=amazonlinux2
# Tue, 30 Jun 2020 21:00:02 GMT
ARG SWIFT_BRANCH=swift-5.2.4-release
# Tue, 30 Jun 2020 21:00:02 GMT
ARG SWIFT_VERSION=swift-5.2.4-RELEASE
# Tue, 30 Jun 2020 21:00:02 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Tue, 30 Jun 2020 21:00:03 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=amazonlinux2 SWIFT_BRANCH=swift-5.2.4-release SWIFT_VERSION=swift-5.2.4-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Tue, 30 Jun 2020 21:01:32 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz
# Tue, 30 Jun 2020 21:01:33 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:3d24604292f287c31563b1f563e83307e7915909506659401fb07c1c3e6e164c`  
		Last Modified: Tue, 30 Jun 2020 20:21:31 GMT  
		Size: 61.7 MB (61684682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea50e5b47eb33e6b56eb394bef851b8cbe7627ceb40460d4f3d654fcbb0a676`  
		Last Modified: Tue, 30 Jun 2020 21:04:44 GMT  
		Size: 234.4 MB (234382905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec95769a775463f018621e30a9b7bce62c5db31569f165e7162c5f67216dd938`  
		Last Modified: Tue, 30 Jun 2020 21:05:36 GMT  
		Size: 389.0 MB (388969887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:bionic`

```console
$ docker pull swift@sha256:b1e98d1807bd6df4a7b8431d0ddb0a2ed5f9ce119d0db113451dd30e5d57740c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:bionic` - linux; amd64

```console
$ docker pull swift@sha256:087c8e19d8b53e3442f6ebbd1c2d4bac57098ddcff3b3db12fc38572cb82b75c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **537.5 MB (537509085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bef395c099c7e6e27dd068ba2e66d6bf929e31e5c1c44c216629e3a5de39fcb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:20:29 GMT
ADD file:1e8d02626176dc8141df3c0a1365774ce73d79934654fe24a4b1e7f173108232 in / 
# Wed, 17 Jun 2020 01:20:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:20:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:20:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:20:32 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:29:10 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:29:10 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 17 Jun 2020 02:29:11 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Wed, 17 Jun 2020 02:29:11 GMT
ARG SWIFT_BRANCH=swift-5.2.4-release
# Wed, 17 Jun 2020 02:29:12 GMT
ARG SWIFT_VERSION=swift-5.2.4-RELEASE
# Wed, 17 Jun 2020 02:29:12 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:29:12 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.2.4-release SWIFT_VERSION=swift-5.2.4-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:30:41 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Wed, 17 Jun 2020 02:30:43 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:d7c3167c320d7a820935f54cf4290890ea19567da496ecf774e8773b35d5f065`  
		Last Modified: Wed, 27 May 2020 12:21:15 GMT  
		Size: 26.7 MB (26688718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131f805ec7fd68d45a887e2ef82de61de0247b4eb934ab03b7c933650e854baa`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 35.4 KB (35369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322ed380e680a77f30528ba013e3a802a7b44948a0609c7d1d732dd46a9a310d`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac240b130982ad1c3ba3188abbf18ba4e54bdd9e504ce2d5c2eff6d3e86b8dd`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459101facad87c08bc7770f59f7ce58838101b487f08e56534d241b1637ea11f`  
		Last Modified: Wed, 17 Jun 2020 02:58:20 GMT  
		Size: 124.1 MB (124051844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1061d32da7815faf492e182f868761c28abd0fbc6abcf84bc52c29b7d396bf`  
		Last Modified: Wed, 17 Jun 2020 02:59:01 GMT  
		Size: 386.7 MB (386732147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:bionic-slim`

```console
$ docker pull swift@sha256:6be4635b0b8b3708a3ae8b6c9c30371283a513c25f3e8f6aa6af03803f60ee13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:bionic-slim` - linux; amd64

```console
$ docker pull swift@sha256:e1f25d8ce666f4a4205f6264f05f12d0cab03323126a50067e7e8ccb739e0984
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79656583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6feb0c96ff84c71e02cb5f7a45bdc3df7606cea92f2c576b6ea1dc1efa92b833`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:20:29 GMT
ADD file:1e8d02626176dc8141df3c0a1365774ce73d79934654fe24a4b1e7f173108232 in / 
# Wed, 17 Jun 2020 01:20:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:20:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:20:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:20:32 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:33:54 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:33:54 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 17 Jun 2020 02:33:55 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Wed, 17 Jun 2020 02:33:55 GMT
ARG SWIFT_BRANCH=swift-5.2.4-release
# Wed, 17 Jun 2020 02:33:55 GMT
ARG SWIFT_VERSION=swift-5.2.4-RELEASE
# Wed, 17 Jun 2020 02:33:56 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:33:56 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.2.4-release SWIFT_VERSION=swift-5.2.4-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:35:12 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl gnupg && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl gnupg
```

-	Layers:
	-	`sha256:d7c3167c320d7a820935f54cf4290890ea19567da496ecf774e8773b35d5f065`  
		Last Modified: Wed, 27 May 2020 12:21:15 GMT  
		Size: 26.7 MB (26688718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131f805ec7fd68d45a887e2ef82de61de0247b4eb934ab03b7c933650e854baa`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 35.4 KB (35369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322ed380e680a77f30528ba013e3a802a7b44948a0609c7d1d732dd46a9a310d`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac240b130982ad1c3ba3188abbf18ba4e54bdd9e504ce2d5c2eff6d3e86b8dd`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be976c7c6b240f9e676229be402cd77dde5ddbf2fd331b3bfa7b9ee1099456e`  
		Last Modified: Wed, 17 Jun 2020 03:00:32 GMT  
		Size: 20.5 MB (20471960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8286c2d75be4187ec9a12110bdc196beaed37a383866af8009ab333012a17a37`  
		Last Modified: Wed, 17 Jun 2020 03:00:33 GMT  
		Size: 32.5 MB (32459529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:centos8`

```console
$ docker pull swift@sha256:6343f107c590e305973893809591cd6ea3ed31cbdaa996dce36dcc9787b382b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:centos8` - linux; amd64

```console
$ docker pull swift@sha256:209d86ff24e0843b84c683840df6a1aec9788a2b7e6675ca452c051a9b84d22c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **628.3 MB (628290894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3678c629101e3b6c922738049111e92c8fa40d10a322d4625aeac7f1a17b3762`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 00:22:24 GMT
ADD file:84700c11fcc969ac08ef25f115513d76c7b72a4118c01fbc86ef0a6056fdebeb in / 
# Wed, 17 Jun 2020 00:22:25 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200611
# Wed, 17 Jun 2020 00:22:25 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 00:46:24 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 00:46:24 GMT
LABEL description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 00:46:29 GMT
RUN yum install -y https://dl.fedoraproject.org/pub/epel/epel-release-latest-8.noarch.rpm
# Wed, 17 Jun 2020 00:47:01 GMT
RUN yum -y update && yum install --enablerepo=PowerTools -y   binutils   gcc   git   glibc-static   libbsd-devel   libedit   libedit-devel   libicu-devel   libstdc++-static   pkg-config   python2   sqlite   zlib-devel
# Wed, 17 Jun 2020 00:47:02 GMT
RUN ln -s /usr/bin/python2 /usr/bin/python
# Wed, 17 Jun 2020 00:47:02 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 17 Jun 2020 00:47:02 GMT
ARG SWIFT_PLATFORM=centos8
# Wed, 17 Jun 2020 00:47:03 GMT
ARG SWIFT_BRANCH=swift-5.2.4-release
# Wed, 17 Jun 2020 00:47:03 GMT
ARG SWIFT_VERSION=swift-5.2.4-RELEASE
# Wed, 17 Jun 2020 00:47:03 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 00:47:03 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=centos8 SWIFT_BRANCH=swift-5.2.4-release SWIFT_VERSION=swift-5.2.4-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 00:48:20 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz
# Wed, 17 Jun 2020 00:48:22 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:6910e5a164f725142d77994b247ba20040477fbab49a721bdbe8d61cf855ac23`  
		Last Modified: Wed, 17 Jun 2020 00:23:52 GMT  
		Size: 74.9 MB (74866818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25c5181aa902d0b68a772ff8e20440647e871f794439c373f247e767e6eda27`  
		Last Modified: Wed, 17 Jun 2020 00:49:44 GMT  
		Size: 18.4 MB (18386404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a75d228738821afda2ed880b6196234987ea752ed7c0ac05d6ae66217a976d7`  
		Last Modified: Wed, 17 Jun 2020 00:50:09 GMT  
		Size: 146.7 MB (146701694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f4f2ea37f9d8633debbd6c006f56912bb9b0df660c0e63bd3d5fc46b76b478`  
		Last Modified: Wed, 17 Jun 2020 00:49:42 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd08af79dd11a734b52c6712cbbf524b0ed1b8905ea7c6561a7cf87628b35566`  
		Last Modified: Wed, 17 Jun 2020 00:50:58 GMT  
		Size: 388.3 MB (388335825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:focal`

```console
$ docker pull swift@sha256:a958e3eb9c1041f280a42e5a5b026f519f62150dd87469fbc10d9f21700d14da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:focal` - linux; amd64

```console
$ docker pull swift@sha256:cb3959bdf578d26f7f3a4c1e510f398aa9c239ad0cc6fd652be5ebbf94994e10
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **509.0 MB (509035668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48809fb5ee4c86af95d0ac0143f4015c0ec32ca66332fc0c7fbd3dae190e142e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:20:53 GMT
ADD file:b2342c7e6665d5ff3850d4f04e2521d1851eb2054f9a8d56fcf4e7c314b9f20e in / 
# Wed, 17 Jun 2020 01:20:54 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:20:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:20:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:20:56 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:37:08 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:37:08 GMT
LABEL description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:39:10 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     binutils     git     gnupg2     libc6-dev     libcurl4     libedit2     libgcc-9-dev     libpython2.7     libsqlite3-0     libstdc++-9-dev     libxml2     libz3-dev     pkg-config     tzdata     zlib1g-dev     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:39:10 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 17 Jun 2020 02:39:11 GMT
ARG SWIFT_PLATFORM=ubuntu20.04
# Wed, 17 Jun 2020 02:39:11 GMT
ARG SWIFT_BRANCH=swift-5.2.4-release
# Wed, 17 Jun 2020 02:39:11 GMT
ARG SWIFT_VERSION=swift-5.2.4-RELEASE
# Wed, 17 Jun 2020 02:39:11 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:39:11 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu20.04 SWIFT_BRANCH=swift-5.2.4-release SWIFT_VERSION=swift-5.2.4-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:40:31 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Wed, 17 Jun 2020 02:40:33 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:a4a2a29f9ba48efd3d2075f395538b2eec56fb1bedfb7aecf5e54174446f9e2a`  
		Last Modified: Sat, 06 Jun 2020 15:19:59 GMT  
		Size: 28.6 MB (28556492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127c9761dcbaa288abc58fc56437c2f2ffbe611b9f7f30e0b5b43cd348bb2094`  
		Last Modified: Wed, 17 Jun 2020 01:22:02 GMT  
		Size: 32.3 KB (32317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13bf203e905463e64d89b14509aafa983fb8baf7c1931fe0a65652aeb6c838f`  
		Last Modified: Wed, 17 Jun 2020 01:22:01 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4039240d2e0b4bcb42ccbce75bc54570e471ad81457478de35fbeef63536e9c0`  
		Last Modified: Wed, 17 Jun 2020 01:22:02 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b80c06486cbec0481f48d39da79eacaf873f3c3c4427e7e8207a3823a2edaf`  
		Last Modified: Wed, 17 Jun 2020 03:01:26 GMT  
		Size: 93.6 MB (93569449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cf548f128817483083eecb82910c032f5ba0e2131fbb62fe308de466244849`  
		Last Modified: Wed, 17 Jun 2020 03:02:12 GMT  
		Size: 386.9 MB (386876405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:focal-slim`

```console
$ docker pull swift@sha256:db4dc7ea4b23dd19d412dfc53ea4a41398ebab18e67911e55734cacf4e0e2057
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:focal-slim` - linux; amd64

```console
$ docker pull swift@sha256:808a617b894f102c4eb7b5c1bb88ae2c677e1eb6e29274638d88fa865417e9f5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.3 MB (83298389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92095e8734294fb793dd79492fbf1722ae8d8f8abd440121bd1053373f172754`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:20:53 GMT
ADD file:b2342c7e6665d5ff3850d4f04e2521d1851eb2054f9a8d56fcf4e7c314b9f20e in / 
# Wed, 17 Jun 2020 01:20:54 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:20:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:20:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:20:56 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:37:08 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:37:08 GMT
LABEL description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:37:20 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:37:20 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 17 Jun 2020 02:37:20 GMT
ARG SWIFT_PLATFORM=ubuntu20.04
# Wed, 17 Jun 2020 02:37:20 GMT
ARG SWIFT_BRANCH=swift-5.2.4-release
# Wed, 17 Jun 2020 02:37:21 GMT
ARG SWIFT_VERSION=swift-5.2.4-RELEASE
# Wed, 17 Jun 2020 02:37:21 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:37:21 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu20.04 SWIFT_BRANCH=swift-5.2.4-release SWIFT_VERSION=swift-5.2.4-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:38:33 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl gnupg && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl gnupg
```

-	Layers:
	-	`sha256:a4a2a29f9ba48efd3d2075f395538b2eec56fb1bedfb7aecf5e54174446f9e2a`  
		Last Modified: Sat, 06 Jun 2020 15:19:59 GMT  
		Size: 28.6 MB (28556492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127c9761dcbaa288abc58fc56437c2f2ffbe611b9f7f30e0b5b43cd348bb2094`  
		Last Modified: Wed, 17 Jun 2020 01:22:02 GMT  
		Size: 32.3 KB (32317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13bf203e905463e64d89b14509aafa983fb8baf7c1931fe0a65652aeb6c838f`  
		Last Modified: Wed, 17 Jun 2020 01:22:01 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4039240d2e0b4bcb42ccbce75bc54570e471ad81457478de35fbeef63536e9c0`  
		Last Modified: Wed, 17 Jun 2020 01:22:02 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd287c1f1dc0268bbff81424af64f947ec7ce2ac383a579ddb0f687cf73df67a`  
		Last Modified: Wed, 17 Jun 2020 03:00:57 GMT  
		Size: 22.2 MB (22241328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c2c728627fbd9713ebca4f546a7cb38fdcdbcda29b3e71980135ba0e0feac4`  
		Last Modified: Wed, 17 Jun 2020 03:00:58 GMT  
		Size: 32.5 MB (32467247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:latest`

```console
$ docker pull swift@sha256:b1e98d1807bd6df4a7b8431d0ddb0a2ed5f9ce119d0db113451dd30e5d57740c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:latest` - linux; amd64

```console
$ docker pull swift@sha256:087c8e19d8b53e3442f6ebbd1c2d4bac57098ddcff3b3db12fc38572cb82b75c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **537.5 MB (537509085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bef395c099c7e6e27dd068ba2e66d6bf929e31e5c1c44c216629e3a5de39fcb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:20:29 GMT
ADD file:1e8d02626176dc8141df3c0a1365774ce73d79934654fe24a4b1e7f173108232 in / 
# Wed, 17 Jun 2020 01:20:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:20:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:20:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:20:32 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:29:10 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:29:10 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 17 Jun 2020 02:29:11 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Wed, 17 Jun 2020 02:29:11 GMT
ARG SWIFT_BRANCH=swift-5.2.4-release
# Wed, 17 Jun 2020 02:29:12 GMT
ARG SWIFT_VERSION=swift-5.2.4-RELEASE
# Wed, 17 Jun 2020 02:29:12 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:29:12 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.2.4-release SWIFT_VERSION=swift-5.2.4-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:30:41 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Wed, 17 Jun 2020 02:30:43 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:d7c3167c320d7a820935f54cf4290890ea19567da496ecf774e8773b35d5f065`  
		Last Modified: Wed, 27 May 2020 12:21:15 GMT  
		Size: 26.7 MB (26688718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131f805ec7fd68d45a887e2ef82de61de0247b4eb934ab03b7c933650e854baa`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 35.4 KB (35369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322ed380e680a77f30528ba013e3a802a7b44948a0609c7d1d732dd46a9a310d`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac240b130982ad1c3ba3188abbf18ba4e54bdd9e504ce2d5c2eff6d3e86b8dd`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459101facad87c08bc7770f59f7ce58838101b487f08e56534d241b1637ea11f`  
		Last Modified: Wed, 17 Jun 2020 02:58:20 GMT  
		Size: 124.1 MB (124051844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1061d32da7815faf492e182f868761c28abd0fbc6abcf84bc52c29b7d396bf`  
		Last Modified: Wed, 17 Jun 2020 02:59:01 GMT  
		Size: 386.7 MB (386732147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:slim`

```console
$ docker pull swift@sha256:6be4635b0b8b3708a3ae8b6c9c30371283a513c25f3e8f6aa6af03803f60ee13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:slim` - linux; amd64

```console
$ docker pull swift@sha256:e1f25d8ce666f4a4205f6264f05f12d0cab03323126a50067e7e8ccb739e0984
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79656583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6feb0c96ff84c71e02cb5f7a45bdc3df7606cea92f2c576b6ea1dc1efa92b833`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:20:29 GMT
ADD file:1e8d02626176dc8141df3c0a1365774ce73d79934654fe24a4b1e7f173108232 in / 
# Wed, 17 Jun 2020 01:20:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:20:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:20:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:20:32 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:27:31 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:33:54 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:33:54 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 17 Jun 2020 02:33:55 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Wed, 17 Jun 2020 02:33:55 GMT
ARG SWIFT_BRANCH=swift-5.2.4-release
# Wed, 17 Jun 2020 02:33:55 GMT
ARG SWIFT_VERSION=swift-5.2.4-RELEASE
# Wed, 17 Jun 2020 02:33:56 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:33:56 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.2.4-release SWIFT_VERSION=swift-5.2.4-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:35:12 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl gnupg && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl gnupg
```

-	Layers:
	-	`sha256:d7c3167c320d7a820935f54cf4290890ea19567da496ecf774e8773b35d5f065`  
		Last Modified: Wed, 27 May 2020 12:21:15 GMT  
		Size: 26.7 MB (26688718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131f805ec7fd68d45a887e2ef82de61de0247b4eb934ab03b7c933650e854baa`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 35.4 KB (35369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322ed380e680a77f30528ba013e3a802a7b44948a0609c7d1d732dd46a9a310d`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac240b130982ad1c3ba3188abbf18ba4e54bdd9e504ce2d5c2eff6d3e86b8dd`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be976c7c6b240f9e676229be402cd77dde5ddbf2fd331b3bfa7b9ee1099456e`  
		Last Modified: Wed, 17 Jun 2020 03:00:32 GMT  
		Size: 20.5 MB (20471960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8286c2d75be4187ec9a12110bdc196beaed37a383866af8009ab333012a17a37`  
		Last Modified: Wed, 17 Jun 2020 03:00:33 GMT  
		Size: 32.5 MB (32459529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:xenial`

```console
$ docker pull swift@sha256:e5d21afd43717807a9df19dfc0fa7859899894460a18ffb36240de0112580e18
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:xenial` - linux; amd64

```console
$ docker pull swift@sha256:692333469a7fc90442ed6165c9de9ce7b9de4c6ea60d4c8248db7f38c9fe4167
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **549.6 MB (549629701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2480ab93016ba0ca44bc7dda935d209946c06b39e0d1f95c8a6fbc7a7cb19f95`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:21:26 GMT
ADD file:52af30f80ba214985a59cb0ef7073c64f8514d58396c0de48f8d7056dec2a58a in / 
# Wed, 17 Jun 2020 01:21:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:21:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:21:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:30:50 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:30:51 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:31:47 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl3     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:31:47 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 17 Jun 2020 02:31:48 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Wed, 17 Jun 2020 02:31:48 GMT
ARG SWIFT_BRANCH=swift-5.2.4-release
# Wed, 17 Jun 2020 02:31:48 GMT
ARG SWIFT_VERSION=swift-5.2.4-RELEASE
# Wed, 17 Jun 2020 02:31:49 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:31:49 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-5.2.4-release SWIFT_VERSION=swift-5.2.4-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:33:20 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Wed, 17 Jun 2020 02:33:22 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:b5e173e44934e01d8d2674bc8b1da00f761c4fe796e0fb2bee1bd1129d2e4ae1`  
		Last Modified: Fri, 15 May 2020 13:20:22 GMT  
		Size: 44.3 MB (44320272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29047100b0407dff554ea80b8005380d62b13a66d7fe2e2adb07b9c091b9f2c0`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 531.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15743a713c2a4033877dab08fb3989280f8c856234227158a4011811c7991372`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6bc9e2987763aa991b7dfd742be04c7b3bb04448982ffe88e58d55c93b76d4`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11426dc469ff356e2be300a91a31d297702f5754f463aaa564ca00b9a37b1ea2`  
		Last Modified: Wed, 17 Jun 2020 02:59:31 GMT  
		Size: 111.5 MB (111534848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba73bfd6b863e49120e0da4ead85b0017b6c8c8389746dbc1ff26bfc02524b9`  
		Last Modified: Wed, 17 Jun 2020 03:00:17 GMT  
		Size: 393.8 MB (393773025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:xenial-slim`

```console
$ docker pull swift@sha256:4c6a9e0f040e42a94f0fc63d99d0a6a652f2a1371e73cd5b560a8ae82a4cef48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:xenial-slim` - linux; amd64

```console
$ docker pull swift@sha256:77af1fb0305217aaa904a20c4266bb37465ae9ed3e18dae70ca48f3191a638b3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.5 MB (97538700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c756b51ad5ff62a291e5d1911ecc48634d899d1bde88ff69f8ddbabdb6c91238`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:21:26 GMT
ADD file:52af30f80ba214985a59cb0ef7073c64f8514d58396c0de48f8d7056dec2a58a in / 
# Wed, 17 Jun 2020 01:21:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:21:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:21:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:30:50 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 17 Jun 2020 02:30:51 GMT
LABEL Description=Docker Container for the Swift programming language
# Wed, 17 Jun 2020 02:35:35 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl3     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:35:35 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 17 Jun 2020 02:35:36 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Wed, 17 Jun 2020 02:35:36 GMT
ARG SWIFT_BRANCH=swift-5.2.4-release
# Wed, 17 Jun 2020 02:35:36 GMT
ARG SWIFT_VERSION=swift-5.2.4-RELEASE
# Wed, 17 Jun 2020 02:35:36 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:35:37 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-5.2.4-release SWIFT_VERSION=swift-5.2.4-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 17 Jun 2020 02:36:50 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
```

-	Layers:
	-	`sha256:b5e173e44934e01d8d2674bc8b1da00f761c4fe796e0fb2bee1bd1129d2e4ae1`  
		Last Modified: Fri, 15 May 2020 13:20:22 GMT  
		Size: 44.3 MB (44320272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29047100b0407dff554ea80b8005380d62b13a66d7fe2e2adb07b9c091b9f2c0`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 531.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15743a713c2a4033877dab08fb3989280f8c856234227158a4011811c7991372`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6bc9e2987763aa991b7dfd742be04c7b3bb04448982ffe88e58d55c93b76d4`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da1f8178404835f2182a23ff9eb65d65ff3015da8d71433f43db492410a3129d`  
		Last Modified: Wed, 17 Jun 2020 03:00:45 GMT  
		Size: 20.8 MB (20845087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a2dadc5cb2bea665f3846de4ac7f09e7458df26fcd0ff3befbc73a28528e3b2`  
		Last Modified: Wed, 17 Jun 2020 03:00:46 GMT  
		Size: 32.4 MB (32371785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
