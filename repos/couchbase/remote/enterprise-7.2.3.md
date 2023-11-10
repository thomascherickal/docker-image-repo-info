## `couchbase:enterprise-7.2.3`

```console
$ docker pull couchbase@sha256:df43354ee813933e1007063ac5c488001f118e8a7aeccac7aabefb472c98a7f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchbase:enterprise-7.2.3` - linux; amd64

```console
$ docker pull couchbase@sha256:30a719eb55cf915ccc1fc3037c585659bf911a0290b8d29363f40e5406b853cc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **670.0 MB (670026981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db7fbc1619ff2425d0c59b892519586bb1b7cb4a3e8a8c2c5cb7518874eb3c64`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 03 Oct 2023 10:45:50 GMT
ARG RELEASE
# Tue, 03 Oct 2023 10:45:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 10:45:51 GMT
ADD file:4809da414c2d478b4d991cbdaa2df457f2b3d07d0ff6cf673f09a66f90833e81 in / 
# Tue, 03 Oct 2023 10:45:52 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:34:46 GMT
LABEL maintainer=docker@couchbase.com
# Fri, 13 Oct 2023 07:34:46 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Fri, 13 Oct 2023 07:34:46 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Fri, 13 Oct 2023 07:35:15 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Fri, 10 Nov 2023 02:29:47 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.3
# Fri, 10 Nov 2023 02:29:47 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.2.3-linux_@@ARCH@@.deb
# Fri, 10 Nov 2023 02:29:48 GMT
ARG CB_SKIP_CHECKSUM=false
# Fri, 10 Nov 2023 02:29:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 10 Nov 2023 02:29:48 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 10 Nov 2023 02:31:16 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=1ca43fd4d5c7d390974ba5ae0465875b4c42687dd497ceadb2ef6816585e3ec7            ;;          'amd64')            CB_SHA256=941ad294cc93102b655290701e4f6f6c653c146dc525ade7c734047b3797e316            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Fri, 10 Nov 2023 02:31:21 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Fri, 10 Nov 2023 02:31:21 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Fri, 10 Nov 2023 02:31:21 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Fri, 10 Nov 2023 02:31:21 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 10 Nov 2023 02:31:22 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 10 Nov 2023 02:31:23 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Fri, 10 Nov 2023 02:31:23 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Fri, 10 Nov 2023 02:31:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 10 Nov 2023 02:31:23 GMT
CMD ["couchbase-server"]
# Fri, 10 Nov 2023 02:31:23 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Fri, 10 Nov 2023 02:31:23 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:7a2c559011895d255fce249c00396abff5ae7e0c0a92931d0ed493e71de78e3a`  
		Last Modified: Tue, 03 Oct 2023 17:02:08 GMT  
		Size: 28.6 MB (28580681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f74dd8ee7b698aa30f6021db1eba8fe81ac68ece2c5829894a3fcc95667e11`  
		Last Modified: Fri, 13 Oct 2023 07:45:16 GMT  
		Size: 6.3 MB (6285994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1a75ff3a5b171e3c1c3fbc5afea445ecc3a08b39d72f9dc1e2947fca4f6122`  
		Last Modified: Fri, 10 Nov 2023 02:33:34 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a04f1697a41e55e09d502ee5eabcd3d679a6830482227c5b528bc0154a401693`  
		Last Modified: Fri, 10 Nov 2023 02:34:38 GMT  
		Size: 635.2 MB (635155930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aeda838f16da5cc23e88012cb185b110883252687a2f28e1da64d0e6365cc5b`  
		Last Modified: Fri, 10 Nov 2023 02:33:34 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7674453f6880dea13c982170b32f8b4718bd53850cd6d471d232ca214f50eb82`  
		Last Modified: Fri, 10 Nov 2023 02:33:32 GMT  
		Size: 746.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5067d0f6ca46c82b9cd877d9abb6a7cebb2b3604b01cdeffb6c61b8a214b5c8`  
		Last Modified: Fri, 10 Nov 2023 02:33:32 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a3f7c056770fb2d5384cde5cbd2d79cc17c2d624a90b0885c8411b9b55d56f`  
		Last Modified: Fri, 10 Nov 2023 02:33:32 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065cd9561ac344b31145954eb7bae61b22ea86a166357d456566feb0a0881734`  
		Last Modified: Fri, 10 Nov 2023 02:33:32 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35bd03b45f6589722d4e9af1cffcb8fb4a9341bab0732bf4b0494c2c363e5384`  
		Last Modified: Fri, 10 Nov 2023 02:33:32 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchbase:enterprise-7.2.3` - linux; arm64 variant v8

```console
$ docker pull couchbase@sha256:2402f3a3d7051ed014d44dc9efb414216ab5c6dab1e165caa6ed93c0cd5ffd6a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **641.4 MB (641436635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ab2cd176f47370879282a6af69e162fe7dd2dc83f4f109bc76717876418732d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 03 Oct 2023 11:04:09 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:04:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:04:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:04:10 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:04:16 GMT
ADD file:f70cc2610ea8fcd25e6e9ae727eb9345d5b7198102f6a6d8e458ab8f99efefc3 in / 
# Tue, 03 Oct 2023 11:04:17 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 03:56:50 GMT
LABEL maintainer=docker@couchbase.com
# Fri, 13 Oct 2023 03:56:50 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Fri, 13 Oct 2023 03:56:50 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Fri, 13 Oct 2023 03:57:08 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Fri, 10 Nov 2023 01:43:23 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.3
# Fri, 10 Nov 2023 01:43:23 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.2.3-linux_@@ARCH@@.deb
# Fri, 10 Nov 2023 01:43:23 GMT
ARG CB_SKIP_CHECKSUM=false
# Fri, 10 Nov 2023 01:43:23 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 10 Nov 2023 01:43:24 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 10 Nov 2023 01:44:20 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=1ca43fd4d5c7d390974ba5ae0465875b4c42687dd497ceadb2ef6816585e3ec7            ;;          'amd64')            CB_SHA256=941ad294cc93102b655290701e4f6f6c653c146dc525ade7c734047b3797e316            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Fri, 10 Nov 2023 01:44:28 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Fri, 10 Nov 2023 01:44:28 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Fri, 10 Nov 2023 01:44:28 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Fri, 10 Nov 2023 01:44:28 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 10 Nov 2023 01:44:29 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 10 Nov 2023 01:44:29 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Fri, 10 Nov 2023 01:44:29 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Fri, 10 Nov 2023 01:44:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 10 Nov 2023 01:44:30 GMT
CMD ["couchbase-server"]
# Fri, 10 Nov 2023 01:44:30 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Fri, 10 Nov 2023 01:44:30 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:6cba4020c0a193cd551ed8edf368670967e3546345b52c4ec66cb0931436e9b9`  
		Last Modified: Thu, 05 Oct 2023 12:12:17 GMT  
		Size: 27.2 MB (27199503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e1c15a1b1f2e05138fe2b49be3e2f9ea9a9dcd2a096c2ee69d1636a18082ef`  
		Last Modified: Fri, 13 Oct 2023 04:01:39 GMT  
		Size: 6.1 MB (6109875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cea53286f7ab7a97fa36583245885cc3353954c1c6d63130bc63d071cb6bb57`  
		Last Modified: Fri, 10 Nov 2023 01:46:10 GMT  
		Size: 1.8 KB (1846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a3c3a7b30e49189ae27bb559a88d0291f1caa58e78a480168843fcf2277609`  
		Last Modified: Fri, 10 Nov 2023 01:46:52 GMT  
		Size: 608.1 MB (608122879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2acf0fd612f89fabd0c3f99190d74f3cda970efdd7f8cb99f4f2c8556f730845`  
		Last Modified: Fri, 10 Nov 2023 01:46:10 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f77331fc2cc9d44ce7becda98387a00a4e2c22f7591e2721a86b86b89a8d16b0`  
		Last Modified: Fri, 10 Nov 2023 01:46:08 GMT  
		Size: 744.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532e1d7eeba3d9113ce36baebaeca71384413d551db4772a759d05dfcfdc246b`  
		Last Modified: Fri, 10 Nov 2023 01:46:09 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5764486cea1e5eaebd81b69ec3083bf81a1f630a1f5beb74672b617913c6f8c7`  
		Last Modified: Fri, 10 Nov 2023 01:46:08 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62496740dd163e95661a18f8a7526e9fdf54f719127088a9148dc19dcda36bfd`  
		Last Modified: Fri, 10 Nov 2023 01:46:08 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16edc0102aba9b82ae4ebb1632c780764d101dc09d3f869958e759bbecf1055b`  
		Last Modified: Fri, 10 Nov 2023 01:46:08 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
