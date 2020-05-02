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
-	[`swift:5.2.3`](#swift523)
-	[`swift:5.2.3-bionic`](#swift523-bionic)
-	[`swift:5.2.3-bionic-slim`](#swift523-bionic-slim)
-	[`swift:5.2.3-slim`](#swift523-slim)
-	[`swift:5.2.3-xenial`](#swift523-xenial)
-	[`swift:5.2.3-xenial-slim`](#swift523-xenial-slim)
-	[`swift:5.2-bionic`](#swift52-bionic)
-	[`swift:5.2-bionic-slim`](#swift52-bionic-slim)
-	[`swift:5.2-slim`](#swift52-slim)
-	[`swift:5.2-xenial`](#swift52-xenial)
-	[`swift:5.2-xenial-slim`](#swift52-xenial-slim)
-	[`swift:bionic`](#swiftbionic)
-	[`swift:bionic-slim`](#swiftbionic-slim)
-	[`swift:latest`](#swiftlatest)
-	[`swift:slim`](#swiftslim)
-	[`swift:xenial`](#swiftxenial)
-	[`swift:xenial-slim`](#swiftxenial-slim)

## `swift:4`

```console
$ docker pull swift@sha256:0b3e72a5af09f93983e4029ef9653a406bb0349e313ca809d3a0d341b90dd736
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:4` - linux; amd64

```console
$ docker pull swift@sha256:62508fb30694d78efa386497b7b17158568493a4dff2ac512702f7afe6decfb2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **496.9 MB (496870900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6a86a74b4ad3e5430c72f5fe640913d1305207c41e4fc1b0ed38e7fc86831a6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:25:51 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 24 Apr 2020 21:25:51 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 24 Apr 2020 21:44:25 GMT
RUN apt-get -q update &&     apt-get -q install -y     make     libc6-dev     clang-3.8     curl     libedit-dev     libpython2.7     libicu-dev     libssl-dev     libxml2     tzdata     git     libcurl4-openssl-dev     pkg-config     && update-alternatives --quiet --install /usr/bin/clang clang /usr/bin/clang-3.8 100     && update-alternatives --quiet --install /usr/bin/clang++ clang++ /usr/bin/clang++-3.8 100     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:44:25 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Fri, 24 Apr 2020 21:44:26 GMT
ARG SWIFT_BRANCH=swift-4.2.4-release
# Fri, 24 Apr 2020 21:44:26 GMT
ARG SWIFT_VERSION=swift-4.2.4-RELEASE
# Fri, 24 Apr 2020 21:44:26 GMT
ENV SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-4.2.4-release SWIFT_VERSION=swift-4.2.4-RELEASE
# Fri, 24 Apr 2020 21:45:10 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           8513444E2DA36B7C1659AF4D7638F1FB2B2B08C4           A3BAFD3556A59079C06894BD63BC1CFE91D306C6           5E4DF843FB065D7F7E24FBA2EF5430F071E1B235         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
# Fri, 24 Apr 2020 21:45:11 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb47c322eeb3f3831495f380f3f3c5fa87d32146dfe5d1fc73331e6b0c0fca9`  
		Last Modified: Fri, 24 Apr 2020 21:56:49 GMT  
		Size: 224.5 MB (224456061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af86238a5645c7753125cdd883cb6693f059ca3a44804705401ce014c5fe35c7`  
		Last Modified: Fri, 24 Apr 2020 21:56:49 GMT  
		Size: 228.2 MB (228166158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:4.0`

```console
$ docker pull swift@sha256:afd74428831c1e08ce778f69f302508218fc647d2dabdd91e389fafb9cd05a77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:4.0` - linux; amd64

```console
$ docker pull swift@sha256:0b0b95fcc9bf0194159bb53052a9ac7c1803eb9dfb4b8fca7239403449a51696
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **439.3 MB (439343133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4162407a859c74e937887598df4d591a229e5dfabdc04c27525e1e8f56244a98`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:45:15 GMT
LABEL maintainer=Haris Amin <aminharis7@gmail.com>
# Fri, 24 Apr 2020 21:45:16 GMT
LABEL Description=Docker Container for the Apple's Swift programming language
# Fri, 24 Apr 2020 21:46:04 GMT
RUN apt-get -q update &&     apt-get -q install -y     make     libc6-dev     clang-3.8     curl     libedit-dev     libpython2.7     libicu-dev     libssl-dev     libxml2     tzdata     git     libcurl4-openssl-dev     pkg-config     && update-alternatives --quiet --install /usr/bin/clang clang /usr/bin/clang-3.8 100     && update-alternatives --quiet --install /usr/bin/clang++ clang++ /usr/bin/clang++-3.8 100     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:46:05 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Fri, 24 Apr 2020 21:47:00 GMT
ARG SWIFT_BRANCH=swift-4.0.3-release
# Fri, 24 Apr 2020 21:47:01 GMT
ARG SWIFT_VERSION=swift-4.0.3-RELEASE
# Fri, 24 Apr 2020 21:47:01 GMT
ENV SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-4.0.3-release SWIFT_VERSION=swift-4.0.3-RELEASE
# Fri, 24 Apr 2020 21:47:34 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           8513444E2DA36B7C1659AF4D7638F1FB2B2B08C4           A3BAFD3556A59079C06894BD63BC1CFE91D306C6           5E4DF843FB065D7F7E24FBA2EF5430F071E1B235         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
# Fri, 24 Apr 2020 21:47:35 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e921f1e439c9e57e62899f6fccec9d2b228278e575d90e5faa1e506b9ef9a11f`  
		Last Modified: Fri, 24 Apr 2020 21:57:41 GMT  
		Size: 224.5 MB (224456516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d477baac871c80af61d5f952a07401716f16b67cfe31c974e933d9b3c2175d`  
		Last Modified: Fri, 24 Apr 2020 21:58:18 GMT  
		Size: 170.6 MB (170637936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:4.0.3`

```console
$ docker pull swift@sha256:afd74428831c1e08ce778f69f302508218fc647d2dabdd91e389fafb9cd05a77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:4.0.3` - linux; amd64

```console
$ docker pull swift@sha256:0b0b95fcc9bf0194159bb53052a9ac7c1803eb9dfb4b8fca7239403449a51696
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **439.3 MB (439343133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4162407a859c74e937887598df4d591a229e5dfabdc04c27525e1e8f56244a98`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:45:15 GMT
LABEL maintainer=Haris Amin <aminharis7@gmail.com>
# Fri, 24 Apr 2020 21:45:16 GMT
LABEL Description=Docker Container for the Apple's Swift programming language
# Fri, 24 Apr 2020 21:46:04 GMT
RUN apt-get -q update &&     apt-get -q install -y     make     libc6-dev     clang-3.8     curl     libedit-dev     libpython2.7     libicu-dev     libssl-dev     libxml2     tzdata     git     libcurl4-openssl-dev     pkg-config     && update-alternatives --quiet --install /usr/bin/clang clang /usr/bin/clang-3.8 100     && update-alternatives --quiet --install /usr/bin/clang++ clang++ /usr/bin/clang++-3.8 100     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:46:05 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Fri, 24 Apr 2020 21:47:00 GMT
ARG SWIFT_BRANCH=swift-4.0.3-release
# Fri, 24 Apr 2020 21:47:01 GMT
ARG SWIFT_VERSION=swift-4.0.3-RELEASE
# Fri, 24 Apr 2020 21:47:01 GMT
ENV SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-4.0.3-release SWIFT_VERSION=swift-4.0.3-RELEASE
# Fri, 24 Apr 2020 21:47:34 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           8513444E2DA36B7C1659AF4D7638F1FB2B2B08C4           A3BAFD3556A59079C06894BD63BC1CFE91D306C6           5E4DF843FB065D7F7E24FBA2EF5430F071E1B235         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
# Fri, 24 Apr 2020 21:47:35 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e921f1e439c9e57e62899f6fccec9d2b228278e575d90e5faa1e506b9ef9a11f`  
		Last Modified: Fri, 24 Apr 2020 21:57:41 GMT  
		Size: 224.5 MB (224456516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d477baac871c80af61d5f952a07401716f16b67cfe31c974e933d9b3c2175d`  
		Last Modified: Fri, 24 Apr 2020 21:58:18 GMT  
		Size: 170.6 MB (170637936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:4.1`

```console
$ docker pull swift@sha256:3ff875313f89137f1f5ed122570c0221a888e00992cf43dd8dbd19b443c2fc98
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:4.1` - linux; amd64

```console
$ docker pull swift@sha256:1b6d2ac9677206b94c22349f8eaf8d586574e9b27e1359a752d53cc3f2ac89be
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **451.9 MB (451937473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13ca9d5b6955d631e265a63efb3a798f7f5d3cdfe2c62e12be71a5f910081269`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:45:15 GMT
LABEL maintainer=Haris Amin <aminharis7@gmail.com>
# Fri, 24 Apr 2020 21:45:16 GMT
LABEL Description=Docker Container for the Apple's Swift programming language
# Fri, 24 Apr 2020 21:46:04 GMT
RUN apt-get -q update &&     apt-get -q install -y     make     libc6-dev     clang-3.8     curl     libedit-dev     libpython2.7     libicu-dev     libssl-dev     libxml2     tzdata     git     libcurl4-openssl-dev     pkg-config     && update-alternatives --quiet --install /usr/bin/clang clang /usr/bin/clang-3.8 100     && update-alternatives --quiet --install /usr/bin/clang++ clang++ /usr/bin/clang++-3.8 100     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:46:05 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Fri, 24 Apr 2020 21:46:05 GMT
ARG SWIFT_BRANCH=swift-4.1.3-release
# Fri, 24 Apr 2020 21:46:05 GMT
ARG SWIFT_VERSION=swift-4.1.3-RELEASE
# Fri, 24 Apr 2020 21:46:05 GMT
ENV SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-4.1.3-release SWIFT_VERSION=swift-4.1.3-RELEASE
# Fri, 24 Apr 2020 21:46:43 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           8513444E2DA36B7C1659AF4D7638F1FB2B2B08C4           A3BAFD3556A59079C06894BD63BC1CFE91D306C6           5E4DF843FB065D7F7E24FBA2EF5430F071E1B235         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
# Fri, 24 Apr 2020 21:46:44 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e921f1e439c9e57e62899f6fccec9d2b228278e575d90e5faa1e506b9ef9a11f`  
		Last Modified: Fri, 24 Apr 2020 21:57:41 GMT  
		Size: 224.5 MB (224456516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9527d39e2432b1d6742c4d0a1b916e51cb045c77149d2e4b92a7db86a785c8d8`  
		Last Modified: Fri, 24 Apr 2020 21:57:32 GMT  
		Size: 183.2 MB (183232276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:4.1.3`

```console
$ docker pull swift@sha256:3ff875313f89137f1f5ed122570c0221a888e00992cf43dd8dbd19b443c2fc98
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:4.1.3` - linux; amd64

```console
$ docker pull swift@sha256:1b6d2ac9677206b94c22349f8eaf8d586574e9b27e1359a752d53cc3f2ac89be
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **451.9 MB (451937473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13ca9d5b6955d631e265a63efb3a798f7f5d3cdfe2c62e12be71a5f910081269`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:45:15 GMT
LABEL maintainer=Haris Amin <aminharis7@gmail.com>
# Fri, 24 Apr 2020 21:45:16 GMT
LABEL Description=Docker Container for the Apple's Swift programming language
# Fri, 24 Apr 2020 21:46:04 GMT
RUN apt-get -q update &&     apt-get -q install -y     make     libc6-dev     clang-3.8     curl     libedit-dev     libpython2.7     libicu-dev     libssl-dev     libxml2     tzdata     git     libcurl4-openssl-dev     pkg-config     && update-alternatives --quiet --install /usr/bin/clang clang /usr/bin/clang-3.8 100     && update-alternatives --quiet --install /usr/bin/clang++ clang++ /usr/bin/clang++-3.8 100     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:46:05 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Fri, 24 Apr 2020 21:46:05 GMT
ARG SWIFT_BRANCH=swift-4.1.3-release
# Fri, 24 Apr 2020 21:46:05 GMT
ARG SWIFT_VERSION=swift-4.1.3-RELEASE
# Fri, 24 Apr 2020 21:46:05 GMT
ENV SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-4.1.3-release SWIFT_VERSION=swift-4.1.3-RELEASE
# Fri, 24 Apr 2020 21:46:43 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           8513444E2DA36B7C1659AF4D7638F1FB2B2B08C4           A3BAFD3556A59079C06894BD63BC1CFE91D306C6           5E4DF843FB065D7F7E24FBA2EF5430F071E1B235         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
# Fri, 24 Apr 2020 21:46:44 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e921f1e439c9e57e62899f6fccec9d2b228278e575d90e5faa1e506b9ef9a11f`  
		Last Modified: Fri, 24 Apr 2020 21:57:41 GMT  
		Size: 224.5 MB (224456516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9527d39e2432b1d6742c4d0a1b916e51cb045c77149d2e4b92a7db86a785c8d8`  
		Last Modified: Fri, 24 Apr 2020 21:57:32 GMT  
		Size: 183.2 MB (183232276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:4.2`

```console
$ docker pull swift@sha256:0b3e72a5af09f93983e4029ef9653a406bb0349e313ca809d3a0d341b90dd736
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:4.2` - linux; amd64

```console
$ docker pull swift@sha256:62508fb30694d78efa386497b7b17158568493a4dff2ac512702f7afe6decfb2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **496.9 MB (496870900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6a86a74b4ad3e5430c72f5fe640913d1305207c41e4fc1b0ed38e7fc86831a6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:25:51 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 24 Apr 2020 21:25:51 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 24 Apr 2020 21:44:25 GMT
RUN apt-get -q update &&     apt-get -q install -y     make     libc6-dev     clang-3.8     curl     libedit-dev     libpython2.7     libicu-dev     libssl-dev     libxml2     tzdata     git     libcurl4-openssl-dev     pkg-config     && update-alternatives --quiet --install /usr/bin/clang clang /usr/bin/clang-3.8 100     && update-alternatives --quiet --install /usr/bin/clang++ clang++ /usr/bin/clang++-3.8 100     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:44:25 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Fri, 24 Apr 2020 21:44:26 GMT
ARG SWIFT_BRANCH=swift-4.2.4-release
# Fri, 24 Apr 2020 21:44:26 GMT
ARG SWIFT_VERSION=swift-4.2.4-RELEASE
# Fri, 24 Apr 2020 21:44:26 GMT
ENV SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-4.2.4-release SWIFT_VERSION=swift-4.2.4-RELEASE
# Fri, 24 Apr 2020 21:45:10 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           8513444E2DA36B7C1659AF4D7638F1FB2B2B08C4           A3BAFD3556A59079C06894BD63BC1CFE91D306C6           5E4DF843FB065D7F7E24FBA2EF5430F071E1B235         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
# Fri, 24 Apr 2020 21:45:11 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb47c322eeb3f3831495f380f3f3c5fa87d32146dfe5d1fc73331e6b0c0fca9`  
		Last Modified: Fri, 24 Apr 2020 21:56:49 GMT  
		Size: 224.5 MB (224456061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af86238a5645c7753125cdd883cb6693f059ca3a44804705401ce014c5fe35c7`  
		Last Modified: Fri, 24 Apr 2020 21:56:49 GMT  
		Size: 228.2 MB (228166158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:4.2.4`

```console
$ docker pull swift@sha256:0b3e72a5af09f93983e4029ef9653a406bb0349e313ca809d3a0d341b90dd736
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:4.2.4` - linux; amd64

```console
$ docker pull swift@sha256:62508fb30694d78efa386497b7b17158568493a4dff2ac512702f7afe6decfb2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **496.9 MB (496870900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6a86a74b4ad3e5430c72f5fe640913d1305207c41e4fc1b0ed38e7fc86831a6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:25:51 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 24 Apr 2020 21:25:51 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 24 Apr 2020 21:44:25 GMT
RUN apt-get -q update &&     apt-get -q install -y     make     libc6-dev     clang-3.8     curl     libedit-dev     libpython2.7     libicu-dev     libssl-dev     libxml2     tzdata     git     libcurl4-openssl-dev     pkg-config     && update-alternatives --quiet --install /usr/bin/clang clang /usr/bin/clang-3.8 100     && update-alternatives --quiet --install /usr/bin/clang++ clang++ /usr/bin/clang++-3.8 100     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:44:25 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Fri, 24 Apr 2020 21:44:26 GMT
ARG SWIFT_BRANCH=swift-4.2.4-release
# Fri, 24 Apr 2020 21:44:26 GMT
ARG SWIFT_VERSION=swift-4.2.4-RELEASE
# Fri, 24 Apr 2020 21:44:26 GMT
ENV SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-4.2.4-release SWIFT_VERSION=swift-4.2.4-RELEASE
# Fri, 24 Apr 2020 21:45:10 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           8513444E2DA36B7C1659AF4D7638F1FB2B2B08C4           A3BAFD3556A59079C06894BD63BC1CFE91D306C6           5E4DF843FB065D7F7E24FBA2EF5430F071E1B235         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
# Fri, 24 Apr 2020 21:45:11 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb47c322eeb3f3831495f380f3f3c5fa87d32146dfe5d1fc73331e6b0c0fca9`  
		Last Modified: Fri, 24 Apr 2020 21:56:49 GMT  
		Size: 224.5 MB (224456061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af86238a5645c7753125cdd883cb6693f059ca3a44804705401ce014c5fe35c7`  
		Last Modified: Fri, 24 Apr 2020 21:56:49 GMT  
		Size: 228.2 MB (228166158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.0`

```console
$ docker pull swift@sha256:e07593eea016a48efda0051b53838ad3e26e752107b3944c0a0ef13389a7be14
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.0` - linux; amd64

```console
$ docker pull swift@sha256:3bb4d10f13035efc16d1ff405a18fe8684c8411d1bb433972cabe42916568863
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **470.2 MB (470210656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4544d3cabf5e087463856e83bc6fbea6c85c2e864d5fb664caa1522bfcd1407`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:07:00 GMT
ADD file:c3e6bb316dfa6b81dd4478aaa310df532883b1c0a14edeec3f63d641980c1789 in / 
# Fri, 24 Apr 2020 01:07:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 01:07:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:07:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:07:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 24 Apr 2020 21:37:45 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libbsd0     libcurl4     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:37:45 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Fri, 24 Apr 2020 21:37:45 GMT
ARG SWIFT_BRANCH=swift-5.0.3-release
# Fri, 24 Apr 2020 21:37:45 GMT
ARG SWIFT_VERSION=swift-5.0.3-RELEASE
# Fri, 24 Apr 2020 21:37:46 GMT
ENV SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.0.3-release SWIFT_VERSION=swift-5.0.3-RELEASE
# Fri, 24 Apr 2020 21:38:50 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && apt-get update     && apt-get install -y curl     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && apt-get purge -y curl     && apt-get -y autoremove     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           A62AE125BBBFBB96A6E042EC925CC1CCED3D1561         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
# Fri, 24 Apr 2020 21:38:51 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:23884877105a7ff84a910895cd044061a4561385ff6c36480ee080b76ec0e771`  
		Last Modified: Sat, 04 Apr 2020 12:21:10 GMT  
		Size: 26.7 MB (26689802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc38caa0f5b94141276220daaf428892096e4afd24b05668cd188311e00a635f`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 35.4 KB (35367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2910811b6c4227c2f42aaea9a3dd5f53b1d469f67e2cf7e601f631b119b61ff7`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36505266dcc64eeb1010bd2112e6f73981e1a8246e4f6d4e287763b57f101b0b`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e142b8b06167b57f80b70748c7c3c08e018f9a597c970b07e70ae3d8b61d12`  
		Last Modified: Fri, 24 Apr 2020 21:54:07 GMT  
		Size: 124.0 MB (123977961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9462c32df41222ce4b6be7b39897de97bdb6761648158bbef5fc9e59197b56a`  
		Last Modified: Fri, 24 Apr 2020 21:54:35 GMT  
		Size: 319.5 MB (319506518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.0.3`

```console
$ docker pull swift@sha256:e07593eea016a48efda0051b53838ad3e26e752107b3944c0a0ef13389a7be14
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.0.3` - linux; amd64

```console
$ docker pull swift@sha256:3bb4d10f13035efc16d1ff405a18fe8684c8411d1bb433972cabe42916568863
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **470.2 MB (470210656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4544d3cabf5e087463856e83bc6fbea6c85c2e864d5fb664caa1522bfcd1407`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:07:00 GMT
ADD file:c3e6bb316dfa6b81dd4478aaa310df532883b1c0a14edeec3f63d641980c1789 in / 
# Fri, 24 Apr 2020 01:07:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 01:07:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:07:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:07:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 24 Apr 2020 21:37:45 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libbsd0     libcurl4     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:37:45 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Fri, 24 Apr 2020 21:37:45 GMT
ARG SWIFT_BRANCH=swift-5.0.3-release
# Fri, 24 Apr 2020 21:37:45 GMT
ARG SWIFT_VERSION=swift-5.0.3-RELEASE
# Fri, 24 Apr 2020 21:37:46 GMT
ENV SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.0.3-release SWIFT_VERSION=swift-5.0.3-RELEASE
# Fri, 24 Apr 2020 21:38:50 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && apt-get update     && apt-get install -y curl     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && apt-get purge -y curl     && apt-get -y autoremove     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           A62AE125BBBFBB96A6E042EC925CC1CCED3D1561         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
# Fri, 24 Apr 2020 21:38:51 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:23884877105a7ff84a910895cd044061a4561385ff6c36480ee080b76ec0e771`  
		Last Modified: Sat, 04 Apr 2020 12:21:10 GMT  
		Size: 26.7 MB (26689802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc38caa0f5b94141276220daaf428892096e4afd24b05668cd188311e00a635f`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 35.4 KB (35367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2910811b6c4227c2f42aaea9a3dd5f53b1d469f67e2cf7e601f631b119b61ff7`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36505266dcc64eeb1010bd2112e6f73981e1a8246e4f6d4e287763b57f101b0b`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e142b8b06167b57f80b70748c7c3c08e018f9a597c970b07e70ae3d8b61d12`  
		Last Modified: Fri, 24 Apr 2020 21:54:07 GMT  
		Size: 124.0 MB (123977961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9462c32df41222ce4b6be7b39897de97bdb6761648158bbef5fc9e59197b56a`  
		Last Modified: Fri, 24 Apr 2020 21:54:35 GMT  
		Size: 319.5 MB (319506518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.0.3-bionic`

```console
$ docker pull swift@sha256:e07593eea016a48efda0051b53838ad3e26e752107b3944c0a0ef13389a7be14
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.0.3-bionic` - linux; amd64

```console
$ docker pull swift@sha256:3bb4d10f13035efc16d1ff405a18fe8684c8411d1bb433972cabe42916568863
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **470.2 MB (470210656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4544d3cabf5e087463856e83bc6fbea6c85c2e864d5fb664caa1522bfcd1407`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:07:00 GMT
ADD file:c3e6bb316dfa6b81dd4478aaa310df532883b1c0a14edeec3f63d641980c1789 in / 
# Fri, 24 Apr 2020 01:07:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 01:07:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:07:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:07:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 24 Apr 2020 21:37:45 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libbsd0     libcurl4     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:37:45 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Fri, 24 Apr 2020 21:37:45 GMT
ARG SWIFT_BRANCH=swift-5.0.3-release
# Fri, 24 Apr 2020 21:37:45 GMT
ARG SWIFT_VERSION=swift-5.0.3-RELEASE
# Fri, 24 Apr 2020 21:37:46 GMT
ENV SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.0.3-release SWIFT_VERSION=swift-5.0.3-RELEASE
# Fri, 24 Apr 2020 21:38:50 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && apt-get update     && apt-get install -y curl     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && apt-get purge -y curl     && apt-get -y autoremove     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           A62AE125BBBFBB96A6E042EC925CC1CCED3D1561         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
# Fri, 24 Apr 2020 21:38:51 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:23884877105a7ff84a910895cd044061a4561385ff6c36480ee080b76ec0e771`  
		Last Modified: Sat, 04 Apr 2020 12:21:10 GMT  
		Size: 26.7 MB (26689802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc38caa0f5b94141276220daaf428892096e4afd24b05668cd188311e00a635f`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 35.4 KB (35367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2910811b6c4227c2f42aaea9a3dd5f53b1d469f67e2cf7e601f631b119b61ff7`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36505266dcc64eeb1010bd2112e6f73981e1a8246e4f6d4e287763b57f101b0b`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e142b8b06167b57f80b70748c7c3c08e018f9a597c970b07e70ae3d8b61d12`  
		Last Modified: Fri, 24 Apr 2020 21:54:07 GMT  
		Size: 124.0 MB (123977961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9462c32df41222ce4b6be7b39897de97bdb6761648158bbef5fc9e59197b56a`  
		Last Modified: Fri, 24 Apr 2020 21:54:35 GMT  
		Size: 319.5 MB (319506518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.0.3-bionic-slim`

```console
$ docker pull swift@sha256:cffaf634a13e75fc87a58c4c2387470238e221245b21982091fec54d9b3bfdcb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.0.3-bionic-slim` - linux; amd64

```console
$ docker pull swift@sha256:5b2b923229b11ab2510dfd98593613c6f9fa12b7cfccb52895c10735968da4d0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75160033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10c4afb483dfccfbae142426cfef4a82f181d0c2aa4ee219ea1f65a67305ae64`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:07:00 GMT
ADD file:c3e6bb316dfa6b81dd4478aaa310df532883b1c0a14edeec3f63d641980c1789 in / 
# Fri, 24 Apr 2020 01:07:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 01:07:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:07:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:07:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 24 Apr 2020 21:41:07 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libbsd0     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:41:07 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Fri, 24 Apr 2020 21:41:08 GMT
ARG SWIFT_BRANCH=swift-5.0.3-release
# Fri, 24 Apr 2020 21:41:08 GMT
ARG SWIFT_VERSION=swift-5.0.3-RELEASE
# Fri, 24 Apr 2020 21:41:08 GMT
ENV SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.0.3-release SWIFT_VERSION=swift-5.0.3-RELEASE
# Fri, 24 Apr 2020 21:42:09 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && apt-get update     && apt-get install -y curl gpg     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           A62AE125BBBFBB96A6E042EC925CC1CCED3D1561         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && apt-get purge -y curl gpg     && apt-get -y autoremove     && rm -r /var/lib/apt/lists/*     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
```

-	Layers:
	-	`sha256:23884877105a7ff84a910895cd044061a4561385ff6c36480ee080b76ec0e771`  
		Last Modified: Sat, 04 Apr 2020 12:21:10 GMT  
		Size: 26.7 MB (26689802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc38caa0f5b94141276220daaf428892096e4afd24b05668cd188311e00a635f`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 35.4 KB (35367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2910811b6c4227c2f42aaea9a3dd5f53b1d469f67e2cf7e601f631b119b61ff7`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36505266dcc64eeb1010bd2112e6f73981e1a8246e4f6d4e287763b57f101b0b`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2640ac56e0f664dc9727c8f656d8391b7494749fe6951fb6df417cec54c1165`  
		Last Modified: Fri, 24 Apr 2020 21:55:46 GMT  
		Size: 20.5 MB (20535152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ea0fb732e6023e9c57ba3472e271f258036a74db113118aaa0dd4490895694`  
		Last Modified: Fri, 24 Apr 2020 21:55:47 GMT  
		Size: 27.9 MB (27898704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.0.3-slim`

```console
$ docker pull swift@sha256:cffaf634a13e75fc87a58c4c2387470238e221245b21982091fec54d9b3bfdcb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.0.3-slim` - linux; amd64

```console
$ docker pull swift@sha256:5b2b923229b11ab2510dfd98593613c6f9fa12b7cfccb52895c10735968da4d0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75160033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10c4afb483dfccfbae142426cfef4a82f181d0c2aa4ee219ea1f65a67305ae64`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:07:00 GMT
ADD file:c3e6bb316dfa6b81dd4478aaa310df532883b1c0a14edeec3f63d641980c1789 in / 
# Fri, 24 Apr 2020 01:07:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 01:07:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:07:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:07:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 24 Apr 2020 21:41:07 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libbsd0     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:41:07 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Fri, 24 Apr 2020 21:41:08 GMT
ARG SWIFT_BRANCH=swift-5.0.3-release
# Fri, 24 Apr 2020 21:41:08 GMT
ARG SWIFT_VERSION=swift-5.0.3-RELEASE
# Fri, 24 Apr 2020 21:41:08 GMT
ENV SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.0.3-release SWIFT_VERSION=swift-5.0.3-RELEASE
# Fri, 24 Apr 2020 21:42:09 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && apt-get update     && apt-get install -y curl gpg     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           A62AE125BBBFBB96A6E042EC925CC1CCED3D1561         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && apt-get purge -y curl gpg     && apt-get -y autoremove     && rm -r /var/lib/apt/lists/*     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
```

-	Layers:
	-	`sha256:23884877105a7ff84a910895cd044061a4561385ff6c36480ee080b76ec0e771`  
		Last Modified: Sat, 04 Apr 2020 12:21:10 GMT  
		Size: 26.7 MB (26689802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc38caa0f5b94141276220daaf428892096e4afd24b05668cd188311e00a635f`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 35.4 KB (35367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2910811b6c4227c2f42aaea9a3dd5f53b1d469f67e2cf7e601f631b119b61ff7`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36505266dcc64eeb1010bd2112e6f73981e1a8246e4f6d4e287763b57f101b0b`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2640ac56e0f664dc9727c8f656d8391b7494749fe6951fb6df417cec54c1165`  
		Last Modified: Fri, 24 Apr 2020 21:55:46 GMT  
		Size: 20.5 MB (20535152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ea0fb732e6023e9c57ba3472e271f258036a74db113118aaa0dd4490895694`  
		Last Modified: Fri, 24 Apr 2020 21:55:47 GMT  
		Size: 27.9 MB (27898704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.0.3-xenial`

```console
$ docker pull swift@sha256:0e3ff4ec52e9dd9864b3746af424f9bda1efd61bffb883f56926ba3e168ee6d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.0.3-xenial` - linux; amd64

```console
$ docker pull swift@sha256:da011f15d24e34cf45e3b75cfe447175ff856a763eba6ae45db3d096894bbf2e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **478.2 MB (478201907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:945f2ebaba031046210fe7484ecc914c17dbcfab3e29d45d5ca5d155d62c1b88`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:25:51 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 24 Apr 2020 21:25:51 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 24 Apr 2020 21:39:32 GMT
RUN apt-get -q update &&     apt-get -q install -y     libatomic1     libbsd0     libcurl3     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:39:33 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Fri, 24 Apr 2020 21:39:33 GMT
ARG SWIFT_BRANCH=swift-5.0.3-release
# Fri, 24 Apr 2020 21:39:33 GMT
ARG SWIFT_VERSION=swift-5.0.3-RELEASE
# Fri, 24 Apr 2020 21:39:33 GMT
ENV SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-5.0.3-release SWIFT_VERSION=swift-5.0.3-RELEASE
# Fri, 24 Apr 2020 21:40:47 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && apt-get -q update     && apt-get -q install -y curl     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && apt-get purge -y curl     && apt-get -y autoremove     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           A62AE125BBBFBB96A6E042EC925CC1CCED3D1561         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
# Fri, 24 Apr 2020 21:40:49 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ad3b5f4abe148570dad4c6f0ce493e1c03f9b491366b767d97459bc18ea3b6`  
		Last Modified: Fri, 24 Apr 2020 21:55:05 GMT  
		Size: 111.4 MB (111384949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c6ae28090be18c2b2d24c49e866fc106d518596d3cf031cea5f5a0008bd86b`  
		Last Modified: Fri, 24 Apr 2020 21:55:38 GMT  
		Size: 322.6 MB (322568277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.0.3-xenial-slim`

```console
$ docker pull swift@sha256:0654b2ad0dc62e52106b4472fc71f7826aa7ef609b6761201914b82e9b503c12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.0.3-xenial-slim` - linux; amd64

```console
$ docker pull swift@sha256:0acc100147386e65c2306f6edd84ba9bfc37d6e82f83094d8f236438fb0b761a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.0 MB (92960345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:960c926d6686ad580b3fb06a692483b20509a070d48c6f507637a8bb265b3cd2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:25:51 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 24 Apr 2020 21:25:51 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 24 Apr 2020 21:42:24 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libbsd0     libcurl3     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:42:25 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Fri, 24 Apr 2020 21:42:25 GMT
ARG SWIFT_BRANCH=swift-5.0.3-release
# Fri, 24 Apr 2020 21:42:25 GMT
ARG SWIFT_VERSION=swift-5.0.3-RELEASE
# Fri, 24 Apr 2020 21:42:25 GMT
ENV SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-5.0.3-release SWIFT_VERSION=swift-5.0.3-RELEASE
# Fri, 24 Apr 2020 21:43:24 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && apt-get update     && apt-get install -y curl     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           A62AE125BBBFBB96A6E042EC925CC1CCED3D1561         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && apt-get purge -y curl     && apt-get -y autoremove     && rm -r /var/lib/apt/lists/*     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1af1171977fa90eb39537bbfff424f97aa0e5379689e876c82e36b69933109c`  
		Last Modified: Fri, 24 Apr 2020 21:55:58 GMT  
		Size: 20.9 MB (20926021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef52b5e33312643b5814b8e731e7f72a1aef5374a6bafe3a2cd1829423b1b7c`  
		Last Modified: Fri, 24 Apr 2020 21:55:59 GMT  
		Size: 27.8 MB (27785643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.0-bionic`

```console
$ docker pull swift@sha256:e07593eea016a48efda0051b53838ad3e26e752107b3944c0a0ef13389a7be14
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.0-bionic` - linux; amd64

```console
$ docker pull swift@sha256:3bb4d10f13035efc16d1ff405a18fe8684c8411d1bb433972cabe42916568863
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **470.2 MB (470210656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4544d3cabf5e087463856e83bc6fbea6c85c2e864d5fb664caa1522bfcd1407`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:07:00 GMT
ADD file:c3e6bb316dfa6b81dd4478aaa310df532883b1c0a14edeec3f63d641980c1789 in / 
# Fri, 24 Apr 2020 01:07:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 01:07:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:07:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:07:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 24 Apr 2020 21:37:45 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libbsd0     libcurl4     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:37:45 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Fri, 24 Apr 2020 21:37:45 GMT
ARG SWIFT_BRANCH=swift-5.0.3-release
# Fri, 24 Apr 2020 21:37:45 GMT
ARG SWIFT_VERSION=swift-5.0.3-RELEASE
# Fri, 24 Apr 2020 21:37:46 GMT
ENV SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.0.3-release SWIFT_VERSION=swift-5.0.3-RELEASE
# Fri, 24 Apr 2020 21:38:50 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && apt-get update     && apt-get install -y curl     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && apt-get purge -y curl     && apt-get -y autoremove     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           A62AE125BBBFBB96A6E042EC925CC1CCED3D1561         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
# Fri, 24 Apr 2020 21:38:51 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:23884877105a7ff84a910895cd044061a4561385ff6c36480ee080b76ec0e771`  
		Last Modified: Sat, 04 Apr 2020 12:21:10 GMT  
		Size: 26.7 MB (26689802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc38caa0f5b94141276220daaf428892096e4afd24b05668cd188311e00a635f`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 35.4 KB (35367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2910811b6c4227c2f42aaea9a3dd5f53b1d469f67e2cf7e601f631b119b61ff7`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36505266dcc64eeb1010bd2112e6f73981e1a8246e4f6d4e287763b57f101b0b`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e142b8b06167b57f80b70748c7c3c08e018f9a597c970b07e70ae3d8b61d12`  
		Last Modified: Fri, 24 Apr 2020 21:54:07 GMT  
		Size: 124.0 MB (123977961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9462c32df41222ce4b6be7b39897de97bdb6761648158bbef5fc9e59197b56a`  
		Last Modified: Fri, 24 Apr 2020 21:54:35 GMT  
		Size: 319.5 MB (319506518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.0-bionic-slim`

```console
$ docker pull swift@sha256:cffaf634a13e75fc87a58c4c2387470238e221245b21982091fec54d9b3bfdcb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.0-bionic-slim` - linux; amd64

```console
$ docker pull swift@sha256:5b2b923229b11ab2510dfd98593613c6f9fa12b7cfccb52895c10735968da4d0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75160033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10c4afb483dfccfbae142426cfef4a82f181d0c2aa4ee219ea1f65a67305ae64`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:07:00 GMT
ADD file:c3e6bb316dfa6b81dd4478aaa310df532883b1c0a14edeec3f63d641980c1789 in / 
# Fri, 24 Apr 2020 01:07:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 01:07:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:07:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:07:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 24 Apr 2020 21:41:07 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libbsd0     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:41:07 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Fri, 24 Apr 2020 21:41:08 GMT
ARG SWIFT_BRANCH=swift-5.0.3-release
# Fri, 24 Apr 2020 21:41:08 GMT
ARG SWIFT_VERSION=swift-5.0.3-RELEASE
# Fri, 24 Apr 2020 21:41:08 GMT
ENV SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.0.3-release SWIFT_VERSION=swift-5.0.3-RELEASE
# Fri, 24 Apr 2020 21:42:09 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && apt-get update     && apt-get install -y curl gpg     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           A62AE125BBBFBB96A6E042EC925CC1CCED3D1561         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && apt-get purge -y curl gpg     && apt-get -y autoremove     && rm -r /var/lib/apt/lists/*     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
```

-	Layers:
	-	`sha256:23884877105a7ff84a910895cd044061a4561385ff6c36480ee080b76ec0e771`  
		Last Modified: Sat, 04 Apr 2020 12:21:10 GMT  
		Size: 26.7 MB (26689802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc38caa0f5b94141276220daaf428892096e4afd24b05668cd188311e00a635f`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 35.4 KB (35367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2910811b6c4227c2f42aaea9a3dd5f53b1d469f67e2cf7e601f631b119b61ff7`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36505266dcc64eeb1010bd2112e6f73981e1a8246e4f6d4e287763b57f101b0b`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2640ac56e0f664dc9727c8f656d8391b7494749fe6951fb6df417cec54c1165`  
		Last Modified: Fri, 24 Apr 2020 21:55:46 GMT  
		Size: 20.5 MB (20535152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ea0fb732e6023e9c57ba3472e271f258036a74db113118aaa0dd4490895694`  
		Last Modified: Fri, 24 Apr 2020 21:55:47 GMT  
		Size: 27.9 MB (27898704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.0-slim`

```console
$ docker pull swift@sha256:cffaf634a13e75fc87a58c4c2387470238e221245b21982091fec54d9b3bfdcb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.0-slim` - linux; amd64

```console
$ docker pull swift@sha256:5b2b923229b11ab2510dfd98593613c6f9fa12b7cfccb52895c10735968da4d0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75160033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10c4afb483dfccfbae142426cfef4a82f181d0c2aa4ee219ea1f65a67305ae64`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:07:00 GMT
ADD file:c3e6bb316dfa6b81dd4478aaa310df532883b1c0a14edeec3f63d641980c1789 in / 
# Fri, 24 Apr 2020 01:07:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 01:07:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:07:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:07:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 24 Apr 2020 21:41:07 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libbsd0     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:41:07 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Fri, 24 Apr 2020 21:41:08 GMT
ARG SWIFT_BRANCH=swift-5.0.3-release
# Fri, 24 Apr 2020 21:41:08 GMT
ARG SWIFT_VERSION=swift-5.0.3-RELEASE
# Fri, 24 Apr 2020 21:41:08 GMT
ENV SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.0.3-release SWIFT_VERSION=swift-5.0.3-RELEASE
# Fri, 24 Apr 2020 21:42:09 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && apt-get update     && apt-get install -y curl gpg     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           A62AE125BBBFBB96A6E042EC925CC1CCED3D1561         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && apt-get purge -y curl gpg     && apt-get -y autoremove     && rm -r /var/lib/apt/lists/*     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
```

-	Layers:
	-	`sha256:23884877105a7ff84a910895cd044061a4561385ff6c36480ee080b76ec0e771`  
		Last Modified: Sat, 04 Apr 2020 12:21:10 GMT  
		Size: 26.7 MB (26689802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc38caa0f5b94141276220daaf428892096e4afd24b05668cd188311e00a635f`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 35.4 KB (35367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2910811b6c4227c2f42aaea9a3dd5f53b1d469f67e2cf7e601f631b119b61ff7`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36505266dcc64eeb1010bd2112e6f73981e1a8246e4f6d4e287763b57f101b0b`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2640ac56e0f664dc9727c8f656d8391b7494749fe6951fb6df417cec54c1165`  
		Last Modified: Fri, 24 Apr 2020 21:55:46 GMT  
		Size: 20.5 MB (20535152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ea0fb732e6023e9c57ba3472e271f258036a74db113118aaa0dd4490895694`  
		Last Modified: Fri, 24 Apr 2020 21:55:47 GMT  
		Size: 27.9 MB (27898704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.0-xenial`

```console
$ docker pull swift@sha256:0e3ff4ec52e9dd9864b3746af424f9bda1efd61bffb883f56926ba3e168ee6d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.0-xenial` - linux; amd64

```console
$ docker pull swift@sha256:da011f15d24e34cf45e3b75cfe447175ff856a763eba6ae45db3d096894bbf2e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **478.2 MB (478201907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:945f2ebaba031046210fe7484ecc914c17dbcfab3e29d45d5ca5d155d62c1b88`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:25:51 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 24 Apr 2020 21:25:51 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 24 Apr 2020 21:39:32 GMT
RUN apt-get -q update &&     apt-get -q install -y     libatomic1     libbsd0     libcurl3     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:39:33 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Fri, 24 Apr 2020 21:39:33 GMT
ARG SWIFT_BRANCH=swift-5.0.3-release
# Fri, 24 Apr 2020 21:39:33 GMT
ARG SWIFT_VERSION=swift-5.0.3-RELEASE
# Fri, 24 Apr 2020 21:39:33 GMT
ENV SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-5.0.3-release SWIFT_VERSION=swift-5.0.3-RELEASE
# Fri, 24 Apr 2020 21:40:47 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && apt-get -q update     && apt-get -q install -y curl     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && apt-get purge -y curl     && apt-get -y autoremove     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           A62AE125BBBFBB96A6E042EC925CC1CCED3D1561         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
# Fri, 24 Apr 2020 21:40:49 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ad3b5f4abe148570dad4c6f0ce493e1c03f9b491366b767d97459bc18ea3b6`  
		Last Modified: Fri, 24 Apr 2020 21:55:05 GMT  
		Size: 111.4 MB (111384949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c6ae28090be18c2b2d24c49e866fc106d518596d3cf031cea5f5a0008bd86b`  
		Last Modified: Fri, 24 Apr 2020 21:55:38 GMT  
		Size: 322.6 MB (322568277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.0-xenial-slim`

```console
$ docker pull swift@sha256:0654b2ad0dc62e52106b4472fc71f7826aa7ef609b6761201914b82e9b503c12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.0-xenial-slim` - linux; amd64

```console
$ docker pull swift@sha256:0acc100147386e65c2306f6edd84ba9bfc37d6e82f83094d8f236438fb0b761a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.0 MB (92960345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:960c926d6686ad580b3fb06a692483b20509a070d48c6f507637a8bb265b3cd2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:25:51 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 24 Apr 2020 21:25:51 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 24 Apr 2020 21:42:24 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libbsd0     libcurl3     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:42:25 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Fri, 24 Apr 2020 21:42:25 GMT
ARG SWIFT_BRANCH=swift-5.0.3-release
# Fri, 24 Apr 2020 21:42:25 GMT
ARG SWIFT_VERSION=swift-5.0.3-RELEASE
# Fri, 24 Apr 2020 21:42:25 GMT
ENV SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-5.0.3-release SWIFT_VERSION=swift-5.0.3-RELEASE
# Fri, 24 Apr 2020 21:43:24 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && apt-get update     && apt-get install -y curl     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           A62AE125BBBFBB96A6E042EC925CC1CCED3D1561         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && apt-get purge -y curl     && apt-get -y autoremove     && rm -r /var/lib/apt/lists/*     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1af1171977fa90eb39537bbfff424f97aa0e5379689e876c82e36b69933109c`  
		Last Modified: Fri, 24 Apr 2020 21:55:58 GMT  
		Size: 20.9 MB (20926021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef52b5e33312643b5814b8e731e7f72a1aef5374a6bafe3a2cd1829423b1b7c`  
		Last Modified: Fri, 24 Apr 2020 21:55:59 GMT  
		Size: 27.8 MB (27785643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.1`

```console
$ docker pull swift@sha256:c66c8ea0b3f93f1ab438b0ce70f2065d37b0d1c6052a8299cead7208ddfbf7de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.1` - linux; amd64

```console
$ docker pull swift@sha256:d3450c154de8ee175c575a6c3a467be52498bb16ff5af30e02850941d2bb869c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **496.0 MB (495970701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5b1eefae081057ddfe64b1d6fbd0cf340adc0ca7a3eb1e44f31596086d3b708`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:07:00 GMT
ADD file:c3e6bb316dfa6b81dd4478aaa310df532883b1c0a14edeec3f63d641980c1789 in / 
# Fri, 24 Apr 2020 01:07:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 01:07:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:07:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:07:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 24 Apr 2020 21:24:10 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:24:11 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 24 Apr 2020 21:24:11 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Fri, 24 Apr 2020 21:31:38 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Fri, 24 Apr 2020 21:31:38 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Fri, 24 Apr 2020 21:31:38 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:31:38 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:32:49 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Fri, 24 Apr 2020 21:32:55 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:23884877105a7ff84a910895cd044061a4561385ff6c36480ee080b76ec0e771`  
		Last Modified: Sat, 04 Apr 2020 12:21:10 GMT  
		Size: 26.7 MB (26689802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc38caa0f5b94141276220daaf428892096e4afd24b05668cd188311e00a635f`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 35.4 KB (35367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2910811b6c4227c2f42aaea9a3dd5f53b1d469f67e2cf7e601f631b119b61ff7`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36505266dcc64eeb1010bd2112e6f73981e1a8246e4f6d4e287763b57f101b0b`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25035e7374ff2fcd78ec35d5d95a9e4587422b205f1c630ae8078085434d5b86`  
		Last Modified: Fri, 24 Apr 2020 21:48:23 GMT  
		Size: 124.1 MB (124077069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d932e2e7c39b531ec37ce74db6da19a5373cf4714a82b93f8e2d0b609721426`  
		Last Modified: Fri, 24 Apr 2020 21:51:53 GMT  
		Size: 345.2 MB (345167455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.1.5`

```console
$ docker pull swift@sha256:c66c8ea0b3f93f1ab438b0ce70f2065d37b0d1c6052a8299cead7208ddfbf7de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.1.5` - linux; amd64

```console
$ docker pull swift@sha256:d3450c154de8ee175c575a6c3a467be52498bb16ff5af30e02850941d2bb869c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **496.0 MB (495970701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5b1eefae081057ddfe64b1d6fbd0cf340adc0ca7a3eb1e44f31596086d3b708`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:07:00 GMT
ADD file:c3e6bb316dfa6b81dd4478aaa310df532883b1c0a14edeec3f63d641980c1789 in / 
# Fri, 24 Apr 2020 01:07:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 01:07:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:07:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:07:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 24 Apr 2020 21:24:10 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:24:11 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 24 Apr 2020 21:24:11 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Fri, 24 Apr 2020 21:31:38 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Fri, 24 Apr 2020 21:31:38 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Fri, 24 Apr 2020 21:31:38 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:31:38 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:32:49 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Fri, 24 Apr 2020 21:32:55 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:23884877105a7ff84a910895cd044061a4561385ff6c36480ee080b76ec0e771`  
		Last Modified: Sat, 04 Apr 2020 12:21:10 GMT  
		Size: 26.7 MB (26689802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc38caa0f5b94141276220daaf428892096e4afd24b05668cd188311e00a635f`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 35.4 KB (35367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2910811b6c4227c2f42aaea9a3dd5f53b1d469f67e2cf7e601f631b119b61ff7`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36505266dcc64eeb1010bd2112e6f73981e1a8246e4f6d4e287763b57f101b0b`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25035e7374ff2fcd78ec35d5d95a9e4587422b205f1c630ae8078085434d5b86`  
		Last Modified: Fri, 24 Apr 2020 21:48:23 GMT  
		Size: 124.1 MB (124077069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d932e2e7c39b531ec37ce74db6da19a5373cf4714a82b93f8e2d0b609721426`  
		Last Modified: Fri, 24 Apr 2020 21:51:53 GMT  
		Size: 345.2 MB (345167455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.1.5-bionic`

```console
$ docker pull swift@sha256:c66c8ea0b3f93f1ab438b0ce70f2065d37b0d1c6052a8299cead7208ddfbf7de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.1.5-bionic` - linux; amd64

```console
$ docker pull swift@sha256:d3450c154de8ee175c575a6c3a467be52498bb16ff5af30e02850941d2bb869c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **496.0 MB (495970701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5b1eefae081057ddfe64b1d6fbd0cf340adc0ca7a3eb1e44f31596086d3b708`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:07:00 GMT
ADD file:c3e6bb316dfa6b81dd4478aaa310df532883b1c0a14edeec3f63d641980c1789 in / 
# Fri, 24 Apr 2020 01:07:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 01:07:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:07:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:07:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 24 Apr 2020 21:24:10 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:24:11 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 24 Apr 2020 21:24:11 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Fri, 24 Apr 2020 21:31:38 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Fri, 24 Apr 2020 21:31:38 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Fri, 24 Apr 2020 21:31:38 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:31:38 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:32:49 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Fri, 24 Apr 2020 21:32:55 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:23884877105a7ff84a910895cd044061a4561385ff6c36480ee080b76ec0e771`  
		Last Modified: Sat, 04 Apr 2020 12:21:10 GMT  
		Size: 26.7 MB (26689802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc38caa0f5b94141276220daaf428892096e4afd24b05668cd188311e00a635f`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 35.4 KB (35367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2910811b6c4227c2f42aaea9a3dd5f53b1d469f67e2cf7e601f631b119b61ff7`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36505266dcc64eeb1010bd2112e6f73981e1a8246e4f6d4e287763b57f101b0b`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25035e7374ff2fcd78ec35d5d95a9e4587422b205f1c630ae8078085434d5b86`  
		Last Modified: Fri, 24 Apr 2020 21:48:23 GMT  
		Size: 124.1 MB (124077069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d932e2e7c39b531ec37ce74db6da19a5373cf4714a82b93f8e2d0b609721426`  
		Last Modified: Fri, 24 Apr 2020 21:51:53 GMT  
		Size: 345.2 MB (345167455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.1.5-bionic-sim`

```console
$ docker pull swift@sha256:db74845e123fbfb430d1f309c63848603903e70ce01559a8e6f202bf90c8c25c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.1.5-bionic-sim` - linux; amd64

```console
$ docker pull swift@sha256:29ff1c9856daa9bda26bacf3a576b710049dc27b28bd1252d7beaebc5f751b15
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78297656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96878a4059b4f6e534cd57e2fbf70549ddbbe7955cd04b1f64be2955c506fb53`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:07:00 GMT
ADD file:c3e6bb316dfa6b81dd4478aaa310df532883b1c0a14edeec3f63d641980c1789 in / 
# Fri, 24 Apr 2020 01:07:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 01:07:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:07:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:07:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 24 Apr 2020 21:28:51 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:28:51 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 24 Apr 2020 21:28:51 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Fri, 24 Apr 2020 21:34:38 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Fri, 24 Apr 2020 21:34:38 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Fri, 24 Apr 2020 21:34:38 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:34:39 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:35:44 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl gnupg && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl gnupg
```

-	Layers:
	-	`sha256:23884877105a7ff84a910895cd044061a4561385ff6c36480ee080b76ec0e771`  
		Last Modified: Sat, 04 Apr 2020 12:21:10 GMT  
		Size: 26.7 MB (26689802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc38caa0f5b94141276220daaf428892096e4afd24b05668cd188311e00a635f`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 35.4 KB (35367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2910811b6c4227c2f42aaea9a3dd5f53b1d469f67e2cf7e601f631b119b61ff7`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36505266dcc64eeb1010bd2112e6f73981e1a8246e4f6d4e287763b57f101b0b`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44ab4793853bd7dece7450fb34472239255b43a04156f4c715f1e92ce766bef`  
		Last Modified: Fri, 24 Apr 2020 21:50:30 GMT  
		Size: 20.5 MB (20488873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:106512f011f225234c6120830f782e50d1dd5cf42ee5b9eca048c3d8f842743e`  
		Last Modified: Fri, 24 Apr 2020 21:53:25 GMT  
		Size: 31.1 MB (31082606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.1.5-slim`

```console
$ docker pull swift@sha256:db74845e123fbfb430d1f309c63848603903e70ce01559a8e6f202bf90c8c25c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.1.5-slim` - linux; amd64

```console
$ docker pull swift@sha256:29ff1c9856daa9bda26bacf3a576b710049dc27b28bd1252d7beaebc5f751b15
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78297656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96878a4059b4f6e534cd57e2fbf70549ddbbe7955cd04b1f64be2955c506fb53`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:07:00 GMT
ADD file:c3e6bb316dfa6b81dd4478aaa310df532883b1c0a14edeec3f63d641980c1789 in / 
# Fri, 24 Apr 2020 01:07:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 01:07:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:07:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:07:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 24 Apr 2020 21:28:51 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:28:51 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 24 Apr 2020 21:28:51 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Fri, 24 Apr 2020 21:34:38 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Fri, 24 Apr 2020 21:34:38 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Fri, 24 Apr 2020 21:34:38 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:34:39 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:35:44 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl gnupg && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl gnupg
```

-	Layers:
	-	`sha256:23884877105a7ff84a910895cd044061a4561385ff6c36480ee080b76ec0e771`  
		Last Modified: Sat, 04 Apr 2020 12:21:10 GMT  
		Size: 26.7 MB (26689802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc38caa0f5b94141276220daaf428892096e4afd24b05668cd188311e00a635f`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 35.4 KB (35367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2910811b6c4227c2f42aaea9a3dd5f53b1d469f67e2cf7e601f631b119b61ff7`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36505266dcc64eeb1010bd2112e6f73981e1a8246e4f6d4e287763b57f101b0b`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44ab4793853bd7dece7450fb34472239255b43a04156f4c715f1e92ce766bef`  
		Last Modified: Fri, 24 Apr 2020 21:50:30 GMT  
		Size: 20.5 MB (20488873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:106512f011f225234c6120830f782e50d1dd5cf42ee5b9eca048c3d8f842743e`  
		Last Modified: Fri, 24 Apr 2020 21:53:25 GMT  
		Size: 31.1 MB (31082606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.1.5-xenial`

```console
$ docker pull swift@sha256:40efc2c42bbceb3c21d77766502c4cd4cf021b0fc0bf89791d080ca42a9c309c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.1.5-xenial` - linux; amd64

```console
$ docker pull swift@sha256:c135bcd0299ae5582ca94a9d88a83821a30fedbaf7e804ac5813b149ab6597a8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **507.3 MB (507295529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b88d313c9ef80722cec830c650b6f932b9cb3a9caea4a06ae83d74517f33d3b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:25:51 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 24 Apr 2020 21:25:51 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 24 Apr 2020 21:26:57 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl3     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:26:58 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 24 Apr 2020 21:26:58 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Fri, 24 Apr 2020 21:33:08 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Fri, 24 Apr 2020 21:33:08 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Fri, 24 Apr 2020 21:33:08 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:33:08 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:34:19 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Fri, 24 Apr 2020 21:34:21 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6212d70001551edef31dfd8a0d9fa5e80793dbec6c744030626c8cc618939e70`  
		Last Modified: Fri, 24 Apr 2020 21:49:35 GMT  
		Size: 111.6 MB (111572008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aecae2b8a3fe16ad87f837b050ad742caeb047f8ab1bf0101a363ac0d35b719`  
		Last Modified: Fri, 24 Apr 2020 21:53:16 GMT  
		Size: 351.5 MB (351474840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.1.5-xenial-slim`

```console
$ docker pull swift@sha256:ccf876d6deeeb9a2ae6f552ee36df7393ad017a4010daa43a969bc5885766cc9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.1.5-xenial-slim` - linux; amd64

```console
$ docker pull swift@sha256:7f1c9516297f005378212b6b5437ccfccb683857cd2d582b7df05f1186eb7d19
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.1 MB (96075370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dea13627d66efc9d5a72704a3b30c5a5fc1f45b119b528b268dfe7b53c33e413`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:25:51 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 24 Apr 2020 21:25:51 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 24 Apr 2020 21:30:19 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl3     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:30:19 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 24 Apr 2020 21:30:19 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Fri, 24 Apr 2020 21:35:54 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Fri, 24 Apr 2020 21:35:54 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Fri, 24 Apr 2020 21:35:55 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:35:55 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:36:59 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89383f79d8ec0934f45345737e157e838789f001791fe3f5ef8b5f8c77e39e05`  
		Last Modified: Fri, 24 Apr 2020 21:50:49 GMT  
		Size: 20.9 MB (20873187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb5b078d977aef828e9d0e2a826841117c999252b4bfaed63cdf22b294917073`  
		Last Modified: Fri, 24 Apr 2020 21:53:36 GMT  
		Size: 31.0 MB (30953502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.1-bionic`

```console
$ docker pull swift@sha256:c66c8ea0b3f93f1ab438b0ce70f2065d37b0d1c6052a8299cead7208ddfbf7de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.1-bionic` - linux; amd64

```console
$ docker pull swift@sha256:d3450c154de8ee175c575a6c3a467be52498bb16ff5af30e02850941d2bb869c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **496.0 MB (495970701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5b1eefae081057ddfe64b1d6fbd0cf340adc0ca7a3eb1e44f31596086d3b708`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:07:00 GMT
ADD file:c3e6bb316dfa6b81dd4478aaa310df532883b1c0a14edeec3f63d641980c1789 in / 
# Fri, 24 Apr 2020 01:07:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 01:07:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:07:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:07:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 24 Apr 2020 21:24:10 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:24:11 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 24 Apr 2020 21:24:11 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Fri, 24 Apr 2020 21:31:38 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Fri, 24 Apr 2020 21:31:38 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Fri, 24 Apr 2020 21:31:38 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:31:38 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:32:49 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Fri, 24 Apr 2020 21:32:55 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:23884877105a7ff84a910895cd044061a4561385ff6c36480ee080b76ec0e771`  
		Last Modified: Sat, 04 Apr 2020 12:21:10 GMT  
		Size: 26.7 MB (26689802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc38caa0f5b94141276220daaf428892096e4afd24b05668cd188311e00a635f`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 35.4 KB (35367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2910811b6c4227c2f42aaea9a3dd5f53b1d469f67e2cf7e601f631b119b61ff7`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36505266dcc64eeb1010bd2112e6f73981e1a8246e4f6d4e287763b57f101b0b`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25035e7374ff2fcd78ec35d5d95a9e4587422b205f1c630ae8078085434d5b86`  
		Last Modified: Fri, 24 Apr 2020 21:48:23 GMT  
		Size: 124.1 MB (124077069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d932e2e7c39b531ec37ce74db6da19a5373cf4714a82b93f8e2d0b609721426`  
		Last Modified: Fri, 24 Apr 2020 21:51:53 GMT  
		Size: 345.2 MB (345167455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.1-bionic-slim`

```console
$ docker pull swift@sha256:db74845e123fbfb430d1f309c63848603903e70ce01559a8e6f202bf90c8c25c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.1-bionic-slim` - linux; amd64

```console
$ docker pull swift@sha256:29ff1c9856daa9bda26bacf3a576b710049dc27b28bd1252d7beaebc5f751b15
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78297656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96878a4059b4f6e534cd57e2fbf70549ddbbe7955cd04b1f64be2955c506fb53`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:07:00 GMT
ADD file:c3e6bb316dfa6b81dd4478aaa310df532883b1c0a14edeec3f63d641980c1789 in / 
# Fri, 24 Apr 2020 01:07:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 01:07:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:07:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:07:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 24 Apr 2020 21:28:51 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:28:51 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 24 Apr 2020 21:28:51 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Fri, 24 Apr 2020 21:34:38 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Fri, 24 Apr 2020 21:34:38 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Fri, 24 Apr 2020 21:34:38 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:34:39 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:35:44 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl gnupg && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl gnupg
```

-	Layers:
	-	`sha256:23884877105a7ff84a910895cd044061a4561385ff6c36480ee080b76ec0e771`  
		Last Modified: Sat, 04 Apr 2020 12:21:10 GMT  
		Size: 26.7 MB (26689802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc38caa0f5b94141276220daaf428892096e4afd24b05668cd188311e00a635f`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 35.4 KB (35367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2910811b6c4227c2f42aaea9a3dd5f53b1d469f67e2cf7e601f631b119b61ff7`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36505266dcc64eeb1010bd2112e6f73981e1a8246e4f6d4e287763b57f101b0b`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44ab4793853bd7dece7450fb34472239255b43a04156f4c715f1e92ce766bef`  
		Last Modified: Fri, 24 Apr 2020 21:50:30 GMT  
		Size: 20.5 MB (20488873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:106512f011f225234c6120830f782e50d1dd5cf42ee5b9eca048c3d8f842743e`  
		Last Modified: Fri, 24 Apr 2020 21:53:25 GMT  
		Size: 31.1 MB (31082606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.1-slim`

```console
$ docker pull swift@sha256:db74845e123fbfb430d1f309c63848603903e70ce01559a8e6f202bf90c8c25c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.1-slim` - linux; amd64

```console
$ docker pull swift@sha256:29ff1c9856daa9bda26bacf3a576b710049dc27b28bd1252d7beaebc5f751b15
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78297656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96878a4059b4f6e534cd57e2fbf70549ddbbe7955cd04b1f64be2955c506fb53`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:07:00 GMT
ADD file:c3e6bb316dfa6b81dd4478aaa310df532883b1c0a14edeec3f63d641980c1789 in / 
# Fri, 24 Apr 2020 01:07:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 01:07:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:07:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:07:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 24 Apr 2020 21:28:51 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:28:51 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 24 Apr 2020 21:28:51 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Fri, 24 Apr 2020 21:34:38 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Fri, 24 Apr 2020 21:34:38 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Fri, 24 Apr 2020 21:34:38 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:34:39 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:35:44 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl gnupg && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl gnupg
```

-	Layers:
	-	`sha256:23884877105a7ff84a910895cd044061a4561385ff6c36480ee080b76ec0e771`  
		Last Modified: Sat, 04 Apr 2020 12:21:10 GMT  
		Size: 26.7 MB (26689802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc38caa0f5b94141276220daaf428892096e4afd24b05668cd188311e00a635f`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 35.4 KB (35367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2910811b6c4227c2f42aaea9a3dd5f53b1d469f67e2cf7e601f631b119b61ff7`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36505266dcc64eeb1010bd2112e6f73981e1a8246e4f6d4e287763b57f101b0b`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44ab4793853bd7dece7450fb34472239255b43a04156f4c715f1e92ce766bef`  
		Last Modified: Fri, 24 Apr 2020 21:50:30 GMT  
		Size: 20.5 MB (20488873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:106512f011f225234c6120830f782e50d1dd5cf42ee5b9eca048c3d8f842743e`  
		Last Modified: Fri, 24 Apr 2020 21:53:25 GMT  
		Size: 31.1 MB (31082606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.1-xenial`

```console
$ docker pull swift@sha256:40efc2c42bbceb3c21d77766502c4cd4cf021b0fc0bf89791d080ca42a9c309c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.1-xenial` - linux; amd64

```console
$ docker pull swift@sha256:c135bcd0299ae5582ca94a9d88a83821a30fedbaf7e804ac5813b149ab6597a8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **507.3 MB (507295529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b88d313c9ef80722cec830c650b6f932b9cb3a9caea4a06ae83d74517f33d3b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:25:51 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 24 Apr 2020 21:25:51 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 24 Apr 2020 21:26:57 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl3     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:26:58 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 24 Apr 2020 21:26:58 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Fri, 24 Apr 2020 21:33:08 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Fri, 24 Apr 2020 21:33:08 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Fri, 24 Apr 2020 21:33:08 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:33:08 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:34:19 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Fri, 24 Apr 2020 21:34:21 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6212d70001551edef31dfd8a0d9fa5e80793dbec6c744030626c8cc618939e70`  
		Last Modified: Fri, 24 Apr 2020 21:49:35 GMT  
		Size: 111.6 MB (111572008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aecae2b8a3fe16ad87f837b050ad742caeb047f8ab1bf0101a363ac0d35b719`  
		Last Modified: Fri, 24 Apr 2020 21:53:16 GMT  
		Size: 351.5 MB (351474840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.1-xenial-slim`

```console
$ docker pull swift@sha256:ccf876d6deeeb9a2ae6f552ee36df7393ad017a4010daa43a969bc5885766cc9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.1-xenial-slim` - linux; amd64

```console
$ docker pull swift@sha256:7f1c9516297f005378212b6b5437ccfccb683857cd2d582b7df05f1186eb7d19
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.1 MB (96075370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dea13627d66efc9d5a72704a3b30c5a5fc1f45b119b528b268dfe7b53c33e413`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:25:51 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 24 Apr 2020 21:25:51 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 24 Apr 2020 21:30:19 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl3     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:30:19 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 24 Apr 2020 21:30:19 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Fri, 24 Apr 2020 21:35:54 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Fri, 24 Apr 2020 21:35:54 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Fri, 24 Apr 2020 21:35:55 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:35:55 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:36:59 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89383f79d8ec0934f45345737e157e838789f001791fe3f5ef8b5f8c77e39e05`  
		Last Modified: Fri, 24 Apr 2020 21:50:49 GMT  
		Size: 20.9 MB (20873187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb5b078d977aef828e9d0e2a826841117c999252b4bfaed63cdf22b294917073`  
		Last Modified: Fri, 24 Apr 2020 21:53:36 GMT  
		Size: 31.0 MB (30953502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.2`

```console
$ docker pull swift@sha256:d03a2d3b107c57500be3fd6d717c9a1eb8213b33872fbf6215d3cfc041d5af2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.2` - linux; amd64

```console
$ docker pull swift@sha256:cd6d48c20aa0701fca8c39ee3b4c5bfa84175e62286a70d684bc14f422076613
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **536.2 MB (536214182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d208b5ac2e416f8c91c92b1f804faca633c40a302a0b15f22804735e047b8cb9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:07:00 GMT
ADD file:c3e6bb316dfa6b81dd4478aaa310df532883b1c0a14edeec3f63d641980c1789 in / 
# Fri, 24 Apr 2020 01:07:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 01:07:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:07:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:07:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 24 Apr 2020 21:24:10 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:24:11 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 24 Apr 2020 21:24:11 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Fri, 24 Apr 2020 21:24:11 GMT
ARG SWIFT_BRANCH=swift-5.2.2-release
# Fri, 24 Apr 2020 21:24:11 GMT
ARG SWIFT_VERSION=swift-5.2.2-RELEASE
# Fri, 24 Apr 2020 21:24:11 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:24:12 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.2.2-release SWIFT_VERSION=swift-5.2.2-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:25:30 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Fri, 24 Apr 2020 21:25:33 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:23884877105a7ff84a910895cd044061a4561385ff6c36480ee080b76ec0e771`  
		Last Modified: Sat, 04 Apr 2020 12:21:10 GMT  
		Size: 26.7 MB (26689802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc38caa0f5b94141276220daaf428892096e4afd24b05668cd188311e00a635f`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 35.4 KB (35367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2910811b6c4227c2f42aaea9a3dd5f53b1d469f67e2cf7e601f631b119b61ff7`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36505266dcc64eeb1010bd2112e6f73981e1a8246e4f6d4e287763b57f101b0b`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25035e7374ff2fcd78ec35d5d95a9e4587422b205f1c630ae8078085434d5b86`  
		Last Modified: Fri, 24 Apr 2020 21:48:23 GMT  
		Size: 124.1 MB (124077069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f60046c11fb371a50f0316aca1d59f81d19ed37f4e636e356aaaaf29a51da45`  
		Last Modified: Fri, 24 Apr 2020 21:49:04 GMT  
		Size: 385.4 MB (385410936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.2.3`

**does not exist** (yet?)

## `swift:5.2.3-bionic`

**does not exist** (yet?)

## `swift:5.2.3-bionic-slim`

**does not exist** (yet?)

## `swift:5.2.3-slim`

**does not exist** (yet?)

## `swift:5.2.3-xenial`

**does not exist** (yet?)

## `swift:5.2.3-xenial-slim`

**does not exist** (yet?)

## `swift:5.2-bionic`

```console
$ docker pull swift@sha256:d03a2d3b107c57500be3fd6d717c9a1eb8213b33872fbf6215d3cfc041d5af2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.2-bionic` - linux; amd64

```console
$ docker pull swift@sha256:cd6d48c20aa0701fca8c39ee3b4c5bfa84175e62286a70d684bc14f422076613
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **536.2 MB (536214182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d208b5ac2e416f8c91c92b1f804faca633c40a302a0b15f22804735e047b8cb9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:07:00 GMT
ADD file:c3e6bb316dfa6b81dd4478aaa310df532883b1c0a14edeec3f63d641980c1789 in / 
# Fri, 24 Apr 2020 01:07:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 01:07:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:07:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:07:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 24 Apr 2020 21:24:10 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:24:11 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 24 Apr 2020 21:24:11 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Fri, 24 Apr 2020 21:24:11 GMT
ARG SWIFT_BRANCH=swift-5.2.2-release
# Fri, 24 Apr 2020 21:24:11 GMT
ARG SWIFT_VERSION=swift-5.2.2-RELEASE
# Fri, 24 Apr 2020 21:24:11 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:24:12 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.2.2-release SWIFT_VERSION=swift-5.2.2-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:25:30 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Fri, 24 Apr 2020 21:25:33 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:23884877105a7ff84a910895cd044061a4561385ff6c36480ee080b76ec0e771`  
		Last Modified: Sat, 04 Apr 2020 12:21:10 GMT  
		Size: 26.7 MB (26689802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc38caa0f5b94141276220daaf428892096e4afd24b05668cd188311e00a635f`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 35.4 KB (35367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2910811b6c4227c2f42aaea9a3dd5f53b1d469f67e2cf7e601f631b119b61ff7`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36505266dcc64eeb1010bd2112e6f73981e1a8246e4f6d4e287763b57f101b0b`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25035e7374ff2fcd78ec35d5d95a9e4587422b205f1c630ae8078085434d5b86`  
		Last Modified: Fri, 24 Apr 2020 21:48:23 GMT  
		Size: 124.1 MB (124077069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f60046c11fb371a50f0316aca1d59f81d19ed37f4e636e356aaaaf29a51da45`  
		Last Modified: Fri, 24 Apr 2020 21:49:04 GMT  
		Size: 385.4 MB (385410936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.2-bionic-slim`

```console
$ docker pull swift@sha256:12956856e765e7aeee179c3b7e5b2ab81d2e82536dde02236ff36200ec705351
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.2-bionic-slim` - linux; amd64

```console
$ docker pull swift@sha256:55a996cde6b7f450e092bac6a8c87e4f597fe83ec5572665adc83861e4881071
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79667199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c5515cf84286d6f115c8d1fcdda39dd832f9f1b55359c4e8e026b6d6bc9f612`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:07:00 GMT
ADD file:c3e6bb316dfa6b81dd4478aaa310df532883b1c0a14edeec3f63d641980c1789 in / 
# Fri, 24 Apr 2020 01:07:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 01:07:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:07:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:07:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 24 Apr 2020 21:28:51 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:28:51 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 24 Apr 2020 21:28:51 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Fri, 24 Apr 2020 21:28:51 GMT
ARG SWIFT_BRANCH=swift-5.2.2-release
# Fri, 24 Apr 2020 21:28:51 GMT
ARG SWIFT_VERSION=swift-5.2.2-RELEASE
# Fri, 24 Apr 2020 21:28:51 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:28:52 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.2.2-release SWIFT_VERSION=swift-5.2.2-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:30:02 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl gnupg && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl gnupg
```

-	Layers:
	-	`sha256:23884877105a7ff84a910895cd044061a4561385ff6c36480ee080b76ec0e771`  
		Last Modified: Sat, 04 Apr 2020 12:21:10 GMT  
		Size: 26.7 MB (26689802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc38caa0f5b94141276220daaf428892096e4afd24b05668cd188311e00a635f`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 35.4 KB (35367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2910811b6c4227c2f42aaea9a3dd5f53b1d469f67e2cf7e601f631b119b61ff7`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36505266dcc64eeb1010bd2112e6f73981e1a8246e4f6d4e287763b57f101b0b`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44ab4793853bd7dece7450fb34472239255b43a04156f4c715f1e92ce766bef`  
		Last Modified: Fri, 24 Apr 2020 21:50:30 GMT  
		Size: 20.5 MB (20488873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5662777f9711eee85ef022ab8fe8c1010759a90e59e6a40c5e972a3316903f`  
		Last Modified: Fri, 24 Apr 2020 21:50:33 GMT  
		Size: 32.5 MB (32452149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.2-slim`

```console
$ docker pull swift@sha256:12956856e765e7aeee179c3b7e5b2ab81d2e82536dde02236ff36200ec705351
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.2-slim` - linux; amd64

```console
$ docker pull swift@sha256:55a996cde6b7f450e092bac6a8c87e4f597fe83ec5572665adc83861e4881071
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79667199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c5515cf84286d6f115c8d1fcdda39dd832f9f1b55359c4e8e026b6d6bc9f612`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:07:00 GMT
ADD file:c3e6bb316dfa6b81dd4478aaa310df532883b1c0a14edeec3f63d641980c1789 in / 
# Fri, 24 Apr 2020 01:07:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 01:07:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:07:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:07:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 24 Apr 2020 21:28:51 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:28:51 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 24 Apr 2020 21:28:51 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Fri, 24 Apr 2020 21:28:51 GMT
ARG SWIFT_BRANCH=swift-5.2.2-release
# Fri, 24 Apr 2020 21:28:51 GMT
ARG SWIFT_VERSION=swift-5.2.2-RELEASE
# Fri, 24 Apr 2020 21:28:51 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:28:52 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.2.2-release SWIFT_VERSION=swift-5.2.2-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:30:02 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl gnupg && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl gnupg
```

-	Layers:
	-	`sha256:23884877105a7ff84a910895cd044061a4561385ff6c36480ee080b76ec0e771`  
		Last Modified: Sat, 04 Apr 2020 12:21:10 GMT  
		Size: 26.7 MB (26689802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc38caa0f5b94141276220daaf428892096e4afd24b05668cd188311e00a635f`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 35.4 KB (35367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2910811b6c4227c2f42aaea9a3dd5f53b1d469f67e2cf7e601f631b119b61ff7`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36505266dcc64eeb1010bd2112e6f73981e1a8246e4f6d4e287763b57f101b0b`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44ab4793853bd7dece7450fb34472239255b43a04156f4c715f1e92ce766bef`  
		Last Modified: Fri, 24 Apr 2020 21:50:30 GMT  
		Size: 20.5 MB (20488873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5662777f9711eee85ef022ab8fe8c1010759a90e59e6a40c5e972a3316903f`  
		Last Modified: Fri, 24 Apr 2020 21:50:33 GMT  
		Size: 32.5 MB (32452149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.2-xenial`

```console
$ docker pull swift@sha256:7e025a9a7bc0aaa608413434c4688f53fbaa9e9ac848d19bbae77dab4a55a513
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.2-xenial` - linux; amd64

```console
$ docker pull swift@sha256:e10b0730dc9fdf4e27aae75a16acd3a5c3a63ec477375de57e706e7e4626a9a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **548.7 MB (548733852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:355e296a553eb797aaddb8b86117c93f286b4008033db7b6e050a578ea016a2a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:25:51 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 24 Apr 2020 21:25:51 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 24 Apr 2020 21:26:57 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl3     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:26:58 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 24 Apr 2020 21:26:58 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Fri, 24 Apr 2020 21:26:58 GMT
ARG SWIFT_BRANCH=swift-5.2.2-release
# Fri, 24 Apr 2020 21:26:58 GMT
ARG SWIFT_VERSION=swift-5.2.2-RELEASE
# Fri, 24 Apr 2020 21:26:58 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:26:59 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-5.2.2-release SWIFT_VERSION=swift-5.2.2-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:28:22 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Fri, 24 Apr 2020 21:28:23 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6212d70001551edef31dfd8a0d9fa5e80793dbec6c744030626c8cc618939e70`  
		Last Modified: Fri, 24 Apr 2020 21:49:35 GMT  
		Size: 111.6 MB (111572008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f81fb6d9a810075357412ca1aef2adb7df1276167f1880e9f4a7e92192a2cc2`  
		Last Modified: Fri, 24 Apr 2020 21:50:21 GMT  
		Size: 392.9 MB (392913163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.2-xenial-slim`

```console
$ docker pull swift@sha256:8f4babd555a0d4fc4d020d0dde369f8b02b4d44646168fd00e9d2af0bdf4da1d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.2-xenial-slim` - linux; amd64

```console
$ docker pull swift@sha256:b045fe56024b6a8b9bbc97dfb7e75250156ed613e182168f85a3c7b5fc82a3ca
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.5 MB (97477766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af9633669555d4641ad16dea6b1594b9900b55c06dccdc673f11aeab0acb73af`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:25:51 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 24 Apr 2020 21:25:51 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 24 Apr 2020 21:30:19 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl3     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:30:19 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 24 Apr 2020 21:30:19 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Fri, 24 Apr 2020 21:30:19 GMT
ARG SWIFT_BRANCH=swift-5.2.2-release
# Fri, 24 Apr 2020 21:30:20 GMT
ARG SWIFT_VERSION=swift-5.2.2-RELEASE
# Fri, 24 Apr 2020 21:30:20 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:30:20 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-5.2.2-release SWIFT_VERSION=swift-5.2.2-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:31:30 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89383f79d8ec0934f45345737e157e838789f001791fe3f5ef8b5f8c77e39e05`  
		Last Modified: Fri, 24 Apr 2020 21:50:49 GMT  
		Size: 20.9 MB (20873187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7325eeaf01b42db2a470db58f78bde4ffbaf8bc20372170b981be96e120c4363`  
		Last Modified: Fri, 24 Apr 2020 21:50:51 GMT  
		Size: 32.4 MB (32355898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:bionic`

```console
$ docker pull swift@sha256:d03a2d3b107c57500be3fd6d717c9a1eb8213b33872fbf6215d3cfc041d5af2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:bionic` - linux; amd64

```console
$ docker pull swift@sha256:cd6d48c20aa0701fca8c39ee3b4c5bfa84175e62286a70d684bc14f422076613
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **536.2 MB (536214182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d208b5ac2e416f8c91c92b1f804faca633c40a302a0b15f22804735e047b8cb9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:07:00 GMT
ADD file:c3e6bb316dfa6b81dd4478aaa310df532883b1c0a14edeec3f63d641980c1789 in / 
# Fri, 24 Apr 2020 01:07:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 01:07:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:07:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:07:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 24 Apr 2020 21:24:10 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:24:11 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 24 Apr 2020 21:24:11 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Fri, 24 Apr 2020 21:24:11 GMT
ARG SWIFT_BRANCH=swift-5.2.2-release
# Fri, 24 Apr 2020 21:24:11 GMT
ARG SWIFT_VERSION=swift-5.2.2-RELEASE
# Fri, 24 Apr 2020 21:24:11 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:24:12 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.2.2-release SWIFT_VERSION=swift-5.2.2-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:25:30 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Fri, 24 Apr 2020 21:25:33 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:23884877105a7ff84a910895cd044061a4561385ff6c36480ee080b76ec0e771`  
		Last Modified: Sat, 04 Apr 2020 12:21:10 GMT  
		Size: 26.7 MB (26689802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc38caa0f5b94141276220daaf428892096e4afd24b05668cd188311e00a635f`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 35.4 KB (35367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2910811b6c4227c2f42aaea9a3dd5f53b1d469f67e2cf7e601f631b119b61ff7`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36505266dcc64eeb1010bd2112e6f73981e1a8246e4f6d4e287763b57f101b0b`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25035e7374ff2fcd78ec35d5d95a9e4587422b205f1c630ae8078085434d5b86`  
		Last Modified: Fri, 24 Apr 2020 21:48:23 GMT  
		Size: 124.1 MB (124077069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f60046c11fb371a50f0316aca1d59f81d19ed37f4e636e356aaaaf29a51da45`  
		Last Modified: Fri, 24 Apr 2020 21:49:04 GMT  
		Size: 385.4 MB (385410936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:bionic-slim`

```console
$ docker pull swift@sha256:12956856e765e7aeee179c3b7e5b2ab81d2e82536dde02236ff36200ec705351
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:bionic-slim` - linux; amd64

```console
$ docker pull swift@sha256:55a996cde6b7f450e092bac6a8c87e4f597fe83ec5572665adc83861e4881071
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79667199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c5515cf84286d6f115c8d1fcdda39dd832f9f1b55359c4e8e026b6d6bc9f612`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:07:00 GMT
ADD file:c3e6bb316dfa6b81dd4478aaa310df532883b1c0a14edeec3f63d641980c1789 in / 
# Fri, 24 Apr 2020 01:07:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 01:07:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:07:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:07:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 24 Apr 2020 21:28:51 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:28:51 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 24 Apr 2020 21:28:51 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Fri, 24 Apr 2020 21:28:51 GMT
ARG SWIFT_BRANCH=swift-5.2.2-release
# Fri, 24 Apr 2020 21:28:51 GMT
ARG SWIFT_VERSION=swift-5.2.2-RELEASE
# Fri, 24 Apr 2020 21:28:51 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:28:52 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.2.2-release SWIFT_VERSION=swift-5.2.2-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:30:02 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl gnupg && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl gnupg
```

-	Layers:
	-	`sha256:23884877105a7ff84a910895cd044061a4561385ff6c36480ee080b76ec0e771`  
		Last Modified: Sat, 04 Apr 2020 12:21:10 GMT  
		Size: 26.7 MB (26689802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc38caa0f5b94141276220daaf428892096e4afd24b05668cd188311e00a635f`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 35.4 KB (35367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2910811b6c4227c2f42aaea9a3dd5f53b1d469f67e2cf7e601f631b119b61ff7`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36505266dcc64eeb1010bd2112e6f73981e1a8246e4f6d4e287763b57f101b0b`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44ab4793853bd7dece7450fb34472239255b43a04156f4c715f1e92ce766bef`  
		Last Modified: Fri, 24 Apr 2020 21:50:30 GMT  
		Size: 20.5 MB (20488873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5662777f9711eee85ef022ab8fe8c1010759a90e59e6a40c5e972a3316903f`  
		Last Modified: Fri, 24 Apr 2020 21:50:33 GMT  
		Size: 32.5 MB (32452149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:latest`

```console
$ docker pull swift@sha256:d03a2d3b107c57500be3fd6d717c9a1eb8213b33872fbf6215d3cfc041d5af2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:latest` - linux; amd64

```console
$ docker pull swift@sha256:cd6d48c20aa0701fca8c39ee3b4c5bfa84175e62286a70d684bc14f422076613
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **536.2 MB (536214182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d208b5ac2e416f8c91c92b1f804faca633c40a302a0b15f22804735e047b8cb9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:07:00 GMT
ADD file:c3e6bb316dfa6b81dd4478aaa310df532883b1c0a14edeec3f63d641980c1789 in / 
# Fri, 24 Apr 2020 01:07:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 01:07:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:07:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:07:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 24 Apr 2020 21:24:10 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:24:11 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 24 Apr 2020 21:24:11 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Fri, 24 Apr 2020 21:24:11 GMT
ARG SWIFT_BRANCH=swift-5.2.2-release
# Fri, 24 Apr 2020 21:24:11 GMT
ARG SWIFT_VERSION=swift-5.2.2-RELEASE
# Fri, 24 Apr 2020 21:24:11 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:24:12 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.2.2-release SWIFT_VERSION=swift-5.2.2-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:25:30 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Fri, 24 Apr 2020 21:25:33 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:23884877105a7ff84a910895cd044061a4561385ff6c36480ee080b76ec0e771`  
		Last Modified: Sat, 04 Apr 2020 12:21:10 GMT  
		Size: 26.7 MB (26689802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc38caa0f5b94141276220daaf428892096e4afd24b05668cd188311e00a635f`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 35.4 KB (35367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2910811b6c4227c2f42aaea9a3dd5f53b1d469f67e2cf7e601f631b119b61ff7`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36505266dcc64eeb1010bd2112e6f73981e1a8246e4f6d4e287763b57f101b0b`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25035e7374ff2fcd78ec35d5d95a9e4587422b205f1c630ae8078085434d5b86`  
		Last Modified: Fri, 24 Apr 2020 21:48:23 GMT  
		Size: 124.1 MB (124077069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f60046c11fb371a50f0316aca1d59f81d19ed37f4e636e356aaaaf29a51da45`  
		Last Modified: Fri, 24 Apr 2020 21:49:04 GMT  
		Size: 385.4 MB (385410936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:slim`

```console
$ docker pull swift@sha256:12956856e765e7aeee179c3b7e5b2ab81d2e82536dde02236ff36200ec705351
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:slim` - linux; amd64

```console
$ docker pull swift@sha256:55a996cde6b7f450e092bac6a8c87e4f597fe83ec5572665adc83861e4881071
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79667199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c5515cf84286d6f115c8d1fcdda39dd832f9f1b55359c4e8e026b6d6bc9f612`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:07:00 GMT
ADD file:c3e6bb316dfa6b81dd4478aaa310df532883b1c0a14edeec3f63d641980c1789 in / 
# Fri, 24 Apr 2020 01:07:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 01:07:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:07:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:07:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 24 Apr 2020 21:23:35 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 24 Apr 2020 21:28:51 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:28:51 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 24 Apr 2020 21:28:51 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Fri, 24 Apr 2020 21:28:51 GMT
ARG SWIFT_BRANCH=swift-5.2.2-release
# Fri, 24 Apr 2020 21:28:51 GMT
ARG SWIFT_VERSION=swift-5.2.2-RELEASE
# Fri, 24 Apr 2020 21:28:51 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:28:52 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.2.2-release SWIFT_VERSION=swift-5.2.2-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:30:02 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl gnupg && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl gnupg
```

-	Layers:
	-	`sha256:23884877105a7ff84a910895cd044061a4561385ff6c36480ee080b76ec0e771`  
		Last Modified: Sat, 04 Apr 2020 12:21:10 GMT  
		Size: 26.7 MB (26689802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc38caa0f5b94141276220daaf428892096e4afd24b05668cd188311e00a635f`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 35.4 KB (35367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2910811b6c4227c2f42aaea9a3dd5f53b1d469f67e2cf7e601f631b119b61ff7`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36505266dcc64eeb1010bd2112e6f73981e1a8246e4f6d4e287763b57f101b0b`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44ab4793853bd7dece7450fb34472239255b43a04156f4c715f1e92ce766bef`  
		Last Modified: Fri, 24 Apr 2020 21:50:30 GMT  
		Size: 20.5 MB (20488873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5662777f9711eee85ef022ab8fe8c1010759a90e59e6a40c5e972a3316903f`  
		Last Modified: Fri, 24 Apr 2020 21:50:33 GMT  
		Size: 32.5 MB (32452149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:xenial`

```console
$ docker pull swift@sha256:7e025a9a7bc0aaa608413434c4688f53fbaa9e9ac848d19bbae77dab4a55a513
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:xenial` - linux; amd64

```console
$ docker pull swift@sha256:e10b0730dc9fdf4e27aae75a16acd3a5c3a63ec477375de57e706e7e4626a9a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **548.7 MB (548733852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:355e296a553eb797aaddb8b86117c93f286b4008033db7b6e050a578ea016a2a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:25:51 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 24 Apr 2020 21:25:51 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 24 Apr 2020 21:26:57 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl3     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:26:58 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 24 Apr 2020 21:26:58 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Fri, 24 Apr 2020 21:26:58 GMT
ARG SWIFT_BRANCH=swift-5.2.2-release
# Fri, 24 Apr 2020 21:26:58 GMT
ARG SWIFT_VERSION=swift-5.2.2-RELEASE
# Fri, 24 Apr 2020 21:26:58 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:26:59 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-5.2.2-release SWIFT_VERSION=swift-5.2.2-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:28:22 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Fri, 24 Apr 2020 21:28:23 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6212d70001551edef31dfd8a0d9fa5e80793dbec6c744030626c8cc618939e70`  
		Last Modified: Fri, 24 Apr 2020 21:49:35 GMT  
		Size: 111.6 MB (111572008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f81fb6d9a810075357412ca1aef2adb7df1276167f1880e9f4a7e92192a2cc2`  
		Last Modified: Fri, 24 Apr 2020 21:50:21 GMT  
		Size: 392.9 MB (392913163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:xenial-slim`

```console
$ docker pull swift@sha256:8f4babd555a0d4fc4d020d0dde369f8b02b4d44646168fd00e9d2af0bdf4da1d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:xenial-slim` - linux; amd64

```console
$ docker pull swift@sha256:b045fe56024b6a8b9bbc97dfb7e75250156ed613e182168f85a3c7b5fc82a3ca
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.5 MB (97477766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af9633669555d4641ad16dea6b1594b9900b55c06dccdc673f11aeab0acb73af`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:25:51 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 24 Apr 2020 21:25:51 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 24 Apr 2020 21:30:19 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl3     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:30:19 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 24 Apr 2020 21:30:19 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Fri, 24 Apr 2020 21:30:19 GMT
ARG SWIFT_BRANCH=swift-5.2.2-release
# Fri, 24 Apr 2020 21:30:20 GMT
ARG SWIFT_VERSION=swift-5.2.2-RELEASE
# Fri, 24 Apr 2020 21:30:20 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:30:20 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-5.2.2-release SWIFT_VERSION=swift-5.2.2-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 24 Apr 2020 21:31:30 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89383f79d8ec0934f45345737e157e838789f001791fe3f5ef8b5f8c77e39e05`  
		Last Modified: Fri, 24 Apr 2020 21:50:49 GMT  
		Size: 20.9 MB (20873187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7325eeaf01b42db2a470db58f78bde4ffbaf8bc20372170b981be96e120c4363`  
		Last Modified: Fri, 24 Apr 2020 21:50:51 GMT  
		Size: 32.4 MB (32355898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
