## `swift:xenial`

```console
$ docker pull swift@sha256:d8f8a15f272d6905e45d529f4b12dde096bf80382890701ee7cf60bc7d87351f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `swift:xenial` - linux; amd64

```console
$ docker pull swift@sha256:adc59c184968a74f817f360fa69afecf91438be9bbdb9842da5d6a6432c4a9f3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **672.5 MB (672459227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c290d42b05c9d8eab8c2725edf0f7f006ed90b93a069f16ecb336d01bb40bd9e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:27 GMT
ADD file:11b425d4c08e81a3e0cb2e0345d27cd5fc844dd83f1096af4cc05f635824ff5d in / 
# Tue, 31 Aug 2021 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:21:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:21:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:21:30 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 05:16:23 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Tue, 31 Aug 2021 05:16:23 GMT
LABEL Description=Docker Container for the Swift programming language
# Tue, 31 Aug 2021 05:18:24 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl3     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython3.5     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Tue, 31 Aug 2021 05:18:25 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Tue, 31 Aug 2021 05:18:25 GMT
ARG SWIFT_PLATFORM=ubuntu16.04
# Tue, 31 Aug 2021 05:18:25 GMT
ARG SWIFT_BRANCH=swift-5.4.2-release
# Tue, 31 Aug 2021 05:18:25 GMT
ARG SWIFT_VERSION=swift-5.4.2-RELEASE
# Tue, 31 Aug 2021 05:18:26 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Tue, 31 Aug 2021 05:18:26 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu16.04 SWIFT_BRANCH=swift-5.4.2-release SWIFT_VERSION=swift-5.4.2-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Tue, 31 Aug 2021 05:20:01 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Tue, 31 Aug 2021 05:20:06 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:58690f9b18fca6469a14da4e212c96849469f9b1be6661d2342a4bf01774aa50`  
		Last Modified: Thu, 05 Aug 2021 00:25:05 GMT  
		Size: 46.5 MB (46497548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51569e7c50720acf6860327847fe342a1afbe148d24c529fb81df105e3eed01`  
		Last Modified: Tue, 31 Aug 2021 01:23:09 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ef40b9ecabc2679fe2419957220c0272a965c5cf7e0269fa1aeeb8c56f2e1`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb15d46c38dcd1ea0b1990006c3366ecd10c79d374f341687eb2cb23a2c8672e`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec569ec8e60d23e246bc888957209531c7b313d0021e6f7ab2b999f599d5b1d8`  
		Last Modified: Tue, 31 Aug 2021 06:11:28 GMT  
		Size: 112.7 MB (112670487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4228ce03313e14c0a4c076aae3d25fa53e3719243441b363c54369d56c0a0f16`  
		Last Modified: Tue, 31 Aug 2021 06:12:25 GMT  
		Size: 513.3 MB (513289637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
