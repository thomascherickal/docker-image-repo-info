## `couchbase:enterprise-7.2.3`

```console
$ docker pull couchbase@sha256:5e5cf0ff763af2cc3676b0f180004c69a8ebcb5a2a69cb350df18ad793bb6b04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchbase:enterprise-7.2.3` - linux; amd64

```console
$ docker pull couchbase@sha256:3ba1eaad23b3fcd7f2072d0ca8e68ae2e2c4ced137d6a582e9b162aa072675bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **670.0 MB (670030067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2ed85a13e0a5d11ec439fbf0301fca61203dfdbbc3b1c0519c482acdce98cd9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 28 Nov 2023 05:17:39 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:17:41 GMT
ADD file:9169bb1d6ef21313aed17e924538fee03d858460ae6b05e01968457dfc043bd7 in / 
# Tue, 28 Nov 2023 05:17:41 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 04:31:16 GMT
LABEL maintainer=docker@couchbase.com
# Sat, 02 Dec 2023 04:31:16 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Sat, 02 Dec 2023 04:31:16 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Sat, 02 Dec 2023 04:31:57 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Sat, 02 Dec 2023 04:31:57 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.3
# Sat, 02 Dec 2023 04:31:57 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.2.3-linux_@@ARCH@@.deb
# Sat, 02 Dec 2023 04:31:57 GMT
ARG CB_SKIP_CHECKSUM=false
# Sat, 02 Dec 2023 04:31:57 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Sat, 02 Dec 2023 04:31:58 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Sat, 02 Dec 2023 04:32:59 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=1ca43fd4d5c7d390974ba5ae0465875b4c42687dd497ceadb2ef6816585e3ec7            ;;          'amd64')            CB_SHA256=941ad294cc93102b655290701e4f6f6c653c146dc525ade7c734047b3797e316            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Sat, 02 Dec 2023 04:33:03 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Sat, 02 Dec 2023 04:33:03 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Sat, 02 Dec 2023 04:33:04 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Sat, 02 Dec 2023 04:33:04 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Sat, 02 Dec 2023 04:33:04 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Sat, 02 Dec 2023 04:33:05 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Sat, 02 Dec 2023 04:33:05 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Sat, 02 Dec 2023 04:33:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 04:33:05 GMT
CMD ["couchbase-server"]
# Sat, 02 Dec 2023 04:33:05 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Sat, 02 Dec 2023 04:33:05 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:30ecab32a3b65c6ec04c63a65b90e627b49d1297d8793896ed50b656377d8a06`  
		Last Modified: Tue, 28 Nov 2023 10:11:56 GMT  
		Size: 28.6 MB (28584029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3d1c486e8f867c0ed736dbfaae0b4cbe06bc1921fb87b2cf512387368c5a4f0`  
		Last Modified: Sat, 02 Dec 2023 04:40:46 GMT  
		Size: 6.3 MB (6286102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9961f4a99857da1ed5260e158bf534c2f2f58b809cbdd055e7c2c378b21a964`  
		Last Modified: Sat, 02 Dec 2023 04:40:44 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b7966760cc0ca59e5aa6ba1e3487c94d6a6491452b7669a20f6af219e0fa89`  
		Last Modified: Sat, 02 Dec 2023 04:41:40 GMT  
		Size: 635.2 MB (635155566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c035bf7e5cbc383f2968fb0b9125fcfb9e1d96d7816f9c02c373d765ed47523`  
		Last Modified: Sat, 02 Dec 2023 04:40:44 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540b404a792e9f22f43fa8e028c7ee707e085c625c7609ae3fd545ce2eef35b8`  
		Last Modified: Sat, 02 Dec 2023 04:40:43 GMT  
		Size: 742.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40d38e87451bb08b7696a5fe662013ff84bce4af5cfe83e3a4a107e9347fc8df`  
		Last Modified: Sat, 02 Dec 2023 04:40:43 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c256f0adac900cace953387efd52767c6f6f4d21b83e9adb5e2fff5c44f4e78`  
		Last Modified: Sat, 02 Dec 2023 04:40:43 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af69f861712d526e1aa28d26a03c526817a03b5bc5bbd2563762cfa56e1c7a9d`  
		Last Modified: Sat, 02 Dec 2023 04:40:42 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40d0b195d33a02dcce034e17d792340cbad6be2f9b1b6ef715527e4c7d10f2c1`  
		Last Modified: Sat, 02 Dec 2023 04:40:43 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchbase:enterprise-7.2.3` - linux; arm64 variant v8

```console
$ docker pull couchbase@sha256:c585828ec42687fc9d207758935c9a780e3ca8682d8e23c5ab7084a46c2d9e9f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **641.4 MB (641440353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38a4327b152f8bb3a037cd08f5cb09884814910b266a73c9fa863039edcef92d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 28 Nov 2023 05:25:16 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:25:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:25:23 GMT
ADD file:f80c582e6edb1f05fc0cefc201be3c47d4b4c6ceb20889c434c9fdef0291cbbf in / 
# Tue, 28 Nov 2023 05:25:23 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 04:59:21 GMT
LABEL maintainer=docker@couchbase.com
# Sat, 02 Dec 2023 04:59:21 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Sat, 02 Dec 2023 04:59:21 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Sat, 02 Dec 2023 04:59:48 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Sat, 02 Dec 2023 04:59:48 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.3
# Sat, 02 Dec 2023 04:59:48 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.2.3-linux_@@ARCH@@.deb
# Sat, 02 Dec 2023 04:59:48 GMT
ARG CB_SKIP_CHECKSUM=false
# Sat, 02 Dec 2023 04:59:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Sat, 02 Dec 2023 04:59:49 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Sat, 02 Dec 2023 05:00:49 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=1ca43fd4d5c7d390974ba5ae0465875b4c42687dd497ceadb2ef6816585e3ec7            ;;          'amd64')            CB_SHA256=941ad294cc93102b655290701e4f6f6c653c146dc525ade7c734047b3797e316            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Sat, 02 Dec 2023 05:00:58 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Sat, 02 Dec 2023 05:00:58 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Sat, 02 Dec 2023 05:00:58 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Sat, 02 Dec 2023 05:00:58 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Sat, 02 Dec 2023 05:00:59 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Sat, 02 Dec 2023 05:00:59 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Sat, 02 Dec 2023 05:00:59 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Sat, 02 Dec 2023 05:01:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 05:01:00 GMT
CMD ["couchbase-server"]
# Sat, 02 Dec 2023 05:01:00 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Sat, 02 Dec 2023 05:01:00 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:5d2acf9ee7cfde47b6ce997317767b8fa9bf8d93b8297016db9e093d06aa913d`  
		Last Modified: Wed, 29 Nov 2023 17:47:09 GMT  
		Size: 27.2 MB (27203865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1112ac20343e3a25ff87942513bf8aa7ff9106ad70305e15d1af479240ab8618`  
		Last Modified: Sat, 02 Dec 2023 05:04:24 GMT  
		Size: 6.1 MB (6109501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3665ac99bdacff569c704ee81fec61e12164775085151a0e3b3bf4d02a23af49`  
		Last Modified: Sat, 02 Dec 2023 05:04:23 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24ac3864f69d15e5062aee05804675d1d83b4d07dd00ba0e8a1c3d4e54b7580f`  
		Last Modified: Sat, 02 Dec 2023 05:05:04 GMT  
		Size: 608.1 MB (608122622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758549d893a51b1305936cf2bb24d7b5aca693f6879d17914fd435cf8eb817af`  
		Last Modified: Sat, 02 Dec 2023 05:04:23 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c10fb9673d4c8f674ee6f00075dc638bd82fcd9902e5816f0aed2ef24ed7fda1`  
		Last Modified: Sat, 02 Dec 2023 05:04:21 GMT  
		Size: 744.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4fda8b8c85f9e057a315538bcd3183406e4f30cf0ce571fa6f1d791b9a3bb64`  
		Last Modified: Sat, 02 Dec 2023 05:04:21 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8488b730d1b6d59b95aad69e81c2eca5f177f6dabbbc53270a2ee8d5769a95`  
		Last Modified: Sat, 02 Dec 2023 05:04:21 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ace13a5f02b3b6240ef1067104d891a22f428ed4719e445fa49ff79c4492bf3`  
		Last Modified: Sat, 02 Dec 2023 05:04:21 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e827a82e9aad3511bdbd97492af6536ff9392be724019d82f5f834ae0a0b42`  
		Last Modified: Sat, 02 Dec 2023 05:04:21 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
