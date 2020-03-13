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
-	[`swift:bionic`](#swiftbionic)
-	[`swift:bionic-slim`](#swiftbionic-slim)
-	[`swift:latest`](#swiftlatest)
-	[`swift:slim`](#swiftslim)
-	[`swift:xenial`](#swiftxenial)
-	[`swift:xenial-slim`](#swiftxenial-slim)

## `swift:4`

```console
$ docker pull swift@sha256:e8d627ea7f09f8a2ef701651e667655ffe54436e220fb9fc2cad6844f9e7d9de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:4` - linux; amd64

```console
$ docker pull swift@sha256:b5006de083f424be35d666e297ce03bd70e8dc61a951af0dd54e671f48b5301b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **496.8 MB (496826857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5b1adfe95d052ba4483f01146ba78e565c36404ba6f067f3f220a78ae83411b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:04:42 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Sat, 22 Feb 2020 00:04:43 GMT
LABEL Description=Docker Container for the Swift programming language
# Sat, 22 Feb 2020 00:16:14 GMT
RUN apt-get -q update &&     apt-get -q install -y     make     libc6-dev     clang-3.8     curl     libedit-dev     libpython2.7     libicu-dev     libssl-dev     libxml2     tzdata     git     libcurl4-openssl-dev     pkg-config     && update-alternatives --quiet --install /usr/bin/clang clang /usr/bin/clang-3.8 100     && update-alternatives --quiet --install /usr/bin/clang++ clang++ /usr/bin/clang++-3.8 100     && rm -r /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:16:14 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Sat, 22 Feb 2020 00:16:14 GMT
ARG SWIFT_BRANCH=swift-4.2.4-release
# Sat, 22 Feb 2020 00:16:15 GMT
ARG SWIFT_VERSION=swift-4.2.4-RELEASE
# Sat, 22 Feb 2020 00:16:15 GMT
ENV SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-4.2.4-release SWIFT_VERSION=swift-4.2.4-RELEASE
# Sat, 22 Feb 2020 00:16:55 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           8513444E2DA36B7C1659AF4D7638F1FB2B2B08C4           A3BAFD3556A59079C06894BD63BC1CFE91D306C6           5E4DF843FB065D7F7E24FBA2EF5430F071E1B235         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
# Sat, 22 Feb 2020 00:16:56 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56997e437e35ae4071db7c2814414f4852759c54671e3e5e2c17b5a945a2283`  
		Last Modified: Sat, 22 Feb 2020 00:25:24 GMT  
		Size: 224.5 MB (224467416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a1b74fedecdb195d05f9f9bc0b412ce7c292fde64224dcb1e0d24185e8d973`  
		Last Modified: Sat, 22 Feb 2020 00:25:24 GMT  
		Size: 228.2 MB (228166170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:4.0`

```console
$ docker pull swift@sha256:ce29178412e867d156103e2e61f36128cc5047ffab84ab6349557f86bfe16990
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:4.0` - linux; amd64

```console
$ docker pull swift@sha256:c8e92d1d6bcefb303d506b2d8ebdea941d216bb83af18cbe4de513e68456f35e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **439.3 MB (439298334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4023da907c97ff682a348e248650aa30dbf58427acbe1b16caf29022c5e7414c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:17:07 GMT
LABEL maintainer=Haris Amin <aminharis7@gmail.com>
# Sat, 22 Feb 2020 00:17:07 GMT
LABEL Description=Docker Container for the Apple's Swift programming language
# Sat, 22 Feb 2020 00:17:50 GMT
RUN apt-get -q update &&     apt-get -q install -y     make     libc6-dev     clang-3.8     curl     libedit-dev     libpython2.7     libicu-dev     libssl-dev     libxml2     tzdata     git     libcurl4-openssl-dev     pkg-config     && update-alternatives --quiet --install /usr/bin/clang clang /usr/bin/clang-3.8 100     && update-alternatives --quiet --install /usr/bin/clang++ clang++ /usr/bin/clang++-3.8 100     && rm -r /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:17:51 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Sat, 22 Feb 2020 00:18:36 GMT
ARG SWIFT_BRANCH=swift-4.0.3-release
# Sat, 22 Feb 2020 00:18:36 GMT
ARG SWIFT_VERSION=swift-4.0.3-RELEASE
# Sat, 22 Feb 2020 00:18:36 GMT
ENV SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-4.0.3-release SWIFT_VERSION=swift-4.0.3-RELEASE
# Sat, 22 Feb 2020 00:19:06 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           8513444E2DA36B7C1659AF4D7638F1FB2B2B08C4           A3BAFD3556A59079C06894BD63BC1CFE91D306C6           5E4DF843FB065D7F7E24FBA2EF5430F071E1B235         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
# Sat, 22 Feb 2020 00:19:07 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2259f18daacb80cc6e3a74507b8f322a52cdb3b000eb344b11baae8cbb6ace9`  
		Last Modified: Sat, 22 Feb 2020 00:26:16 GMT  
		Size: 224.5 MB (224467143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20761b42580d865f138040de1d119338b8537bf98645135538b06b82ee1b9905`  
		Last Modified: Sat, 22 Feb 2020 00:26:51 GMT  
		Size: 170.6 MB (170637920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:4.0.3`

```console
$ docker pull swift@sha256:ce29178412e867d156103e2e61f36128cc5047ffab84ab6349557f86bfe16990
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:4.0.3` - linux; amd64

```console
$ docker pull swift@sha256:c8e92d1d6bcefb303d506b2d8ebdea941d216bb83af18cbe4de513e68456f35e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **439.3 MB (439298334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4023da907c97ff682a348e248650aa30dbf58427acbe1b16caf29022c5e7414c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:17:07 GMT
LABEL maintainer=Haris Amin <aminharis7@gmail.com>
# Sat, 22 Feb 2020 00:17:07 GMT
LABEL Description=Docker Container for the Apple's Swift programming language
# Sat, 22 Feb 2020 00:17:50 GMT
RUN apt-get -q update &&     apt-get -q install -y     make     libc6-dev     clang-3.8     curl     libedit-dev     libpython2.7     libicu-dev     libssl-dev     libxml2     tzdata     git     libcurl4-openssl-dev     pkg-config     && update-alternatives --quiet --install /usr/bin/clang clang /usr/bin/clang-3.8 100     && update-alternatives --quiet --install /usr/bin/clang++ clang++ /usr/bin/clang++-3.8 100     && rm -r /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:17:51 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Sat, 22 Feb 2020 00:18:36 GMT
ARG SWIFT_BRANCH=swift-4.0.3-release
# Sat, 22 Feb 2020 00:18:36 GMT
ARG SWIFT_VERSION=swift-4.0.3-RELEASE
# Sat, 22 Feb 2020 00:18:36 GMT
ENV SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-4.0.3-release SWIFT_VERSION=swift-4.0.3-RELEASE
# Sat, 22 Feb 2020 00:19:06 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           8513444E2DA36B7C1659AF4D7638F1FB2B2B08C4           A3BAFD3556A59079C06894BD63BC1CFE91D306C6           5E4DF843FB065D7F7E24FBA2EF5430F071E1B235         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
# Sat, 22 Feb 2020 00:19:07 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2259f18daacb80cc6e3a74507b8f322a52cdb3b000eb344b11baae8cbb6ace9`  
		Last Modified: Sat, 22 Feb 2020 00:26:16 GMT  
		Size: 224.5 MB (224467143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20761b42580d865f138040de1d119338b8537bf98645135538b06b82ee1b9905`  
		Last Modified: Sat, 22 Feb 2020 00:26:51 GMT  
		Size: 170.6 MB (170637920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:4.1`

```console
$ docker pull swift@sha256:18407204a6b37921da9811c901ff3a2ca2ee6dc84e4a093ebde9a2c6186c730e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:4.1` - linux; amd64

```console
$ docker pull swift@sha256:c9466eedc9c5bf26cc5e66d0331158443263690f70928b7a0d7b5dcfa232679e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **451.9 MB (451892691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a84ae5529673ef772cdf5d97b731a3c3e991ce6e5f8574d5cf28fbe919141782`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:17:07 GMT
LABEL maintainer=Haris Amin <aminharis7@gmail.com>
# Sat, 22 Feb 2020 00:17:07 GMT
LABEL Description=Docker Container for the Apple's Swift programming language
# Sat, 22 Feb 2020 00:17:50 GMT
RUN apt-get -q update &&     apt-get -q install -y     make     libc6-dev     clang-3.8     curl     libedit-dev     libpython2.7     libicu-dev     libssl-dev     libxml2     tzdata     git     libcurl4-openssl-dev     pkg-config     && update-alternatives --quiet --install /usr/bin/clang clang /usr/bin/clang-3.8 100     && update-alternatives --quiet --install /usr/bin/clang++ clang++ /usr/bin/clang++-3.8 100     && rm -r /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:17:51 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Sat, 22 Feb 2020 00:17:51 GMT
ARG SWIFT_BRANCH=swift-4.1.3-release
# Sat, 22 Feb 2020 00:17:51 GMT
ARG SWIFT_VERSION=swift-4.1.3-RELEASE
# Sat, 22 Feb 2020 00:17:51 GMT
ENV SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-4.1.3-release SWIFT_VERSION=swift-4.1.3-RELEASE
# Sat, 22 Feb 2020 00:18:25 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           8513444E2DA36B7C1659AF4D7638F1FB2B2B08C4           A3BAFD3556A59079C06894BD63BC1CFE91D306C6           5E4DF843FB065D7F7E24FBA2EF5430F071E1B235         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
# Sat, 22 Feb 2020 00:18:26 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2259f18daacb80cc6e3a74507b8f322a52cdb3b000eb344b11baae8cbb6ace9`  
		Last Modified: Sat, 22 Feb 2020 00:26:16 GMT  
		Size: 224.5 MB (224467143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df62a6e50245eb3ffb01b37e9645043d6dff70456a802432cee13313a39c5fc`  
		Last Modified: Sat, 22 Feb 2020 00:26:08 GMT  
		Size: 183.2 MB (183232277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:4.1.3`

```console
$ docker pull swift@sha256:18407204a6b37921da9811c901ff3a2ca2ee6dc84e4a093ebde9a2c6186c730e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:4.1.3` - linux; amd64

```console
$ docker pull swift@sha256:c9466eedc9c5bf26cc5e66d0331158443263690f70928b7a0d7b5dcfa232679e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **451.9 MB (451892691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a84ae5529673ef772cdf5d97b731a3c3e991ce6e5f8574d5cf28fbe919141782`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:17:07 GMT
LABEL maintainer=Haris Amin <aminharis7@gmail.com>
# Sat, 22 Feb 2020 00:17:07 GMT
LABEL Description=Docker Container for the Apple's Swift programming language
# Sat, 22 Feb 2020 00:17:50 GMT
RUN apt-get -q update &&     apt-get -q install -y     make     libc6-dev     clang-3.8     curl     libedit-dev     libpython2.7     libicu-dev     libssl-dev     libxml2     tzdata     git     libcurl4-openssl-dev     pkg-config     && update-alternatives --quiet --install /usr/bin/clang clang /usr/bin/clang-3.8 100     && update-alternatives --quiet --install /usr/bin/clang++ clang++ /usr/bin/clang++-3.8 100     && rm -r /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:17:51 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Sat, 22 Feb 2020 00:17:51 GMT
ARG SWIFT_BRANCH=swift-4.1.3-release
# Sat, 22 Feb 2020 00:17:51 GMT
ARG SWIFT_VERSION=swift-4.1.3-RELEASE
# Sat, 22 Feb 2020 00:17:51 GMT
ENV SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-4.1.3-release SWIFT_VERSION=swift-4.1.3-RELEASE
# Sat, 22 Feb 2020 00:18:25 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           8513444E2DA36B7C1659AF4D7638F1FB2B2B08C4           A3BAFD3556A59079C06894BD63BC1CFE91D306C6           5E4DF843FB065D7F7E24FBA2EF5430F071E1B235         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
# Sat, 22 Feb 2020 00:18:26 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2259f18daacb80cc6e3a74507b8f322a52cdb3b000eb344b11baae8cbb6ace9`  
		Last Modified: Sat, 22 Feb 2020 00:26:16 GMT  
		Size: 224.5 MB (224467143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df62a6e50245eb3ffb01b37e9645043d6dff70456a802432cee13313a39c5fc`  
		Last Modified: Sat, 22 Feb 2020 00:26:08 GMT  
		Size: 183.2 MB (183232277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:4.2`

```console
$ docker pull swift@sha256:e8d627ea7f09f8a2ef701651e667655ffe54436e220fb9fc2cad6844f9e7d9de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:4.2` - linux; amd64

```console
$ docker pull swift@sha256:b5006de083f424be35d666e297ce03bd70e8dc61a951af0dd54e671f48b5301b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **496.8 MB (496826857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5b1adfe95d052ba4483f01146ba78e565c36404ba6f067f3f220a78ae83411b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:04:42 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Sat, 22 Feb 2020 00:04:43 GMT
LABEL Description=Docker Container for the Swift programming language
# Sat, 22 Feb 2020 00:16:14 GMT
RUN apt-get -q update &&     apt-get -q install -y     make     libc6-dev     clang-3.8     curl     libedit-dev     libpython2.7     libicu-dev     libssl-dev     libxml2     tzdata     git     libcurl4-openssl-dev     pkg-config     && update-alternatives --quiet --install /usr/bin/clang clang /usr/bin/clang-3.8 100     && update-alternatives --quiet --install /usr/bin/clang++ clang++ /usr/bin/clang++-3.8 100     && rm -r /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:16:14 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Sat, 22 Feb 2020 00:16:14 GMT
ARG SWIFT_BRANCH=swift-4.2.4-release
# Sat, 22 Feb 2020 00:16:15 GMT
ARG SWIFT_VERSION=swift-4.2.4-RELEASE
# Sat, 22 Feb 2020 00:16:15 GMT
ENV SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-4.2.4-release SWIFT_VERSION=swift-4.2.4-RELEASE
# Sat, 22 Feb 2020 00:16:55 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           8513444E2DA36B7C1659AF4D7638F1FB2B2B08C4           A3BAFD3556A59079C06894BD63BC1CFE91D306C6           5E4DF843FB065D7F7E24FBA2EF5430F071E1B235         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
# Sat, 22 Feb 2020 00:16:56 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56997e437e35ae4071db7c2814414f4852759c54671e3e5e2c17b5a945a2283`  
		Last Modified: Sat, 22 Feb 2020 00:25:24 GMT  
		Size: 224.5 MB (224467416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a1b74fedecdb195d05f9f9bc0b412ce7c292fde64224dcb1e0d24185e8d973`  
		Last Modified: Sat, 22 Feb 2020 00:25:24 GMT  
		Size: 228.2 MB (228166170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:4.2.4`

```console
$ docker pull swift@sha256:e8d627ea7f09f8a2ef701651e667655ffe54436e220fb9fc2cad6844f9e7d9de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:4.2.4` - linux; amd64

```console
$ docker pull swift@sha256:b5006de083f424be35d666e297ce03bd70e8dc61a951af0dd54e671f48b5301b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **496.8 MB (496826857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5b1adfe95d052ba4483f01146ba78e565c36404ba6f067f3f220a78ae83411b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:04:42 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Sat, 22 Feb 2020 00:04:43 GMT
LABEL Description=Docker Container for the Swift programming language
# Sat, 22 Feb 2020 00:16:14 GMT
RUN apt-get -q update &&     apt-get -q install -y     make     libc6-dev     clang-3.8     curl     libedit-dev     libpython2.7     libicu-dev     libssl-dev     libxml2     tzdata     git     libcurl4-openssl-dev     pkg-config     && update-alternatives --quiet --install /usr/bin/clang clang /usr/bin/clang-3.8 100     && update-alternatives --quiet --install /usr/bin/clang++ clang++ /usr/bin/clang++-3.8 100     && rm -r /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:16:14 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Sat, 22 Feb 2020 00:16:14 GMT
ARG SWIFT_BRANCH=swift-4.2.4-release
# Sat, 22 Feb 2020 00:16:15 GMT
ARG SWIFT_VERSION=swift-4.2.4-RELEASE
# Sat, 22 Feb 2020 00:16:15 GMT
ENV SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-4.2.4-release SWIFT_VERSION=swift-4.2.4-RELEASE
# Sat, 22 Feb 2020 00:16:55 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           8513444E2DA36B7C1659AF4D7638F1FB2B2B08C4           A3BAFD3556A59079C06894BD63BC1CFE91D306C6           5E4DF843FB065D7F7E24FBA2EF5430F071E1B235         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
# Sat, 22 Feb 2020 00:16:56 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56997e437e35ae4071db7c2814414f4852759c54671e3e5e2c17b5a945a2283`  
		Last Modified: Sat, 22 Feb 2020 00:25:24 GMT  
		Size: 224.5 MB (224467416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a1b74fedecdb195d05f9f9bc0b412ce7c292fde64224dcb1e0d24185e8d973`  
		Last Modified: Sat, 22 Feb 2020 00:25:24 GMT  
		Size: 228.2 MB (228166170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.0`

```console
$ docker pull swift@sha256:6d8b85b1592e97300ce4081ecfd4474ce4a9f6894a83d02ea9ba35d988f04f95
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.0` - linux; amd64

```console
$ docker pull swift@sha256:697710b03142b8861805b2ae5118589da95cac354d44cba53005f30e095e5b25
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.0 MB (462992218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14aec6b7b3af2bbc3637e113dd87f5e26fdb6f4386b52198b48c8ba78f2704f4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL Description=Docker Container for the Swift programming language
# Sat, 22 Feb 2020 00:09:53 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libbsd0     libcurl4     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:09:54 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Sat, 22 Feb 2020 00:09:54 GMT
ARG SWIFT_BRANCH=swift-5.0.3-release
# Sat, 22 Feb 2020 00:09:54 GMT
ARG SWIFT_VERSION=swift-5.0.3-RELEASE
# Sat, 22 Feb 2020 00:09:54 GMT
ENV SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.0.3-release SWIFT_VERSION=swift-5.0.3-RELEASE
# Sat, 22 Feb 2020 00:10:52 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && apt-get update     && apt-get install -y curl     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && apt-get purge -y curl     && apt-get -y autoremove     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           A62AE125BBBFBB96A6E042EC925CC1CCED3D1561         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
# Sat, 22 Feb 2020 00:10:58 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1154b15f1870c37c0f357d3b1a6acd21c02d8f3c0d0c3d828132e43ea3cc44cf`  
		Last Modified: Sat, 22 Feb 2020 00:22:40 GMT  
		Size: 117.0 MB (116965374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007c485330fb667e606d6c6382c6b3fd0f17510af7853f7e378c6c42ed22f9ff`  
		Last Modified: Sat, 22 Feb 2020 00:23:09 GMT  
		Size: 319.3 MB (319298368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.0.3`

```console
$ docker pull swift@sha256:6d8b85b1592e97300ce4081ecfd4474ce4a9f6894a83d02ea9ba35d988f04f95
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.0.3` - linux; amd64

```console
$ docker pull swift@sha256:697710b03142b8861805b2ae5118589da95cac354d44cba53005f30e095e5b25
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.0 MB (462992218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14aec6b7b3af2bbc3637e113dd87f5e26fdb6f4386b52198b48c8ba78f2704f4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL Description=Docker Container for the Swift programming language
# Sat, 22 Feb 2020 00:09:53 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libbsd0     libcurl4     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:09:54 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Sat, 22 Feb 2020 00:09:54 GMT
ARG SWIFT_BRANCH=swift-5.0.3-release
# Sat, 22 Feb 2020 00:09:54 GMT
ARG SWIFT_VERSION=swift-5.0.3-RELEASE
# Sat, 22 Feb 2020 00:09:54 GMT
ENV SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.0.3-release SWIFT_VERSION=swift-5.0.3-RELEASE
# Sat, 22 Feb 2020 00:10:52 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && apt-get update     && apt-get install -y curl     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && apt-get purge -y curl     && apt-get -y autoremove     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           A62AE125BBBFBB96A6E042EC925CC1CCED3D1561         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
# Sat, 22 Feb 2020 00:10:58 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1154b15f1870c37c0f357d3b1a6acd21c02d8f3c0d0c3d828132e43ea3cc44cf`  
		Last Modified: Sat, 22 Feb 2020 00:22:40 GMT  
		Size: 117.0 MB (116965374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007c485330fb667e606d6c6382c6b3fd0f17510af7853f7e378c6c42ed22f9ff`  
		Last Modified: Sat, 22 Feb 2020 00:23:09 GMT  
		Size: 319.3 MB (319298368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.0.3-bionic`

```console
$ docker pull swift@sha256:6d8b85b1592e97300ce4081ecfd4474ce4a9f6894a83d02ea9ba35d988f04f95
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.0.3-bionic` - linux; amd64

```console
$ docker pull swift@sha256:697710b03142b8861805b2ae5118589da95cac354d44cba53005f30e095e5b25
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.0 MB (462992218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14aec6b7b3af2bbc3637e113dd87f5e26fdb6f4386b52198b48c8ba78f2704f4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL Description=Docker Container for the Swift programming language
# Sat, 22 Feb 2020 00:09:53 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libbsd0     libcurl4     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:09:54 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Sat, 22 Feb 2020 00:09:54 GMT
ARG SWIFT_BRANCH=swift-5.0.3-release
# Sat, 22 Feb 2020 00:09:54 GMT
ARG SWIFT_VERSION=swift-5.0.3-RELEASE
# Sat, 22 Feb 2020 00:09:54 GMT
ENV SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.0.3-release SWIFT_VERSION=swift-5.0.3-RELEASE
# Sat, 22 Feb 2020 00:10:52 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && apt-get update     && apt-get install -y curl     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && apt-get purge -y curl     && apt-get -y autoremove     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           A62AE125BBBFBB96A6E042EC925CC1CCED3D1561         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
# Sat, 22 Feb 2020 00:10:58 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1154b15f1870c37c0f357d3b1a6acd21c02d8f3c0d0c3d828132e43ea3cc44cf`  
		Last Modified: Sat, 22 Feb 2020 00:22:40 GMT  
		Size: 117.0 MB (116965374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007c485330fb667e606d6c6382c6b3fd0f17510af7853f7e378c6c42ed22f9ff`  
		Last Modified: Sat, 22 Feb 2020 00:23:09 GMT  
		Size: 319.3 MB (319298368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.0.3-bionic-slim`

```console
$ docker pull swift@sha256:2d9ce495c9043696d6ff1e284686f71a5fa0b89156456ed3530acd959b674945
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.0.3-bionic-slim` - linux; amd64

```console
$ docker pull swift@sha256:f2890b98664d7abea2e819df17322a7e0c8817ee83c1aed11ce9d3a257728795
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75162101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faf14f6fc2e147276289d4e5c0842a2859c0f4d0edc97341a84878958deaf8ae`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL Description=Docker Container for the Swift programming language
# Sat, 22 Feb 2020 00:13:05 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libbsd0     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:13:06 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Sat, 22 Feb 2020 00:13:06 GMT
ARG SWIFT_BRANCH=swift-5.0.3-release
# Sat, 22 Feb 2020 00:13:06 GMT
ARG SWIFT_VERSION=swift-5.0.3-RELEASE
# Sat, 22 Feb 2020 00:13:06 GMT
ENV SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.0.3-release SWIFT_VERSION=swift-5.0.3-RELEASE
# Sat, 22 Feb 2020 00:13:59 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && apt-get update     && apt-get install -y curl gpg     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           A62AE125BBBFBB96A6E042EC925CC1CCED3D1561         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && apt-get purge -y curl gpg     && apt-get -y autoremove     && rm -r /var/lib/apt/lists/*     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fe32ef0cb4aaeaba41c7cd5c3be7ac9b2dfbd16b0e6bdc1a00856d833d775d`  
		Last Modified: Sat, 22 Feb 2020 00:24:21 GMT  
		Size: 20.5 MB (20534267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dca9598437d829a748b15126e67b58c5c56272d24acf700515b70f58a14ac887`  
		Last Modified: Sat, 22 Feb 2020 00:24:23 GMT  
		Size: 27.9 MB (27899358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.0.3-slim`

```console
$ docker pull swift@sha256:2d9ce495c9043696d6ff1e284686f71a5fa0b89156456ed3530acd959b674945
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.0.3-slim` - linux; amd64

```console
$ docker pull swift@sha256:f2890b98664d7abea2e819df17322a7e0c8817ee83c1aed11ce9d3a257728795
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75162101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faf14f6fc2e147276289d4e5c0842a2859c0f4d0edc97341a84878958deaf8ae`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL Description=Docker Container for the Swift programming language
# Sat, 22 Feb 2020 00:13:05 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libbsd0     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:13:06 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Sat, 22 Feb 2020 00:13:06 GMT
ARG SWIFT_BRANCH=swift-5.0.3-release
# Sat, 22 Feb 2020 00:13:06 GMT
ARG SWIFT_VERSION=swift-5.0.3-RELEASE
# Sat, 22 Feb 2020 00:13:06 GMT
ENV SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.0.3-release SWIFT_VERSION=swift-5.0.3-RELEASE
# Sat, 22 Feb 2020 00:13:59 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && apt-get update     && apt-get install -y curl gpg     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           A62AE125BBBFBB96A6E042EC925CC1CCED3D1561         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && apt-get purge -y curl gpg     && apt-get -y autoremove     && rm -r /var/lib/apt/lists/*     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fe32ef0cb4aaeaba41c7cd5c3be7ac9b2dfbd16b0e6bdc1a00856d833d775d`  
		Last Modified: Sat, 22 Feb 2020 00:24:21 GMT  
		Size: 20.5 MB (20534267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dca9598437d829a748b15126e67b58c5c56272d24acf700515b70f58a14ac887`  
		Last Modified: Sat, 22 Feb 2020 00:24:23 GMT  
		Size: 27.9 MB (27899358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.0.3-xenial`

```console
$ docker pull swift@sha256:b65295dcc2d17989c0b990947f1b680224d01d1c64611970b47e2e6c8869dcea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.0.3-xenial` - linux; amd64

```console
$ docker pull swift@sha256:d61cd776b180b30febf0bcbef737cbc53c1e3b93ab62afa9f04eb69c7778ccb1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **478.1 MB (478078005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a558c7100696556adb4ce96dae4bd5983d899f6c9691d2e1d2131f12e8756b16`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:04:42 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Sat, 22 Feb 2020 00:04:43 GMT
LABEL Description=Docker Container for the Swift programming language
# Sat, 22 Feb 2020 00:11:46 GMT
RUN apt-get -q update &&     apt-get -q install -y     libatomic1     libbsd0     libcurl3     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:11:46 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Sat, 22 Feb 2020 00:11:47 GMT
ARG SWIFT_BRANCH=swift-5.0.3-release
# Sat, 22 Feb 2020 00:11:47 GMT
ARG SWIFT_VERSION=swift-5.0.3-RELEASE
# Sat, 22 Feb 2020 00:11:47 GMT
ENV SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-5.0.3-release SWIFT_VERSION=swift-5.0.3-RELEASE
# Sat, 22 Feb 2020 00:12:45 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && apt-get -q update     && apt-get -q install -y curl     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && apt-get purge -y curl     && apt-get -y autoremove     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           A62AE125BBBFBB96A6E042EC925CC1CCED3D1561         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
# Sat, 22 Feb 2020 00:12:47 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1c54fc70c7c38e98e86b9a5d9332aa63ff2244a103bc12e06deceb4426b8e4`  
		Last Modified: Sat, 22 Feb 2020 00:23:39 GMT  
		Size: 111.4 MB (111399409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3805986177e0da62fb835911f303747ba8de512a774dec7ff8198f43c28be00f`  
		Last Modified: Sat, 22 Feb 2020 00:24:12 GMT  
		Size: 322.5 MB (322485325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.0.3-xenial-slim`

```console
$ docker pull swift@sha256:e1800f9f033359559968cb918f4d9af3119e74247b3d8e92e7deca806268d444
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.0.3-xenial-slim` - linux; amd64

```console
$ docker pull swift@sha256:4e53517b151c7523b54154f1e42a63e3fa1ffcd6f44e6a4f2bfc35ea9e685698
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.9 MB (92904615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1695a7f1394f1e281dec43c57bbbefa09f6882d705add3d853d67505db25c9c9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:04:42 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Sat, 22 Feb 2020 00:04:43 GMT
LABEL Description=Docker Container for the Swift programming language
# Sat, 22 Feb 2020 00:14:19 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libbsd0     libcurl3     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:14:20 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Sat, 22 Feb 2020 00:14:20 GMT
ARG SWIFT_BRANCH=swift-5.0.3-release
# Sat, 22 Feb 2020 00:14:20 GMT
ARG SWIFT_VERSION=swift-5.0.3-RELEASE
# Sat, 22 Feb 2020 00:14:20 GMT
ENV SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-5.0.3-release SWIFT_VERSION=swift-5.0.3-RELEASE
# Sat, 22 Feb 2020 00:15:12 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && apt-get update     && apt-get install -y curl     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           A62AE125BBBFBB96A6E042EC925CC1CCED3D1561         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && apt-get purge -y curl     && apt-get -y autoremove     && rm -r /var/lib/apt/lists/*     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3953e5f397cc8952896cdbe323393a1f84291cdba32553ec213fb5a10166aa0f`  
		Last Modified: Sat, 22 Feb 2020 00:24:33 GMT  
		Size: 20.9 MB (20925756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5a6f25b0ca69f497f684bbab55b64774208fe836db07ef3eed06738e6de48c`  
		Last Modified: Sat, 22 Feb 2020 00:24:33 GMT  
		Size: 27.8 MB (27785588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.0-bionic`

```console
$ docker pull swift@sha256:6d8b85b1592e97300ce4081ecfd4474ce4a9f6894a83d02ea9ba35d988f04f95
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.0-bionic` - linux; amd64

```console
$ docker pull swift@sha256:697710b03142b8861805b2ae5118589da95cac354d44cba53005f30e095e5b25
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.0 MB (462992218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14aec6b7b3af2bbc3637e113dd87f5e26fdb6f4386b52198b48c8ba78f2704f4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL Description=Docker Container for the Swift programming language
# Sat, 22 Feb 2020 00:09:53 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libbsd0     libcurl4     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:09:54 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Sat, 22 Feb 2020 00:09:54 GMT
ARG SWIFT_BRANCH=swift-5.0.3-release
# Sat, 22 Feb 2020 00:09:54 GMT
ARG SWIFT_VERSION=swift-5.0.3-RELEASE
# Sat, 22 Feb 2020 00:09:54 GMT
ENV SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.0.3-release SWIFT_VERSION=swift-5.0.3-RELEASE
# Sat, 22 Feb 2020 00:10:52 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && apt-get update     && apt-get install -y curl     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && apt-get purge -y curl     && apt-get -y autoremove     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           A62AE125BBBFBB96A6E042EC925CC1CCED3D1561         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
# Sat, 22 Feb 2020 00:10:58 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1154b15f1870c37c0f357d3b1a6acd21c02d8f3c0d0c3d828132e43ea3cc44cf`  
		Last Modified: Sat, 22 Feb 2020 00:22:40 GMT  
		Size: 117.0 MB (116965374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007c485330fb667e606d6c6382c6b3fd0f17510af7853f7e378c6c42ed22f9ff`  
		Last Modified: Sat, 22 Feb 2020 00:23:09 GMT  
		Size: 319.3 MB (319298368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.0-bionic-slim`

```console
$ docker pull swift@sha256:2d9ce495c9043696d6ff1e284686f71a5fa0b89156456ed3530acd959b674945
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.0-bionic-slim` - linux; amd64

```console
$ docker pull swift@sha256:f2890b98664d7abea2e819df17322a7e0c8817ee83c1aed11ce9d3a257728795
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75162101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faf14f6fc2e147276289d4e5c0842a2859c0f4d0edc97341a84878958deaf8ae`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL Description=Docker Container for the Swift programming language
# Sat, 22 Feb 2020 00:13:05 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libbsd0     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:13:06 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Sat, 22 Feb 2020 00:13:06 GMT
ARG SWIFT_BRANCH=swift-5.0.3-release
# Sat, 22 Feb 2020 00:13:06 GMT
ARG SWIFT_VERSION=swift-5.0.3-RELEASE
# Sat, 22 Feb 2020 00:13:06 GMT
ENV SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.0.3-release SWIFT_VERSION=swift-5.0.3-RELEASE
# Sat, 22 Feb 2020 00:13:59 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && apt-get update     && apt-get install -y curl gpg     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           A62AE125BBBFBB96A6E042EC925CC1CCED3D1561         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && apt-get purge -y curl gpg     && apt-get -y autoremove     && rm -r /var/lib/apt/lists/*     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fe32ef0cb4aaeaba41c7cd5c3be7ac9b2dfbd16b0e6bdc1a00856d833d775d`  
		Last Modified: Sat, 22 Feb 2020 00:24:21 GMT  
		Size: 20.5 MB (20534267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dca9598437d829a748b15126e67b58c5c56272d24acf700515b70f58a14ac887`  
		Last Modified: Sat, 22 Feb 2020 00:24:23 GMT  
		Size: 27.9 MB (27899358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.0-slim`

```console
$ docker pull swift@sha256:2d9ce495c9043696d6ff1e284686f71a5fa0b89156456ed3530acd959b674945
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.0-slim` - linux; amd64

```console
$ docker pull swift@sha256:f2890b98664d7abea2e819df17322a7e0c8817ee83c1aed11ce9d3a257728795
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75162101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faf14f6fc2e147276289d4e5c0842a2859c0f4d0edc97341a84878958deaf8ae`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL Description=Docker Container for the Swift programming language
# Sat, 22 Feb 2020 00:13:05 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libbsd0     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:13:06 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Sat, 22 Feb 2020 00:13:06 GMT
ARG SWIFT_BRANCH=swift-5.0.3-release
# Sat, 22 Feb 2020 00:13:06 GMT
ARG SWIFT_VERSION=swift-5.0.3-RELEASE
# Sat, 22 Feb 2020 00:13:06 GMT
ENV SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.0.3-release SWIFT_VERSION=swift-5.0.3-RELEASE
# Sat, 22 Feb 2020 00:13:59 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && apt-get update     && apt-get install -y curl gpg     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           A62AE125BBBFBB96A6E042EC925CC1CCED3D1561         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && apt-get purge -y curl gpg     && apt-get -y autoremove     && rm -r /var/lib/apt/lists/*     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fe32ef0cb4aaeaba41c7cd5c3be7ac9b2dfbd16b0e6bdc1a00856d833d775d`  
		Last Modified: Sat, 22 Feb 2020 00:24:21 GMT  
		Size: 20.5 MB (20534267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dca9598437d829a748b15126e67b58c5c56272d24acf700515b70f58a14ac887`  
		Last Modified: Sat, 22 Feb 2020 00:24:23 GMT  
		Size: 27.9 MB (27899358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.0-xenial`

```console
$ docker pull swift@sha256:b65295dcc2d17989c0b990947f1b680224d01d1c64611970b47e2e6c8869dcea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.0-xenial` - linux; amd64

```console
$ docker pull swift@sha256:d61cd776b180b30febf0bcbef737cbc53c1e3b93ab62afa9f04eb69c7778ccb1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **478.1 MB (478078005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a558c7100696556adb4ce96dae4bd5983d899f6c9691d2e1d2131f12e8756b16`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:04:42 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Sat, 22 Feb 2020 00:04:43 GMT
LABEL Description=Docker Container for the Swift programming language
# Sat, 22 Feb 2020 00:11:46 GMT
RUN apt-get -q update &&     apt-get -q install -y     libatomic1     libbsd0     libcurl3     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:11:46 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Sat, 22 Feb 2020 00:11:47 GMT
ARG SWIFT_BRANCH=swift-5.0.3-release
# Sat, 22 Feb 2020 00:11:47 GMT
ARG SWIFT_VERSION=swift-5.0.3-RELEASE
# Sat, 22 Feb 2020 00:11:47 GMT
ENV SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-5.0.3-release SWIFT_VERSION=swift-5.0.3-RELEASE
# Sat, 22 Feb 2020 00:12:45 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && apt-get -q update     && apt-get -q install -y curl     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && apt-get purge -y curl     && apt-get -y autoremove     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           A62AE125BBBFBB96A6E042EC925CC1CCED3D1561         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
# Sat, 22 Feb 2020 00:12:47 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1c54fc70c7c38e98e86b9a5d9332aa63ff2244a103bc12e06deceb4426b8e4`  
		Last Modified: Sat, 22 Feb 2020 00:23:39 GMT  
		Size: 111.4 MB (111399409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3805986177e0da62fb835911f303747ba8de512a774dec7ff8198f43c28be00f`  
		Last Modified: Sat, 22 Feb 2020 00:24:12 GMT  
		Size: 322.5 MB (322485325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.0-xenial-slim`

```console
$ docker pull swift@sha256:e1800f9f033359559968cb918f4d9af3119e74247b3d8e92e7deca806268d444
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.0-xenial-slim` - linux; amd64

```console
$ docker pull swift@sha256:4e53517b151c7523b54154f1e42a63e3fa1ffcd6f44e6a4f2bfc35ea9e685698
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.9 MB (92904615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1695a7f1394f1e281dec43c57bbbefa09f6882d705add3d853d67505db25c9c9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:04:42 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Sat, 22 Feb 2020 00:04:43 GMT
LABEL Description=Docker Container for the Swift programming language
# Sat, 22 Feb 2020 00:14:19 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libbsd0     libcurl3     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:14:20 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Sat, 22 Feb 2020 00:14:20 GMT
ARG SWIFT_BRANCH=swift-5.0.3-release
# Sat, 22 Feb 2020 00:14:20 GMT
ARG SWIFT_VERSION=swift-5.0.3-RELEASE
# Sat, 22 Feb 2020 00:14:20 GMT
ENV SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-5.0.3-release SWIFT_VERSION=swift-5.0.3-RELEASE
# Sat, 22 Feb 2020 00:15:12 GMT
RUN SWIFT_URL=https://swift.org/builds/$SWIFT_BRANCH/$(echo "$SWIFT_PLATFORM" | tr -d .)/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz     && apt-get update     && apt-get install -y curl     && curl -fSsL $SWIFT_URL -o swift.tar.gz     && curl -fSsL $SWIFT_URL.sig -o swift.tar.gz.sig     && export GNUPGHOME="$(mktemp -d)"     && set -e;         for key in           A62AE125BBBFBB96A6E042EC925CC1CCED3D1561         ; do           gpg --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";         done     && gpg --batch --verify --quiet swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && apt-get purge -y curl     && apt-get -y autoremove     && rm -r /var/lib/apt/lists/*     && rm -r "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && chmod -R o+r /usr/lib/swift
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3953e5f397cc8952896cdbe323393a1f84291cdba32553ec213fb5a10166aa0f`  
		Last Modified: Sat, 22 Feb 2020 00:24:33 GMT  
		Size: 20.9 MB (20925756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5a6f25b0ca69f497f684bbab55b64774208fe836db07ef3eed06738e6de48c`  
		Last Modified: Sat, 22 Feb 2020 00:24:33 GMT  
		Size: 27.8 MB (27785588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.1`

```console
$ docker pull swift@sha256:d0600eae226a2b57f8b44846c6659628ec909ecf4d5b8993a8c4f6b5308d7d38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.1` - linux; amd64

```console
$ docker pull swift@sha256:82abef2505dff15317c4dc15953cc1e68669b87ce9ff96030121718f6592e42a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **496.6 MB (496641224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2aab8720dd13d426ba54e90da4f865387441cba1f3f4df7a4f409b3be7723310`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 13 Mar 2020 01:26:26 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Fri, 13 Mar 2020 01:26:27 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 13 Mar 2020 01:26:27 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Fri, 13 Mar 2020 01:26:27 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Fri, 13 Mar 2020 01:26:27 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Fri, 13 Mar 2020 01:26:28 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 13 Mar 2020 01:26:28 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 13 Mar 2020 01:27:35 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Fri, 13 Mar 2020 01:27:38 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f802bea27d7bff5717d70e483efdb17f0c8936780641d7241ddad972de8f292`  
		Last Modified: Fri, 13 Mar 2020 01:33:14 GMT  
		Size: 124.7 MB (124744291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:336540666c2d91b80745843c34812e22f2ae9187594023bed3452545386f32b4`  
		Last Modified: Fri, 13 Mar 2020 01:33:49 GMT  
		Size: 345.2 MB (345168457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.1.5`

```console
$ docker pull swift@sha256:d0600eae226a2b57f8b44846c6659628ec909ecf4d5b8993a8c4f6b5308d7d38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.1.5` - linux; amd64

```console
$ docker pull swift@sha256:82abef2505dff15317c4dc15953cc1e68669b87ce9ff96030121718f6592e42a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **496.6 MB (496641224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2aab8720dd13d426ba54e90da4f865387441cba1f3f4df7a4f409b3be7723310`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 13 Mar 2020 01:26:26 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Fri, 13 Mar 2020 01:26:27 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 13 Mar 2020 01:26:27 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Fri, 13 Mar 2020 01:26:27 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Fri, 13 Mar 2020 01:26:27 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Fri, 13 Mar 2020 01:26:28 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 13 Mar 2020 01:26:28 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 13 Mar 2020 01:27:35 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Fri, 13 Mar 2020 01:27:38 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f802bea27d7bff5717d70e483efdb17f0c8936780641d7241ddad972de8f292`  
		Last Modified: Fri, 13 Mar 2020 01:33:14 GMT  
		Size: 124.7 MB (124744291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:336540666c2d91b80745843c34812e22f2ae9187594023bed3452545386f32b4`  
		Last Modified: Fri, 13 Mar 2020 01:33:49 GMT  
		Size: 345.2 MB (345168457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.1.5-bionic`

```console
$ docker pull swift@sha256:d0600eae226a2b57f8b44846c6659628ec909ecf4d5b8993a8c4f6b5308d7d38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.1.5-bionic` - linux; amd64

```console
$ docker pull swift@sha256:82abef2505dff15317c4dc15953cc1e68669b87ce9ff96030121718f6592e42a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **496.6 MB (496641224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2aab8720dd13d426ba54e90da4f865387441cba1f3f4df7a4f409b3be7723310`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 13 Mar 2020 01:26:26 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Fri, 13 Mar 2020 01:26:27 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 13 Mar 2020 01:26:27 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Fri, 13 Mar 2020 01:26:27 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Fri, 13 Mar 2020 01:26:27 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Fri, 13 Mar 2020 01:26:28 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 13 Mar 2020 01:26:28 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 13 Mar 2020 01:27:35 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Fri, 13 Mar 2020 01:27:38 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f802bea27d7bff5717d70e483efdb17f0c8936780641d7241ddad972de8f292`  
		Last Modified: Fri, 13 Mar 2020 01:33:14 GMT  
		Size: 124.7 MB (124744291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:336540666c2d91b80745843c34812e22f2ae9187594023bed3452545386f32b4`  
		Last Modified: Fri, 13 Mar 2020 01:33:49 GMT  
		Size: 345.2 MB (345168457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.1.5-bionic-sim`

```console
$ docker pull swift@sha256:40dc11956654a968c0c888b7c40305bd05204413f55cdf84366135e04b94b8c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.1.5-bionic-sim` - linux; amd64

```console
$ docker pull swift@sha256:876f54d9ce5f2bda5b625eba1c90cc27712c7a52e064a26c411a2283b5610ed0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78300095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e14bba190fe7dc3af7987aeef1281764929e3d31d5d18a9e2b29e256d1062359`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL Description=Docker Container for the Swift programming language
# Sat, 22 Feb 2020 00:06:52 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:06:53 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Sat, 22 Feb 2020 00:06:53 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Fri, 13 Mar 2020 01:30:07 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Fri, 13 Mar 2020 01:30:07 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Fri, 13 Mar 2020 01:30:07 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 13 Mar 2020 01:30:07 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 13 Mar 2020 01:31:06 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl gnupg && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl gnupg
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab88b7e0fc274afd6609f73a28ce38510199134a6e7bc5214f175af178e0ea2`  
		Last Modified: Sat, 22 Feb 2020 00:21:51 GMT  
		Size: 20.5 MB (20488296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e1070a33f4013a224968327047dadf53d79d7c39ff72c33bb29a42da20f704`  
		Last Modified: Fri, 13 Mar 2020 01:35:13 GMT  
		Size: 31.1 MB (31083323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.1.5-slim`

```console
$ docker pull swift@sha256:40dc11956654a968c0c888b7c40305bd05204413f55cdf84366135e04b94b8c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.1.5-slim` - linux; amd64

```console
$ docker pull swift@sha256:876f54d9ce5f2bda5b625eba1c90cc27712c7a52e064a26c411a2283b5610ed0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78300095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e14bba190fe7dc3af7987aeef1281764929e3d31d5d18a9e2b29e256d1062359`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL Description=Docker Container for the Swift programming language
# Sat, 22 Feb 2020 00:06:52 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:06:53 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Sat, 22 Feb 2020 00:06:53 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Fri, 13 Mar 2020 01:30:07 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Fri, 13 Mar 2020 01:30:07 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Fri, 13 Mar 2020 01:30:07 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 13 Mar 2020 01:30:07 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 13 Mar 2020 01:31:06 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl gnupg && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl gnupg
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab88b7e0fc274afd6609f73a28ce38510199134a6e7bc5214f175af178e0ea2`  
		Last Modified: Sat, 22 Feb 2020 00:21:51 GMT  
		Size: 20.5 MB (20488296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e1070a33f4013a224968327047dadf53d79d7c39ff72c33bb29a42da20f704`  
		Last Modified: Fri, 13 Mar 2020 01:35:13 GMT  
		Size: 31.1 MB (31083323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.1.5-xenial`

```console
$ docker pull swift@sha256:648ce6263c9bef1edd926949bb6dad0f47edfba4924a6ffdb57013d28f19bb60
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.1.5-xenial` - linux; amd64

```console
$ docker pull swift@sha256:eb6766d00fa0ef87eb71a6fbf19ab824886b3a30e3d773f281e0b37363551cc8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **507.3 MB (507251641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69ff652aea089ceee0cc1940f36888585e955c15faf2a7b25dc71046f30ddb14`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:04:42 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Sat, 22 Feb 2020 00:04:43 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 13 Mar 2020 01:28:45 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl3     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Fri, 13 Mar 2020 01:28:45 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 13 Mar 2020 01:28:46 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Fri, 13 Mar 2020 01:28:46 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Fri, 13 Mar 2020 01:28:46 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Fri, 13 Mar 2020 01:28:46 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 13 Mar 2020 01:28:46 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 13 Mar 2020 01:29:53 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Fri, 13 Mar 2020 01:29:55 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee86ac70c7e2bef509323d225f54d9bbfd0259e0dbbf42b8f08d418906ff116`  
		Last Modified: Fri, 13 Mar 2020 01:34:18 GMT  
		Size: 111.6 MB (111583590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc715868d9a4c3f0023e1e61c8a757b28246bd9323ae6543d3c51740b9fb5ed`  
		Last Modified: Fri, 13 Mar 2020 01:34:58 GMT  
		Size: 351.5 MB (351474780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.1.5-xenial-slim`

```console
$ docker pull swift@sha256:d6d6801d108036cfb4ffdb8c7621e464ea6ef6ab71c76ca9eb3ac40c0bd25b87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.1.5-xenial-slim` - linux; amd64

```console
$ docker pull swift@sha256:0f8e22c34fe7ab2288c9baaa30c8e0a4492c436b4b4a55c5274f3f97fb7cadb2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.0 MB (96019434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72f9e1ce46534baeccd60b2078308fbe70f69d2cdd8bedcad6e90b16016f9a4d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:04:42 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Sat, 22 Feb 2020 00:04:43 GMT
LABEL Description=Docker Container for the Swift programming language
# Sat, 22 Feb 2020 00:08:21 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl3     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:08:21 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Sat, 22 Feb 2020 00:08:21 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Fri, 13 Mar 2020 01:31:10 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Fri, 13 Mar 2020 01:31:10 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Fri, 13 Mar 2020 01:31:11 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 13 Mar 2020 01:31:11 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 13 Mar 2020 01:32:08 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f5af521ca427b471b7529129aecf0a5a7f80ad9c0b7ab55b17664a2edfc777`  
		Last Modified: Sat, 22 Feb 2020 00:22:03 GMT  
		Size: 20.9 MB (20872636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf200801be1363637c64a249a5aee675b0d96fe244548f2753f805c516fc27cd`  
		Last Modified: Fri, 13 Mar 2020 01:35:25 GMT  
		Size: 31.0 MB (30953527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.1-bionic`

```console
$ docker pull swift@sha256:d0600eae226a2b57f8b44846c6659628ec909ecf4d5b8993a8c4f6b5308d7d38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.1-bionic` - linux; amd64

```console
$ docker pull swift@sha256:82abef2505dff15317c4dc15953cc1e68669b87ce9ff96030121718f6592e42a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **496.6 MB (496641224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2aab8720dd13d426ba54e90da4f865387441cba1f3f4df7a4f409b3be7723310`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 13 Mar 2020 01:26:26 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Fri, 13 Mar 2020 01:26:27 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 13 Mar 2020 01:26:27 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Fri, 13 Mar 2020 01:26:27 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Fri, 13 Mar 2020 01:26:27 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Fri, 13 Mar 2020 01:26:28 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 13 Mar 2020 01:26:28 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 13 Mar 2020 01:27:35 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Fri, 13 Mar 2020 01:27:38 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f802bea27d7bff5717d70e483efdb17f0c8936780641d7241ddad972de8f292`  
		Last Modified: Fri, 13 Mar 2020 01:33:14 GMT  
		Size: 124.7 MB (124744291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:336540666c2d91b80745843c34812e22f2ae9187594023bed3452545386f32b4`  
		Last Modified: Fri, 13 Mar 2020 01:33:49 GMT  
		Size: 345.2 MB (345168457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.1-bionic-slim`

```console
$ docker pull swift@sha256:40dc11956654a968c0c888b7c40305bd05204413f55cdf84366135e04b94b8c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.1-bionic-slim` - linux; amd64

```console
$ docker pull swift@sha256:876f54d9ce5f2bda5b625eba1c90cc27712c7a52e064a26c411a2283b5610ed0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78300095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e14bba190fe7dc3af7987aeef1281764929e3d31d5d18a9e2b29e256d1062359`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL Description=Docker Container for the Swift programming language
# Sat, 22 Feb 2020 00:06:52 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:06:53 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Sat, 22 Feb 2020 00:06:53 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Fri, 13 Mar 2020 01:30:07 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Fri, 13 Mar 2020 01:30:07 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Fri, 13 Mar 2020 01:30:07 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 13 Mar 2020 01:30:07 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 13 Mar 2020 01:31:06 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl gnupg && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl gnupg
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab88b7e0fc274afd6609f73a28ce38510199134a6e7bc5214f175af178e0ea2`  
		Last Modified: Sat, 22 Feb 2020 00:21:51 GMT  
		Size: 20.5 MB (20488296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e1070a33f4013a224968327047dadf53d79d7c39ff72c33bb29a42da20f704`  
		Last Modified: Fri, 13 Mar 2020 01:35:13 GMT  
		Size: 31.1 MB (31083323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.1-slim`

```console
$ docker pull swift@sha256:40dc11956654a968c0c888b7c40305bd05204413f55cdf84366135e04b94b8c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.1-slim` - linux; amd64

```console
$ docker pull swift@sha256:876f54d9ce5f2bda5b625eba1c90cc27712c7a52e064a26c411a2283b5610ed0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78300095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e14bba190fe7dc3af7987aeef1281764929e3d31d5d18a9e2b29e256d1062359`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL Description=Docker Container for the Swift programming language
# Sat, 22 Feb 2020 00:06:52 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:06:53 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Sat, 22 Feb 2020 00:06:53 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Fri, 13 Mar 2020 01:30:07 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Fri, 13 Mar 2020 01:30:07 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Fri, 13 Mar 2020 01:30:07 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 13 Mar 2020 01:30:07 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 13 Mar 2020 01:31:06 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl gnupg && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl gnupg
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab88b7e0fc274afd6609f73a28ce38510199134a6e7bc5214f175af178e0ea2`  
		Last Modified: Sat, 22 Feb 2020 00:21:51 GMT  
		Size: 20.5 MB (20488296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e1070a33f4013a224968327047dadf53d79d7c39ff72c33bb29a42da20f704`  
		Last Modified: Fri, 13 Mar 2020 01:35:13 GMT  
		Size: 31.1 MB (31083323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.1-xenial`

```console
$ docker pull swift@sha256:648ce6263c9bef1edd926949bb6dad0f47edfba4924a6ffdb57013d28f19bb60
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.1-xenial` - linux; amd64

```console
$ docker pull swift@sha256:eb6766d00fa0ef87eb71a6fbf19ab824886b3a30e3d773f281e0b37363551cc8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **507.3 MB (507251641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69ff652aea089ceee0cc1940f36888585e955c15faf2a7b25dc71046f30ddb14`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:04:42 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Sat, 22 Feb 2020 00:04:43 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 13 Mar 2020 01:28:45 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl3     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Fri, 13 Mar 2020 01:28:45 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 13 Mar 2020 01:28:46 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Fri, 13 Mar 2020 01:28:46 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Fri, 13 Mar 2020 01:28:46 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Fri, 13 Mar 2020 01:28:46 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 13 Mar 2020 01:28:46 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 13 Mar 2020 01:29:53 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Fri, 13 Mar 2020 01:29:55 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee86ac70c7e2bef509323d225f54d9bbfd0259e0dbbf42b8f08d418906ff116`  
		Last Modified: Fri, 13 Mar 2020 01:34:18 GMT  
		Size: 111.6 MB (111583590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc715868d9a4c3f0023e1e61c8a757b28246bd9323ae6543d3c51740b9fb5ed`  
		Last Modified: Fri, 13 Mar 2020 01:34:58 GMT  
		Size: 351.5 MB (351474780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:5.1-xenial-slim`

```console
$ docker pull swift@sha256:d6d6801d108036cfb4ffdb8c7621e464ea6ef6ab71c76ca9eb3ac40c0bd25b87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:5.1-xenial-slim` - linux; amd64

```console
$ docker pull swift@sha256:0f8e22c34fe7ab2288c9baaa30c8e0a4492c436b4b4a55c5274f3f97fb7cadb2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.0 MB (96019434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72f9e1ce46534baeccd60b2078308fbe70f69d2cdd8bedcad6e90b16016f9a4d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:04:42 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Sat, 22 Feb 2020 00:04:43 GMT
LABEL Description=Docker Container for the Swift programming language
# Sat, 22 Feb 2020 00:08:21 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl3     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:08:21 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Sat, 22 Feb 2020 00:08:21 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Fri, 13 Mar 2020 01:31:10 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Fri, 13 Mar 2020 01:31:10 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Fri, 13 Mar 2020 01:31:11 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 13 Mar 2020 01:31:11 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 13 Mar 2020 01:32:08 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f5af521ca427b471b7529129aecf0a5a7f80ad9c0b7ab55b17664a2edfc777`  
		Last Modified: Sat, 22 Feb 2020 00:22:03 GMT  
		Size: 20.9 MB (20872636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf200801be1363637c64a249a5aee675b0d96fe244548f2753f805c516fc27cd`  
		Last Modified: Fri, 13 Mar 2020 01:35:25 GMT  
		Size: 31.0 MB (30953527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:bionic`

```console
$ docker pull swift@sha256:d0600eae226a2b57f8b44846c6659628ec909ecf4d5b8993a8c4f6b5308d7d38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:bionic` - linux; amd64

```console
$ docker pull swift@sha256:82abef2505dff15317c4dc15953cc1e68669b87ce9ff96030121718f6592e42a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **496.6 MB (496641224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2aab8720dd13d426ba54e90da4f865387441cba1f3f4df7a4f409b3be7723310`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 13 Mar 2020 01:26:26 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Fri, 13 Mar 2020 01:26:27 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 13 Mar 2020 01:26:27 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Fri, 13 Mar 2020 01:26:27 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Fri, 13 Mar 2020 01:26:27 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Fri, 13 Mar 2020 01:26:28 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 13 Mar 2020 01:26:28 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 13 Mar 2020 01:27:35 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Fri, 13 Mar 2020 01:27:38 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f802bea27d7bff5717d70e483efdb17f0c8936780641d7241ddad972de8f292`  
		Last Modified: Fri, 13 Mar 2020 01:33:14 GMT  
		Size: 124.7 MB (124744291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:336540666c2d91b80745843c34812e22f2ae9187594023bed3452545386f32b4`  
		Last Modified: Fri, 13 Mar 2020 01:33:49 GMT  
		Size: 345.2 MB (345168457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:bionic-slim`

```console
$ docker pull swift@sha256:40dc11956654a968c0c888b7c40305bd05204413f55cdf84366135e04b94b8c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:bionic-slim` - linux; amd64

```console
$ docker pull swift@sha256:876f54d9ce5f2bda5b625eba1c90cc27712c7a52e064a26c411a2283b5610ed0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78300095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e14bba190fe7dc3af7987aeef1281764929e3d31d5d18a9e2b29e256d1062359`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL Description=Docker Container for the Swift programming language
# Sat, 22 Feb 2020 00:06:52 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:06:53 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Sat, 22 Feb 2020 00:06:53 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Fri, 13 Mar 2020 01:30:07 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Fri, 13 Mar 2020 01:30:07 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Fri, 13 Mar 2020 01:30:07 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 13 Mar 2020 01:30:07 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 13 Mar 2020 01:31:06 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl gnupg && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl gnupg
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab88b7e0fc274afd6609f73a28ce38510199134a6e7bc5214f175af178e0ea2`  
		Last Modified: Sat, 22 Feb 2020 00:21:51 GMT  
		Size: 20.5 MB (20488296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e1070a33f4013a224968327047dadf53d79d7c39ff72c33bb29a42da20f704`  
		Last Modified: Fri, 13 Mar 2020 01:35:13 GMT  
		Size: 31.1 MB (31083323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:latest`

```console
$ docker pull swift@sha256:d0600eae226a2b57f8b44846c6659628ec909ecf4d5b8993a8c4f6b5308d7d38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:latest` - linux; amd64

```console
$ docker pull swift@sha256:82abef2505dff15317c4dc15953cc1e68669b87ce9ff96030121718f6592e42a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **496.6 MB (496641224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2aab8720dd13d426ba54e90da4f865387441cba1f3f4df7a4f409b3be7723310`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 13 Mar 2020 01:26:26 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Fri, 13 Mar 2020 01:26:27 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 13 Mar 2020 01:26:27 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Fri, 13 Mar 2020 01:26:27 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Fri, 13 Mar 2020 01:26:27 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Fri, 13 Mar 2020 01:26:28 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 13 Mar 2020 01:26:28 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 13 Mar 2020 01:27:35 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Fri, 13 Mar 2020 01:27:38 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f802bea27d7bff5717d70e483efdb17f0c8936780641d7241ddad972de8f292`  
		Last Modified: Fri, 13 Mar 2020 01:33:14 GMT  
		Size: 124.7 MB (124744291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:336540666c2d91b80745843c34812e22f2ae9187594023bed3452545386f32b4`  
		Last Modified: Fri, 13 Mar 2020 01:33:49 GMT  
		Size: 345.2 MB (345168457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:slim`

```console
$ docker pull swift@sha256:40dc11956654a968c0c888b7c40305bd05204413f55cdf84366135e04b94b8c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:slim` - linux; amd64

```console
$ docker pull swift@sha256:876f54d9ce5f2bda5b625eba1c90cc27712c7a52e064a26c411a2283b5610ed0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78300095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e14bba190fe7dc3af7987aeef1281764929e3d31d5d18a9e2b29e256d1062359`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Sat, 22 Feb 2020 00:02:42 GMT
LABEL Description=Docker Container for the Swift programming language
# Sat, 22 Feb 2020 00:06:52 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:06:53 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Sat, 22 Feb 2020 00:06:53 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Fri, 13 Mar 2020 01:30:07 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Fri, 13 Mar 2020 01:30:07 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Fri, 13 Mar 2020 01:30:07 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 13 Mar 2020 01:30:07 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 13 Mar 2020 01:31:06 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl gnupg && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl gnupg
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab88b7e0fc274afd6609f73a28ce38510199134a6e7bc5214f175af178e0ea2`  
		Last Modified: Sat, 22 Feb 2020 00:21:51 GMT  
		Size: 20.5 MB (20488296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e1070a33f4013a224968327047dadf53d79d7c39ff72c33bb29a42da20f704`  
		Last Modified: Fri, 13 Mar 2020 01:35:13 GMT  
		Size: 31.1 MB (31083323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:xenial`

```console
$ docker pull swift@sha256:648ce6263c9bef1edd926949bb6dad0f47edfba4924a6ffdb57013d28f19bb60
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:xenial` - linux; amd64

```console
$ docker pull swift@sha256:eb6766d00fa0ef87eb71a6fbf19ab824886b3a30e3d773f281e0b37363551cc8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **507.3 MB (507251641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69ff652aea089ceee0cc1940f36888585e955c15faf2a7b25dc71046f30ddb14`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:04:42 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Sat, 22 Feb 2020 00:04:43 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 13 Mar 2020 01:28:45 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl3     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython2.7     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Fri, 13 Mar 2020 01:28:45 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 13 Mar 2020 01:28:46 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Fri, 13 Mar 2020 01:28:46 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Fri, 13 Mar 2020 01:28:46 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Fri, 13 Mar 2020 01:28:46 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 13 Mar 2020 01:28:46 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 13 Mar 2020 01:29:53 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Fri, 13 Mar 2020 01:29:55 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee86ac70c7e2bef509323d225f54d9bbfd0259e0dbbf42b8f08d418906ff116`  
		Last Modified: Fri, 13 Mar 2020 01:34:18 GMT  
		Size: 111.6 MB (111583590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc715868d9a4c3f0023e1e61c8a757b28246bd9323ae6543d3c51740b9fb5ed`  
		Last Modified: Fri, 13 Mar 2020 01:34:58 GMT  
		Size: 351.5 MB (351474780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swift:xenial-slim`

```console
$ docker pull swift@sha256:d6d6801d108036cfb4ffdb8c7621e464ea6ef6ab71c76ca9eb3ac40c0bd25b87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:xenial-slim` - linux; amd64

```console
$ docker pull swift@sha256:0f8e22c34fe7ab2288c9baaa30c8e0a4492c436b4b4a55c5274f3f97fb7cadb2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.0 MB (96019434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72f9e1ce46534baeccd60b2078308fbe70f69d2cdd8bedcad6e90b16016f9a4d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:04:42 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Sat, 22 Feb 2020 00:04:43 GMT
LABEL Description=Docker Container for the Swift programming language
# Sat, 22 Feb 2020 00:08:21 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl3     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:08:21 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Sat, 22 Feb 2020 00:08:21 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Fri, 13 Mar 2020 01:31:10 GMT
ARG SWIFT_BRANCH=swift-5.1.5-release
# Fri, 13 Mar 2020 01:31:10 GMT
ARG SWIFT_VERSION=swift-5.1.5-RELEASE
# Fri, 13 Mar 2020 01:31:11 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 13 Mar 2020 01:31:11 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-5.1.5-release SWIFT_VERSION=swift-5.1.5-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 13 Mar 2020 01:32:08 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f5af521ca427b471b7529129aecf0a5a7f80ad9c0b7ab55b17664a2edfc777`  
		Last Modified: Sat, 22 Feb 2020 00:22:03 GMT  
		Size: 20.9 MB (20872636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf200801be1363637c64a249a5aee675b0d96fe244548f2753f805c516fc27cd`  
		Last Modified: Fri, 13 Mar 2020 01:35:25 GMT  
		Size: 31.0 MB (30953527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
