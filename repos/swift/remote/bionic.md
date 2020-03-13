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
