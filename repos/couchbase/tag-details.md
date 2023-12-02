<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `couchbase`

-	[`couchbase:6.6.6`](#couchbase666)
-	[`couchbase:7.0.5`](#couchbase705)
-	[`couchbase:7.1.6`](#couchbase716)
-	[`couchbase:7.2.3`](#couchbase723)
-	[`couchbase:community`](#couchbasecommunity)
-	[`couchbase:community-6.6.0`](#couchbasecommunity-660)
-	[`couchbase:community-7.0.2`](#couchbasecommunity-702)
-	[`couchbase:community-7.1.1`](#couchbasecommunity-711)
-	[`couchbase:community-7.2.2`](#couchbasecommunity-722)
-	[`couchbase:enterprise`](#couchbaseenterprise)
-	[`couchbase:enterprise-6.6.6`](#couchbaseenterprise-666)
-	[`couchbase:enterprise-7.0.5`](#couchbaseenterprise-705)
-	[`couchbase:enterprise-7.1.6`](#couchbaseenterprise-716)
-	[`couchbase:enterprise-7.2.3`](#couchbaseenterprise-723)
-	[`couchbase:latest`](#couchbaselatest)

## `couchbase:6.6.6`

```console
$ docker pull couchbase@sha256:c5c8902844c614563a6ce85e6c9f046f9613358226b7106f8b14852b3d8efd21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:6.6.6` - linux; amd64

```console
$ docker pull couchbase@sha256:c59a6cb7131a2f8a1476cc7a96a06d197317d92b572ae3c9166cc9d97b52d0d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **532.0 MB (532022400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1a8e82106c94925522c8767228df70e597c4b6d86ab28743206135ca46b8f8f`
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
# Sat, 02 Dec 2023 04:39:19 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6
# Sat, 02 Dec 2023 04:39:19 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb
# Sat, 02 Dec 2023 04:39:19 GMT
ARG CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa
# Sat, 02 Dec 2023 04:39:19 GMT
ARG CB_SKIP_CHECKSUM=false
# Sat, 02 Dec 2023 04:39:19 GMT
ARG CB_PACKAGE_NAME=couchbase-server
# Sat, 02 Dec 2023 04:39:19 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Sat, 02 Dec 2023 04:39:20 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Sat, 02 Dec 2023 04:40:18 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && dpkg --unpack ./$CB_PACKAGE     && sed -i -e '/Best heuristic/ a \ \ \ \ [ -d /run/systemd/system ] && return 1; return 0' /opt/couchbase/bin/install/systemd-ctl     && dpkg --configure couchbase-server     && apt-get install -yf     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Sat, 02 Dec 2023 04:40:21 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Sat, 02 Dec 2023 04:40:22 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Sat, 02 Dec 2023 04:40:22 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Sat, 02 Dec 2023 04:40:22 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Sat, 02 Dec 2023 04:40:23 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Sat, 02 Dec 2023 04:40:23 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Sat, 02 Dec 2023 04:40:23 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Sat, 02 Dec 2023 04:40:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 04:40:23 GMT
CMD ["couchbase-server"]
# Sat, 02 Dec 2023 04:40:24 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Sat, 02 Dec 2023 04:40:24 GMT
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
	-	`sha256:b95165784d282f95860430bc1191579c77d335b0404c614b83d25b04608d630e`  
		Last Modified: Sat, 02 Dec 2023 04:46:31 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb369cc3658438e3a5cf47ae533359d6f8b384cee669559a598b6609aad514b7`  
		Last Modified: Sat, 02 Dec 2023 04:47:16 GMT  
		Size: 497.1 MB (497147893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f134a7000efa185ccd202c0d13b0af5357166ab9e44ebab5e0cc0c91051404a`  
		Last Modified: Sat, 02 Dec 2023 04:46:31 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae75b6212c00c01a6d144a84147d5c7dc1b5376a8a7d6321def0f565c896f2b`  
		Last Modified: Sat, 02 Dec 2023 04:46:29 GMT  
		Size: 745.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e3a3264c2781947ee720382b69d041c3ada50b0bf4842fcb5c6556b400e0dc`  
		Last Modified: Sat, 02 Dec 2023 04:46:29 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12561950dd2e057fedbd34194fa71cf1d5a86e900fe60afbe9ed9a88047cdf2`  
		Last Modified: Sat, 02 Dec 2023 04:46:29 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4479107f4102f5b3eee56bbea3ae46d58e30c38e7abb8c10291138fd2f05aa3a`  
		Last Modified: Sat, 02 Dec 2023 04:46:29 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b558a4cfceed6f39e9b26fa443f984372e6d3bfc157e326ea132bf8f3a5f0c5`  
		Last Modified: Sat, 02 Dec 2023 04:46:29 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:7.0.5`

```console
$ docker pull couchbase@sha256:62527bd8a005fb33edae9ced2a413aef3eccbd56717355b21f8352e55317a99d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:7.0.5` - linux; amd64

```console
$ docker pull couchbase@sha256:afffef23f4cf2e0d18ba8148a376dfbfa9036f382e4d1ece155fd36357934aff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **616.7 MB (616704804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ae9dc9778c894fc42982104dc360a9ead437af87ffb1f3f0d734277affeba7b`
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
# Sat, 02 Dec 2023 04:36:45 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5
# Sat, 02 Dec 2023 04:36:45 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb
# Sat, 02 Dec 2023 04:36:45 GMT
ARG CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea
# Sat, 02 Dec 2023 04:36:45 GMT
ARG CB_SKIP_CHECKSUM=false
# Sat, 02 Dec 2023 04:36:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Sat, 02 Dec 2023 04:36:46 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Sat, 02 Dec 2023 04:37:56 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Sat, 02 Dec 2023 04:38:00 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Sat, 02 Dec 2023 04:38:00 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Sat, 02 Dec 2023 04:38:01 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Sat, 02 Dec 2023 04:38:01 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Sat, 02 Dec 2023 04:38:01 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Sat, 02 Dec 2023 04:38:02 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Sat, 02 Dec 2023 04:38:02 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Sat, 02 Dec 2023 04:38:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 04:38:02 GMT
CMD ["couchbase-server"]
# Sat, 02 Dec 2023 04:38:02 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Sat, 02 Dec 2023 04:38:02 GMT
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
	-	`sha256:d2794d6f1fb311566d313e3569684a1949cbf6a84798a305118aa1fa0414946d`  
		Last Modified: Sat, 02 Dec 2023 04:44:35 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d510f4b2ee574f99d51c4bb265c837c69db0ef400d539e05a59ea8bbd4ea54`  
		Last Modified: Sat, 02 Dec 2023 04:45:28 GMT  
		Size: 581.8 MB (581830296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47710ed7d267e80f7588b4f2aa5367a8a5051eb5127b01752081bd18f19de00`  
		Last Modified: Sat, 02 Dec 2023 04:44:35 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5d55a9145e95e2575f1d847d85b992eaebdb1785db84c4200e87289c22640ad`  
		Last Modified: Sat, 02 Dec 2023 04:44:33 GMT  
		Size: 745.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab09eba960db9a99154fc47276911f084831d4fd0508a4f87627f6ea10f2742`  
		Last Modified: Sat, 02 Dec 2023 04:44:33 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa8cdf30919ca2c236179cd0f2666704fec4efa774f1ec1c84a1916c331478ab`  
		Last Modified: Sat, 02 Dec 2023 04:44:33 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d143b92791f3b04e595c1f04d98c9e67c0a062ced4f2ba68397e72d8831badc`  
		Last Modified: Sat, 02 Dec 2023 04:44:33 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d592ac9d36387331995e1c9f8dd126ee66aab4248b1cdd49a9e8c6bf516e8610`  
		Last Modified: Sat, 02 Dec 2023 04:44:33 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:7.1.6`

```console
$ docker pull couchbase@sha256:d500cf00d3d7d0f64060156e3809c5c726956655cf775581b4ef861fb7feb561
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchbase:7.1.6` - linux; amd64

```console
$ docker pull couchbase@sha256:7a8abb41ca8835fa15905ce6d66053e365021ac3e3d014362da0a7adfe3098f8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **652.0 MB (652022294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca014cca5430d7f23d07381e3e8d488c6de95dadb5f3aa9dea5c44d927c01482`
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
# Sat, 02 Dec 2023 04:34:08 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6
# Sat, 02 Dec 2023 04:34:08 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb
# Sat, 02 Dec 2023 04:34:08 GMT
ARG CB_SKIP_CHECKSUM=false
# Sat, 02 Dec 2023 04:34:08 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Sat, 02 Dec 2023 04:34:09 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Sat, 02 Dec 2023 04:35:27 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=d4462e7228c372f761bd83f96fa63a7211544df885c2d2e065202ff663dad6f9            ;;          'amd64')            CB_SHA256=abf410a1f97dd14171cd260d4abb853be003db5ec0a44c8324c846068eb90ce7            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Sat, 02 Dec 2023 04:35:29 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Sat, 02 Dec 2023 04:35:29 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Sat, 02 Dec 2023 04:35:30 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Sat, 02 Dec 2023 04:35:30 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Sat, 02 Dec 2023 04:35:30 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Sat, 02 Dec 2023 04:35:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Sat, 02 Dec 2023 04:35:31 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Sat, 02 Dec 2023 04:35:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 04:35:31 GMT
CMD ["couchbase-server"]
# Sat, 02 Dec 2023 04:35:31 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Sat, 02 Dec 2023 04:35:31 GMT
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
	-	`sha256:741f70e047bbbbcd1ddee7fc5c6ff114b14f9023d82f25254e58c6989b7ef699`  
		Last Modified: Sat, 02 Dec 2023 04:42:43 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2c5f2b514272678b0f76febdf8ced7c5d7d7345e0ce98bcfdefb7fe4d6c2ae`  
		Last Modified: Sat, 02 Dec 2023 04:43:41 GMT  
		Size: 617.1 MB (617147797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc3bc35b7df5f8b83cef072dc2f052ab925cd66ff15282b82802b1641e3a5ad`  
		Last Modified: Sat, 02 Dec 2023 04:42:43 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672c61b0cc48318b088e351dd090f358739ead188422badad94bea3e557821b2`  
		Last Modified: Sat, 02 Dec 2023 04:42:41 GMT  
		Size: 742.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a6ce31d0d0df46e32b3ab5a26a8a07dad1def7cca3fd76e8b981434cdaa404d`  
		Last Modified: Sat, 02 Dec 2023 04:42:41 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf714cd839fb4f84896e5ed5b8cc36ad10d9dac7223353046d59cf9329b403f`  
		Last Modified: Sat, 02 Dec 2023 04:42:41 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d976b16760f5c190bde1a2c60be155a6628dad205c320832a23855d06e76b936`  
		Last Modified: Sat, 02 Dec 2023 04:42:41 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d005b04dac33867c717beee3a92588637ad1feda35c6b1f83917e2f02a4be22`  
		Last Modified: Sat, 02 Dec 2023 04:42:41 GMT  
		Size: 866.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchbase:7.1.6` - linux; arm64 variant v8

```console
$ docker pull couchbase@sha256:3c856749a1ed8abe974e97bd3d5a4214849168f8758454130c22cce79e09d0d8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **622.6 MB (622642960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eee50148abaaeddfe928a0aa3bdb4ac72d30a825f88b77a813569b91960a532d`
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
# Sat, 02 Dec 2023 05:02:02 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6
# Sat, 02 Dec 2023 05:02:02 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb
# Sat, 02 Dec 2023 05:02:02 GMT
ARG CB_SKIP_CHECKSUM=false
# Sat, 02 Dec 2023 05:02:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Sat, 02 Dec 2023 05:02:03 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Sat, 02 Dec 2023 05:03:05 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=d4462e7228c372f761bd83f96fa63a7211544df885c2d2e065202ff663dad6f9            ;;          'amd64')            CB_SHA256=abf410a1f97dd14171cd260d4abb853be003db5ec0a44c8324c846068eb90ce7            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Sat, 02 Dec 2023 05:03:13 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Sat, 02 Dec 2023 05:03:13 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Sat, 02 Dec 2023 05:03:13 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Sat, 02 Dec 2023 05:03:13 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Sat, 02 Dec 2023 05:03:14 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Sat, 02 Dec 2023 05:03:14 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Sat, 02 Dec 2023 05:03:14 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Sat, 02 Dec 2023 05:03:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 05:03:14 GMT
CMD ["couchbase-server"]
# Sat, 02 Dec 2023 05:03:14 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Sat, 02 Dec 2023 05:03:14 GMT
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
	-	`sha256:6ab038dcce8e950534800e4e83efa36b4550ae73e0b9804b12b357b79f066448`  
		Last Modified: Sat, 02 Dec 2023 05:05:56 GMT  
		Size: 1.8 KB (1839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ce5c3e88f35d31b1f8ad98a58bff413ec9b2b4238471a71ef0a25955cd6700`  
		Last Modified: Sat, 02 Dec 2023 05:06:36 GMT  
		Size: 589.3 MB (589325223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d04d868de389f9f4c2357cba5a6e3851ae8b7f1f9e2f2ce5e4b726c8c758f40b`  
		Last Modified: Sat, 02 Dec 2023 05:05:56 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d65e9b5f53b17f492cc0c17975c0c0f5abb573c04d2d1a9eca10eb3851e9199`  
		Last Modified: Sat, 02 Dec 2023 05:05:54 GMT  
		Size: 743.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb358361cfd86549547d4d83918ee5496ff49fab58d6e4e39cebe6f2ff790ab9`  
		Last Modified: Sat, 02 Dec 2023 05:05:54 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a422500587009860959352772257ee41bbf6c579719fa4bebb96fa9226e9ba6f`  
		Last Modified: Sat, 02 Dec 2023 05:05:54 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e275b220250392ba4d19e8c5ba806adf1d917ab83ef94bd033ea2bab49b951c2`  
		Last Modified: Sat, 02 Dec 2023 05:05:54 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c12f4e78b1fed2adcdcbd93ea49bf6532100691849a8230fd8ad3617cb0608d6`  
		Last Modified: Sat, 02 Dec 2023 05:05:54 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:7.2.3`

```console
$ docker pull couchbase@sha256:5e5cf0ff763af2cc3676b0f180004c69a8ebcb5a2a69cb350df18ad793bb6b04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchbase:7.2.3` - linux; amd64

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

### `couchbase:7.2.3` - linux; arm64 variant v8

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

## `couchbase:community`

```console
$ docker pull couchbase@sha256:7e5af76785d2784718c7ebc163bb0767139a8480eb140f70a70a8579290d64c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchbase:community` - linux; amd64

```console
$ docker pull couchbase@sha256:1c2d61007f63ff13f27dd5f37d825b7d6ccee89a190567017bb19c8c948da337
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **361.6 MB (361639760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:777dfc2f688532f628935628516dfcabb322522a0ac54391120670905076e568`
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
# Sat, 02 Dec 2023 04:33:09 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2
# Sat, 02 Dec 2023 04:33:10 GMT
ARG CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb
# Sat, 02 Dec 2023 04:33:10 GMT
ARG CB_SKIP_CHECKSUM=false
# Sat, 02 Dec 2023 04:33:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Sat, 02 Dec 2023 04:33:10 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Sat, 02 Dec 2023 04:33:55 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=15e8e8185882210ea02ad83e3667714cce16293afad29506adf07131d684f2db            ;;          'amd64')            CB_SHA256=71bd7359e07810726c3f2735e71aa2a41e6da0865407d407bd666a3d123fa5dc            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Sat, 02 Dec 2023 04:33:58 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Sat, 02 Dec 2023 04:33:58 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Sat, 02 Dec 2023 04:33:58 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Sat, 02 Dec 2023 04:33:58 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Sat, 02 Dec 2023 04:33:59 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Sat, 02 Dec 2023 04:33:59 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Sat, 02 Dec 2023 04:33:59 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Sat, 02 Dec 2023 04:33:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 04:33:59 GMT
CMD ["couchbase-server"]
# Sat, 02 Dec 2023 04:34:00 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Sat, 02 Dec 2023 04:34:00 GMT
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
	-	`sha256:e8e039c045a9969906cae2c070214231badb5f7f7cd4694d92bd7ec5d3e2b4a4`  
		Last Modified: Sat, 02 Dec 2023 04:41:57 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd481c140ddae299421b1de4c3788174283efa934c728af4ab6baecbf9ac193`  
		Last Modified: Sat, 02 Dec 2023 04:42:33 GMT  
		Size: 326.8 MB (326765266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:125d2173bb2069674289bd6d5d4c2771ca30da7ca59b6550aefdffd234e87276`  
		Last Modified: Sat, 02 Dec 2023 04:41:57 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:549cbdd6a3f620c19560bfc012ac3a48e59d958d7a8c56b08de8d9b213318999`  
		Last Modified: Sat, 02 Dec 2023 04:41:55 GMT  
		Size: 743.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7a0ca125b64bf1a6bda39c0f5b5f1e383bf7d471186710bda19c9ceb7ad3db`  
		Last Modified: Sat, 02 Dec 2023 04:41:55 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9aee0405b7778b8bd2497d60af62090967ba61066a49093d9deee15259cfdd`  
		Last Modified: Sat, 02 Dec 2023 04:41:55 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8cc970b1d11e6a85a739a7e3167bcd743b73992117042a6770cc23a873048e`  
		Last Modified: Sat, 02 Dec 2023 04:41:55 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0064a1218edb7e0cbfc2ff7afea072b81df7e823ec27173545a1100e13fd305f`  
		Last Modified: Sat, 02 Dec 2023 04:41:55 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchbase:community` - linux; arm64 variant v8

```console
$ docker pull couchbase@sha256:73b7ffcd6ee95b9f40298fd0d0688ce9c8408585ce5c4cae3a9e640a1cdc9437
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.3 MB (338250147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:835c0d475a411402af17a6229df7f9198571d1bf101859005de3380517e835fa`
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
# Sat, 02 Dec 2023 05:01:14 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2
# Sat, 02 Dec 2023 05:01:14 GMT
ARG CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb
# Sat, 02 Dec 2023 05:01:14 GMT
ARG CB_SKIP_CHECKSUM=false
# Sat, 02 Dec 2023 05:01:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Sat, 02 Dec 2023 05:01:15 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Sat, 02 Dec 2023 05:01:50 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=15e8e8185882210ea02ad83e3667714cce16293afad29506adf07131d684f2db            ;;          'amd64')            CB_SHA256=71bd7359e07810726c3f2735e71aa2a41e6da0865407d407bd666a3d123fa5dc            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Sat, 02 Dec 2023 05:01:56 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Sat, 02 Dec 2023 05:01:56 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Sat, 02 Dec 2023 05:01:57 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Sat, 02 Dec 2023 05:01:57 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Sat, 02 Dec 2023 05:01:57 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Sat, 02 Dec 2023 05:01:58 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Sat, 02 Dec 2023 05:01:58 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Sat, 02 Dec 2023 05:01:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 05:01:58 GMT
CMD ["couchbase-server"]
# Sat, 02 Dec 2023 05:01:58 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Sat, 02 Dec 2023 05:01:58 GMT
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
	-	`sha256:1ad9c7fcda9559b49e143f423a1693f3d05d280e9d18dcafe3d0214ea217e0fc`  
		Last Modified: Sat, 02 Dec 2023 05:05:19 GMT  
		Size: 1.8 KB (1842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19896a300ef0f70ff73969f70ee52778607900326fbf2118d4bf1fc8e365c66`  
		Last Modified: Sat, 02 Dec 2023 05:05:45 GMT  
		Size: 304.9 MB (304932402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e529d8bfcaf10c6bd6a5c55c83968c0035ff39c8eb62e3a095406c7d8164dc1a`  
		Last Modified: Sat, 02 Dec 2023 05:05:19 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb97afb0a18a337a1b36f95fe7a2c33b09dc97eb8abaf0f1a1b5619d4e876ad`  
		Last Modified: Sat, 02 Dec 2023 05:05:17 GMT  
		Size: 745.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a900d471317b4b663a5c75739abf179877205d96c7ecea9fcf535d06db6bff3`  
		Last Modified: Sat, 02 Dec 2023 05:05:17 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ecff4b6f6e4a939fa87f6fa89c6fbfd015980097a1b7c54ac753cdaa5c1b0ab`  
		Last Modified: Sat, 02 Dec 2023 05:05:17 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c430d6f8971ea671c8f8777bfa0ae572677f4861c5ec82059cc516130b5299`  
		Last Modified: Sat, 02 Dec 2023 05:05:17 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45bb29edbe5617fed7485e4a68037ca201c6af7f26f9e70afd84b760ec6cd84a`  
		Last Modified: Sat, 02 Dec 2023 05:05:17 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community-6.6.0`

```console
$ docker pull couchbase@sha256:43103efdd4b562366c7a48afa977c4ad148e09c877da28a83a86b2c5ee2daa97
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:community-6.6.0` - linux; amd64

```console
$ docker pull couchbase@sha256:733f14529d8ce4ca199fead4b0e7b70d64707c694e7d59941e9a8fa465d0d14a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **352.5 MB (352547379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd5ed30ac5a740e1c21e9670045cc39cdd980f2d6336e38074dbf09e4953e071`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 30 May 2023 09:32:07 GMT
ARG RELEASE
# Tue, 30 May 2023 09:32:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:32:09 GMT
ADD file:3c74e7e08cbf9a87694ce6fa541af617599680fa54d9e48556fc0fbc120b4a83 in / 
# Tue, 30 May 2023 09:32:09 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:52:57 GMT
LABEL maintainer=docker@couchbase.com
# Fri, 02 Jun 2023 00:52:57 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Fri, 02 Jun 2023 00:52:57 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Fri, 02 Jun 2023 00:53:13 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Fri, 02 Jun 2023 00:53:14 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0
# Fri, 02 Jun 2023 00:53:14 GMT
ARG CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb
# Fri, 02 Jun 2023 00:53:14 GMT
ARG CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559
# Fri, 02 Jun 2023 00:53:14 GMT
ARG CB_SKIP_CHECKSUM=false
# Fri, 02 Jun 2023 00:53:14 GMT
ARG CB_PACKAGE_NAME=couchbase-server-community
# Fri, 02 Jun 2023 00:53:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 02 Jun 2023 00:53:15 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server-community CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 02 Jun 2023 00:53:51 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server-community CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && dpkg --unpack ./$CB_PACKAGE     && sed -i -e '/Best heuristic/ a \ \ \ \ [ -d /run/systemd/system ] && return 1; return 0' /opt/couchbase/bin/install/systemd-ctl     && dpkg --configure couchbase-server-community     && apt-get install -yf     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Fri, 02 Jun 2023 00:53:53 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server-community CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Fri, 02 Jun 2023 00:53:53 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Fri, 02 Jun 2023 00:53:54 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server-community CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Fri, 02 Jun 2023 00:53:54 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 02 Jun 2023 00:53:54 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server-community CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 02 Jun 2023 00:54:04 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server-community CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Fri, 02 Jun 2023 00:54:04 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Fri, 02 Jun 2023 00:54:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Jun 2023 00:54:04 GMT
CMD ["couchbase-server"]
# Fri, 02 Jun 2023 00:54:04 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Fri, 02 Jun 2023 00:54:04 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:41af1b5f0f51947706ae712999cf098bef968a7799e7cb4bb2268829e62a6ab3`  
		Last Modified: Fri, 02 Jun 2023 00:09:06 GMT  
		Size: 26.7 MB (26717357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab5f202a3c4b1bd6205dc849c236881ff887808976fbf649e678dff74a73934`  
		Last Modified: Fri, 02 Jun 2023 00:54:23 GMT  
		Size: 5.6 MB (5629354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dadf0925394d75b216c6a30f94134fe95733d405956abf344dc3048c719c877`  
		Last Modified: Fri, 02 Jun 2023 00:54:22 GMT  
		Size: 2.0 KB (1962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40492fc9a214ba15d8bb4c524ec9e72b8b35a76beab8196b16842325b6e56783`  
		Last Modified: Fri, 02 Jun 2023 00:54:54 GMT  
		Size: 319.8 MB (319763045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f21f2b605acadae68e7c2bd841e9f21af1de5b216cf72f026ba93be04266ddb`  
		Last Modified: Fri, 02 Jun 2023 00:54:22 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ab2e4a82b64efff588831a51244dbb85c77ea5d3374438e5aed551ff3ba84d`  
		Last Modified: Fri, 02 Jun 2023 00:54:21 GMT  
		Size: 738.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2eaeb0e9ba32a1677e828e005bc16c3855f43587500c1cb07fb4f62e7afceb`  
		Last Modified: Fri, 02 Jun 2023 00:54:20 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c82b8edf16e57d16d79bcfc3ac0d58af7910eb4295c1c14a575d5299dca634`  
		Last Modified: Fri, 02 Jun 2023 00:54:20 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15775e525cac0400a6f14e171b409884f6ac33affcaa39fa8537d7c0975350b8`  
		Last Modified: Fri, 02 Jun 2023 00:54:20 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ddf4b17f9af1512ea650822b8fac99fd67d425fb99fdadb3fbb449e8addf2cc`  
		Last Modified: Fri, 02 Jun 2023 00:54:20 GMT  
		Size: 433.1 KB (433134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1139270b66df32366a4850ae2aa3ddc25be3a64b7088770984f457b592d476c`  
		Last Modified: Fri, 02 Jun 2023 00:54:20 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community-7.0.2`

```console
$ docker pull couchbase@sha256:2c02dd364bd9364b2e1b8abe1f9964ccfbe6c172449d06d6eb088b3649411f00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:community-7.0.2` - linux; amd64

```console
$ docker pull couchbase@sha256:cb693c76d10b76312914e106fd08ad5bbfa6b0a1acc45193e8a3cc511c901620
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **429.1 MB (429073076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3225058bc95cf03127581d0c8a8b26ffbc5372904936dc9e7e6fef56f3d98c6`
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
# Sat, 02 Dec 2023 04:38:19 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Sat, 02 Dec 2023 04:38:20 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Sat, 02 Dec 2023 04:38:20 GMT
ARG CB_VERSION=7.0.2
# Sat, 02 Dec 2023 04:38:20 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2
# Sat, 02 Dec 2023 04:38:20 GMT
ARG CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb
# Sat, 02 Dec 2023 04:38:20 GMT
ARG CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e
# Sat, 02 Dec 2023 04:38:20 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Sat, 02 Dec 2023 04:38:21 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Sat, 02 Dec 2023 04:39:10 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Sat, 02 Dec 2023 04:39:14 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Sat, 02 Dec 2023 04:39:14 GMT
COPY file:cf9c7c8a9eda8a5fefcaa60d67181024b8a07b30eb318d4c9591b33a95ca6680 in /etc/service/couchbase-server/run 
# Sat, 02 Dec 2023 04:39:14 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Sat, 02 Dec 2023 04:39:14 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Sat, 02 Dec 2023 04:39:15 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Sat, 02 Dec 2023 04:39:15 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Sat, 02 Dec 2023 04:39:15 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Sat, 02 Dec 2023 04:39:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 04:39:16 GMT
CMD ["couchbase-server"]
# Sat, 02 Dec 2023 04:39:16 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Sat, 02 Dec 2023 04:39:16 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:30ecab32a3b65c6ec04c63a65b90e627b49d1297d8793896ed50b656377d8a06`  
		Last Modified: Tue, 28 Nov 2023 10:11:56 GMT  
		Size: 28.6 MB (28584029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65927d84c24c98e842144855954f018a422bc7e00f62308c065f19ce0edf1e9e`  
		Last Modified: Sat, 02 Dec 2023 04:45:43 GMT  
		Size: 6.3 MB (6292702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2612fc827a2f2cb20b9d45cf6f20bf4df15529289b1db462651dc590613d5901`  
		Last Modified: Sat, 02 Dec 2023 04:45:40 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b40b79652403b877dcb2205c84dbd4ef60ef8351ec632f0787477e380f44361`  
		Last Modified: Sat, 02 Dec 2023 04:45:40 GMT  
		Size: 1.8 KB (1833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9126cbba021dd665a7466dbf63ecf40772147a5f61b215ab903fa7308613883`  
		Last Modified: Sat, 02 Dec 2023 04:46:23 GMT  
		Size: 394.1 MB (394062361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b67e25a6340abd393796f3d27833c93b91b8dd1f572c581aa3af4dfa6cb1576`  
		Last Modified: Sat, 02 Dec 2023 04:45:40 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce50b39df7a855ee9e0d71b930af3b8ca6491ff8cee25ec1f242976060538843`  
		Last Modified: Sat, 02 Dec 2023 04:45:40 GMT  
		Size: 597.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f398ef2f2d335dce55c49e05380613b650449e15fa269b1d1bd245185748fc50`  
		Last Modified: Sat, 02 Dec 2023 04:45:38 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c71a6e05d717a9ba3dd83ddade009d27f0404763464988dd365c88adc3a950`  
		Last Modified: Sat, 02 Dec 2023 04:45:38 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa8c5c217a2ee26e891ce6ac87f0cc80cb3f310fd97da7ccb1ca150a2536ac8`  
		Last Modified: Sat, 02 Dec 2023 04:45:38 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857a79c56d8629196a07236f53adc8d9705294ea30879cb95711279c481ce78d`  
		Last Modified: Sat, 02 Dec 2023 04:45:38 GMT  
		Size: 129.5 KB (129508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cecd8f43744f56644c9aedc42f287f21c38f2f11246a77ec01fd5fece7dd0336`  
		Last Modified: Sat, 02 Dec 2023 04:45:38 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community-7.1.1`

```console
$ docker pull couchbase@sha256:cd6bedd5f84c5e8919a381b75845bb18adf88ee24d68d5542bb93465e658f727
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchbase:community-7.1.1` - linux; amd64

```console
$ docker pull couchbase@sha256:f71cb5791e83c1125f4e6a457c98e9f37c8a3151110bcbb58ddd159dc8ed4648
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.7 MB (346674223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b12387335e21a1f8a56a4064ff238d74766b265c3b8515a53acd3758fafd5393`
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
# Sat, 02 Dec 2023 04:35:47 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1
# Sat, 02 Dec 2023 04:35:47 GMT
ARG CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb
# Sat, 02 Dec 2023 04:35:47 GMT
ARG CB_SKIP_CHECKSUM=false
# Sat, 02 Dec 2023 04:35:47 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Sat, 02 Dec 2023 04:35:47 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Sat, 02 Dec 2023 04:36:29 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=275a0bb41d81920e9948fc05f736eef753179f698a04609eb8fe617d0fe55b8b            ;;          'amd64')            CB_SHA256=2fa47dc00f6d85aad5298149bb52450cc98c2c1e18eb54ab8ed45346c24a9403            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Sat, 02 Dec 2023 04:36:32 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Sat, 02 Dec 2023 04:36:32 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Sat, 02 Dec 2023 04:36:33 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Sat, 02 Dec 2023 04:36:33 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Sat, 02 Dec 2023 04:36:33 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Sat, 02 Dec 2023 04:36:34 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Sat, 02 Dec 2023 04:36:34 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Sat, 02 Dec 2023 04:36:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 04:36:34 GMT
CMD ["couchbase-server"]
# Sat, 02 Dec 2023 04:36:34 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Sat, 02 Dec 2023 04:36:34 GMT
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
	-	`sha256:f581649588541f2ec5f90144ee7d27131fddd2590e1e97eff9e4e43005f13596`  
		Last Modified: Sat, 02 Dec 2023 04:43:52 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec7b906f344a1a2011c71dd95533511f4744f7da87554cb7122f2fa1caa41ac`  
		Last Modified: Sat, 02 Dec 2023 04:44:26 GMT  
		Size: 311.8 MB (311799720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7055055bdfab17c4734f796f9580b625012f802c1839065188bebc886c69b0a7`  
		Last Modified: Sat, 02 Dec 2023 04:43:52 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047f8cc8cc5b0a33daca20d3856cbaf3b41b7dd0e30ef11ba69d64d802418e82`  
		Last Modified: Sat, 02 Dec 2023 04:43:50 GMT  
		Size: 745.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03232613e49c9053a1a5bae737e81e681f97419b70b8bae815ffba93424cd05`  
		Last Modified: Sat, 02 Dec 2023 04:43:50 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c65bd14b9bb6addb37fb9ef912974e63231c8604d304553b44a8573943536d8b`  
		Last Modified: Sat, 02 Dec 2023 04:43:50 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a161b0053778b3a3149ced460e960515ae4b23cab0c05157d9f286518e3f33f`  
		Last Modified: Sat, 02 Dec 2023 04:43:50 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaab0ae15c8e9553aa27690fab698d7a6d221b932dc636956875f4065f536ba3`  
		Last Modified: Sat, 02 Dec 2023 04:43:51 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchbase:community-7.1.1` - linux; arm64 variant v8

```console
$ docker pull couchbase@sha256:cdf01b56df3836c3493039b63d04a63baf27d4fd552fda79d5b5144ddb3a59aa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.3 MB (327343653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8c966d7cff68b5966cedf7fd5cfce2b528ae947bbff539f25495a4cb356dcde`
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
# Sat, 02 Dec 2023 05:03:25 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1
# Sat, 02 Dec 2023 05:03:25 GMT
ARG CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb
# Sat, 02 Dec 2023 05:03:25 GMT
ARG CB_SKIP_CHECKSUM=false
# Sat, 02 Dec 2023 05:03:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Sat, 02 Dec 2023 05:03:26 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Sat, 02 Dec 2023 05:04:00 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=275a0bb41d81920e9948fc05f736eef753179f698a04609eb8fe617d0fe55b8b            ;;          'amd64')            CB_SHA256=2fa47dc00f6d85aad5298149bb52450cc98c2c1e18eb54ab8ed45346c24a9403            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Sat, 02 Dec 2023 05:04:06 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Sat, 02 Dec 2023 05:04:06 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Sat, 02 Dec 2023 05:04:06 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Sat, 02 Dec 2023 05:04:06 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Sat, 02 Dec 2023 05:04:07 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Sat, 02 Dec 2023 05:04:07 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Sat, 02 Dec 2023 05:04:07 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Sat, 02 Dec 2023 05:04:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 05:04:08 GMT
CMD ["couchbase-server"]
# Sat, 02 Dec 2023 05:04:08 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Sat, 02 Dec 2023 05:04:08 GMT
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
	-	`sha256:647a354037dffc8198d30c7d569431a09c39974ca7049530892e6767f6a63a7d`  
		Last Modified: Sat, 02 Dec 2023 05:06:46 GMT  
		Size: 1.8 KB (1839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ea8635765fa8c4498238120051ec6c34c5c11971a766a6656c7da4e86c9c4f`  
		Last Modified: Sat, 02 Dec 2023 05:07:11 GMT  
		Size: 294.0 MB (294025912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db608a9098a8ced7b0138d94a6c501041d3e0cdc9fc7b8059a2d15c82193fb7`  
		Last Modified: Sat, 02 Dec 2023 05:06:46 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f2a8ec3594de3e177923fc510bdf8190dffcc7232c2ae0616cee5b8f0e3932`  
		Last Modified: Sat, 02 Dec 2023 05:06:44 GMT  
		Size: 745.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5bcdd388d16ea03d63ba51b60529c1f809cddd2713a3690b9377e3d6002121b`  
		Last Modified: Sat, 02 Dec 2023 05:06:44 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a78bf26a3bf756a49c5f4b5f89edddbcf34ad3f44141af8e03ec3c321d7572b`  
		Last Modified: Sat, 02 Dec 2023 05:06:44 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac70be9026585f2b613358f5e5ed0d467fa9d0656e3b03f42504eccea0a2a79`  
		Last Modified: Sat, 02 Dec 2023 05:06:44 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb47b6edb424651b36d9bdec02133c23a962a0f27303698afae5335bfa88696`  
		Last Modified: Sat, 02 Dec 2023 05:06:44 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community-7.2.2`

```console
$ docker pull couchbase@sha256:7e5af76785d2784718c7ebc163bb0767139a8480eb140f70a70a8579290d64c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchbase:community-7.2.2` - linux; amd64

```console
$ docker pull couchbase@sha256:1c2d61007f63ff13f27dd5f37d825b7d6ccee89a190567017bb19c8c948da337
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **361.6 MB (361639760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:777dfc2f688532f628935628516dfcabb322522a0ac54391120670905076e568`
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
# Sat, 02 Dec 2023 04:33:09 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2
# Sat, 02 Dec 2023 04:33:10 GMT
ARG CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb
# Sat, 02 Dec 2023 04:33:10 GMT
ARG CB_SKIP_CHECKSUM=false
# Sat, 02 Dec 2023 04:33:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Sat, 02 Dec 2023 04:33:10 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Sat, 02 Dec 2023 04:33:55 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=15e8e8185882210ea02ad83e3667714cce16293afad29506adf07131d684f2db            ;;          'amd64')            CB_SHA256=71bd7359e07810726c3f2735e71aa2a41e6da0865407d407bd666a3d123fa5dc            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Sat, 02 Dec 2023 04:33:58 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Sat, 02 Dec 2023 04:33:58 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Sat, 02 Dec 2023 04:33:58 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Sat, 02 Dec 2023 04:33:58 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Sat, 02 Dec 2023 04:33:59 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Sat, 02 Dec 2023 04:33:59 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Sat, 02 Dec 2023 04:33:59 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Sat, 02 Dec 2023 04:33:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 04:33:59 GMT
CMD ["couchbase-server"]
# Sat, 02 Dec 2023 04:34:00 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Sat, 02 Dec 2023 04:34:00 GMT
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
	-	`sha256:e8e039c045a9969906cae2c070214231badb5f7f7cd4694d92bd7ec5d3e2b4a4`  
		Last Modified: Sat, 02 Dec 2023 04:41:57 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd481c140ddae299421b1de4c3788174283efa934c728af4ab6baecbf9ac193`  
		Last Modified: Sat, 02 Dec 2023 04:42:33 GMT  
		Size: 326.8 MB (326765266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:125d2173bb2069674289bd6d5d4c2771ca30da7ca59b6550aefdffd234e87276`  
		Last Modified: Sat, 02 Dec 2023 04:41:57 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:549cbdd6a3f620c19560bfc012ac3a48e59d958d7a8c56b08de8d9b213318999`  
		Last Modified: Sat, 02 Dec 2023 04:41:55 GMT  
		Size: 743.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7a0ca125b64bf1a6bda39c0f5b5f1e383bf7d471186710bda19c9ceb7ad3db`  
		Last Modified: Sat, 02 Dec 2023 04:41:55 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9aee0405b7778b8bd2497d60af62090967ba61066a49093d9deee15259cfdd`  
		Last Modified: Sat, 02 Dec 2023 04:41:55 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8cc970b1d11e6a85a739a7e3167bcd743b73992117042a6770cc23a873048e`  
		Last Modified: Sat, 02 Dec 2023 04:41:55 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0064a1218edb7e0cbfc2ff7afea072b81df7e823ec27173545a1100e13fd305f`  
		Last Modified: Sat, 02 Dec 2023 04:41:55 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchbase:community-7.2.2` - linux; arm64 variant v8

```console
$ docker pull couchbase@sha256:73b7ffcd6ee95b9f40298fd0d0688ce9c8408585ce5c4cae3a9e640a1cdc9437
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.3 MB (338250147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:835c0d475a411402af17a6229df7f9198571d1bf101859005de3380517e835fa`
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
# Sat, 02 Dec 2023 05:01:14 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2
# Sat, 02 Dec 2023 05:01:14 GMT
ARG CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb
# Sat, 02 Dec 2023 05:01:14 GMT
ARG CB_SKIP_CHECKSUM=false
# Sat, 02 Dec 2023 05:01:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Sat, 02 Dec 2023 05:01:15 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Sat, 02 Dec 2023 05:01:50 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=15e8e8185882210ea02ad83e3667714cce16293afad29506adf07131d684f2db            ;;          'amd64')            CB_SHA256=71bd7359e07810726c3f2735e71aa2a41e6da0865407d407bd666a3d123fa5dc            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Sat, 02 Dec 2023 05:01:56 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Sat, 02 Dec 2023 05:01:56 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Sat, 02 Dec 2023 05:01:57 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Sat, 02 Dec 2023 05:01:57 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Sat, 02 Dec 2023 05:01:57 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Sat, 02 Dec 2023 05:01:58 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Sat, 02 Dec 2023 05:01:58 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Sat, 02 Dec 2023 05:01:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 05:01:58 GMT
CMD ["couchbase-server"]
# Sat, 02 Dec 2023 05:01:58 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Sat, 02 Dec 2023 05:01:58 GMT
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
	-	`sha256:1ad9c7fcda9559b49e143f423a1693f3d05d280e9d18dcafe3d0214ea217e0fc`  
		Last Modified: Sat, 02 Dec 2023 05:05:19 GMT  
		Size: 1.8 KB (1842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19896a300ef0f70ff73969f70ee52778607900326fbf2118d4bf1fc8e365c66`  
		Last Modified: Sat, 02 Dec 2023 05:05:45 GMT  
		Size: 304.9 MB (304932402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e529d8bfcaf10c6bd6a5c55c83968c0035ff39c8eb62e3a095406c7d8164dc1a`  
		Last Modified: Sat, 02 Dec 2023 05:05:19 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb97afb0a18a337a1b36f95fe7a2c33b09dc97eb8abaf0f1a1b5619d4e876ad`  
		Last Modified: Sat, 02 Dec 2023 05:05:17 GMT  
		Size: 745.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a900d471317b4b663a5c75739abf179877205d96c7ecea9fcf535d06db6bff3`  
		Last Modified: Sat, 02 Dec 2023 05:05:17 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ecff4b6f6e4a939fa87f6fa89c6fbfd015980097a1b7c54ac753cdaa5c1b0ab`  
		Last Modified: Sat, 02 Dec 2023 05:05:17 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c430d6f8971ea671c8f8777bfa0ae572677f4861c5ec82059cc516130b5299`  
		Last Modified: Sat, 02 Dec 2023 05:05:17 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45bb29edbe5617fed7485e4a68037ca201c6af7f26f9e70afd84b760ec6cd84a`  
		Last Modified: Sat, 02 Dec 2023 05:05:17 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise`

```console
$ docker pull couchbase@sha256:5e5cf0ff763af2cc3676b0f180004c69a8ebcb5a2a69cb350df18ad793bb6b04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchbase:enterprise` - linux; amd64

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

### `couchbase:enterprise` - linux; arm64 variant v8

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

## `couchbase:enterprise-6.6.6`

```console
$ docker pull couchbase@sha256:c5c8902844c614563a6ce85e6c9f046f9613358226b7106f8b14852b3d8efd21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.6.6` - linux; amd64

```console
$ docker pull couchbase@sha256:c59a6cb7131a2f8a1476cc7a96a06d197317d92b572ae3c9166cc9d97b52d0d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **532.0 MB (532022400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1a8e82106c94925522c8767228df70e597c4b6d86ab28743206135ca46b8f8f`
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
# Sat, 02 Dec 2023 04:39:19 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6
# Sat, 02 Dec 2023 04:39:19 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb
# Sat, 02 Dec 2023 04:39:19 GMT
ARG CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa
# Sat, 02 Dec 2023 04:39:19 GMT
ARG CB_SKIP_CHECKSUM=false
# Sat, 02 Dec 2023 04:39:19 GMT
ARG CB_PACKAGE_NAME=couchbase-server
# Sat, 02 Dec 2023 04:39:19 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Sat, 02 Dec 2023 04:39:20 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Sat, 02 Dec 2023 04:40:18 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && dpkg --unpack ./$CB_PACKAGE     && sed -i -e '/Best heuristic/ a \ \ \ \ [ -d /run/systemd/system ] && return 1; return 0' /opt/couchbase/bin/install/systemd-ctl     && dpkg --configure couchbase-server     && apt-get install -yf     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Sat, 02 Dec 2023 04:40:21 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Sat, 02 Dec 2023 04:40:22 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Sat, 02 Dec 2023 04:40:22 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Sat, 02 Dec 2023 04:40:22 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Sat, 02 Dec 2023 04:40:23 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Sat, 02 Dec 2023 04:40:23 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Sat, 02 Dec 2023 04:40:23 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Sat, 02 Dec 2023 04:40:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 04:40:23 GMT
CMD ["couchbase-server"]
# Sat, 02 Dec 2023 04:40:24 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Sat, 02 Dec 2023 04:40:24 GMT
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
	-	`sha256:b95165784d282f95860430bc1191579c77d335b0404c614b83d25b04608d630e`  
		Last Modified: Sat, 02 Dec 2023 04:46:31 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb369cc3658438e3a5cf47ae533359d6f8b384cee669559a598b6609aad514b7`  
		Last Modified: Sat, 02 Dec 2023 04:47:16 GMT  
		Size: 497.1 MB (497147893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f134a7000efa185ccd202c0d13b0af5357166ab9e44ebab5e0cc0c91051404a`  
		Last Modified: Sat, 02 Dec 2023 04:46:31 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae75b6212c00c01a6d144a84147d5c7dc1b5376a8a7d6321def0f565c896f2b`  
		Last Modified: Sat, 02 Dec 2023 04:46:29 GMT  
		Size: 745.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e3a3264c2781947ee720382b69d041c3ada50b0bf4842fcb5c6556b400e0dc`  
		Last Modified: Sat, 02 Dec 2023 04:46:29 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12561950dd2e057fedbd34194fa71cf1d5a86e900fe60afbe9ed9a88047cdf2`  
		Last Modified: Sat, 02 Dec 2023 04:46:29 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4479107f4102f5b3eee56bbea3ae46d58e30c38e7abb8c10291138fd2f05aa3a`  
		Last Modified: Sat, 02 Dec 2023 04:46:29 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b558a4cfceed6f39e9b26fa443f984372e6d3bfc157e326ea132bf8f3a5f0c5`  
		Last Modified: Sat, 02 Dec 2023 04:46:29 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-7.0.5`

```console
$ docker pull couchbase@sha256:62527bd8a005fb33edae9ced2a413aef3eccbd56717355b21f8352e55317a99d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-7.0.5` - linux; amd64

```console
$ docker pull couchbase@sha256:afffef23f4cf2e0d18ba8148a376dfbfa9036f382e4d1ece155fd36357934aff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **616.7 MB (616704804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ae9dc9778c894fc42982104dc360a9ead437af87ffb1f3f0d734277affeba7b`
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
# Sat, 02 Dec 2023 04:36:45 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5
# Sat, 02 Dec 2023 04:36:45 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb
# Sat, 02 Dec 2023 04:36:45 GMT
ARG CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea
# Sat, 02 Dec 2023 04:36:45 GMT
ARG CB_SKIP_CHECKSUM=false
# Sat, 02 Dec 2023 04:36:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Sat, 02 Dec 2023 04:36:46 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Sat, 02 Dec 2023 04:37:56 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Sat, 02 Dec 2023 04:38:00 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Sat, 02 Dec 2023 04:38:00 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Sat, 02 Dec 2023 04:38:01 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Sat, 02 Dec 2023 04:38:01 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Sat, 02 Dec 2023 04:38:01 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Sat, 02 Dec 2023 04:38:02 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Sat, 02 Dec 2023 04:38:02 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Sat, 02 Dec 2023 04:38:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 04:38:02 GMT
CMD ["couchbase-server"]
# Sat, 02 Dec 2023 04:38:02 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Sat, 02 Dec 2023 04:38:02 GMT
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
	-	`sha256:d2794d6f1fb311566d313e3569684a1949cbf6a84798a305118aa1fa0414946d`  
		Last Modified: Sat, 02 Dec 2023 04:44:35 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d510f4b2ee574f99d51c4bb265c837c69db0ef400d539e05a59ea8bbd4ea54`  
		Last Modified: Sat, 02 Dec 2023 04:45:28 GMT  
		Size: 581.8 MB (581830296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47710ed7d267e80f7588b4f2aa5367a8a5051eb5127b01752081bd18f19de00`  
		Last Modified: Sat, 02 Dec 2023 04:44:35 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5d55a9145e95e2575f1d847d85b992eaebdb1785db84c4200e87289c22640ad`  
		Last Modified: Sat, 02 Dec 2023 04:44:33 GMT  
		Size: 745.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab09eba960db9a99154fc47276911f084831d4fd0508a4f87627f6ea10f2742`  
		Last Modified: Sat, 02 Dec 2023 04:44:33 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa8cdf30919ca2c236179cd0f2666704fec4efa774f1ec1c84a1916c331478ab`  
		Last Modified: Sat, 02 Dec 2023 04:44:33 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d143b92791f3b04e595c1f04d98c9e67c0a062ced4f2ba68397e72d8831badc`  
		Last Modified: Sat, 02 Dec 2023 04:44:33 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d592ac9d36387331995e1c9f8dd126ee66aab4248b1cdd49a9e8c6bf516e8610`  
		Last Modified: Sat, 02 Dec 2023 04:44:33 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-7.1.6`

```console
$ docker pull couchbase@sha256:d500cf00d3d7d0f64060156e3809c5c726956655cf775581b4ef861fb7feb561
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchbase:enterprise-7.1.6` - linux; amd64

```console
$ docker pull couchbase@sha256:7a8abb41ca8835fa15905ce6d66053e365021ac3e3d014362da0a7adfe3098f8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **652.0 MB (652022294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca014cca5430d7f23d07381e3e8d488c6de95dadb5f3aa9dea5c44d927c01482`
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
# Sat, 02 Dec 2023 04:34:08 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6
# Sat, 02 Dec 2023 04:34:08 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb
# Sat, 02 Dec 2023 04:34:08 GMT
ARG CB_SKIP_CHECKSUM=false
# Sat, 02 Dec 2023 04:34:08 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Sat, 02 Dec 2023 04:34:09 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Sat, 02 Dec 2023 04:35:27 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=d4462e7228c372f761bd83f96fa63a7211544df885c2d2e065202ff663dad6f9            ;;          'amd64')            CB_SHA256=abf410a1f97dd14171cd260d4abb853be003db5ec0a44c8324c846068eb90ce7            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Sat, 02 Dec 2023 04:35:29 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Sat, 02 Dec 2023 04:35:29 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Sat, 02 Dec 2023 04:35:30 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Sat, 02 Dec 2023 04:35:30 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Sat, 02 Dec 2023 04:35:30 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Sat, 02 Dec 2023 04:35:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Sat, 02 Dec 2023 04:35:31 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Sat, 02 Dec 2023 04:35:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 04:35:31 GMT
CMD ["couchbase-server"]
# Sat, 02 Dec 2023 04:35:31 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Sat, 02 Dec 2023 04:35:31 GMT
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
	-	`sha256:741f70e047bbbbcd1ddee7fc5c6ff114b14f9023d82f25254e58c6989b7ef699`  
		Last Modified: Sat, 02 Dec 2023 04:42:43 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2c5f2b514272678b0f76febdf8ced7c5d7d7345e0ce98bcfdefb7fe4d6c2ae`  
		Last Modified: Sat, 02 Dec 2023 04:43:41 GMT  
		Size: 617.1 MB (617147797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc3bc35b7df5f8b83cef072dc2f052ab925cd66ff15282b82802b1641e3a5ad`  
		Last Modified: Sat, 02 Dec 2023 04:42:43 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672c61b0cc48318b088e351dd090f358739ead188422badad94bea3e557821b2`  
		Last Modified: Sat, 02 Dec 2023 04:42:41 GMT  
		Size: 742.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a6ce31d0d0df46e32b3ab5a26a8a07dad1def7cca3fd76e8b981434cdaa404d`  
		Last Modified: Sat, 02 Dec 2023 04:42:41 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf714cd839fb4f84896e5ed5b8cc36ad10d9dac7223353046d59cf9329b403f`  
		Last Modified: Sat, 02 Dec 2023 04:42:41 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d976b16760f5c190bde1a2c60be155a6628dad205c320832a23855d06e76b936`  
		Last Modified: Sat, 02 Dec 2023 04:42:41 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d005b04dac33867c717beee3a92588637ad1feda35c6b1f83917e2f02a4be22`  
		Last Modified: Sat, 02 Dec 2023 04:42:41 GMT  
		Size: 866.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchbase:enterprise-7.1.6` - linux; arm64 variant v8

```console
$ docker pull couchbase@sha256:3c856749a1ed8abe974e97bd3d5a4214849168f8758454130c22cce79e09d0d8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **622.6 MB (622642960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eee50148abaaeddfe928a0aa3bdb4ac72d30a825f88b77a813569b91960a532d`
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
# Sat, 02 Dec 2023 05:02:02 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6
# Sat, 02 Dec 2023 05:02:02 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb
# Sat, 02 Dec 2023 05:02:02 GMT
ARG CB_SKIP_CHECKSUM=false
# Sat, 02 Dec 2023 05:02:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Sat, 02 Dec 2023 05:02:03 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Sat, 02 Dec 2023 05:03:05 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=d4462e7228c372f761bd83f96fa63a7211544df885c2d2e065202ff663dad6f9            ;;          'amd64')            CB_SHA256=abf410a1f97dd14171cd260d4abb853be003db5ec0a44c8324c846068eb90ce7            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Sat, 02 Dec 2023 05:03:13 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Sat, 02 Dec 2023 05:03:13 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Sat, 02 Dec 2023 05:03:13 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Sat, 02 Dec 2023 05:03:13 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Sat, 02 Dec 2023 05:03:14 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Sat, 02 Dec 2023 05:03:14 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Sat, 02 Dec 2023 05:03:14 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Sat, 02 Dec 2023 05:03:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 05:03:14 GMT
CMD ["couchbase-server"]
# Sat, 02 Dec 2023 05:03:14 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Sat, 02 Dec 2023 05:03:14 GMT
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
	-	`sha256:6ab038dcce8e950534800e4e83efa36b4550ae73e0b9804b12b357b79f066448`  
		Last Modified: Sat, 02 Dec 2023 05:05:56 GMT  
		Size: 1.8 KB (1839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ce5c3e88f35d31b1f8ad98a58bff413ec9b2b4238471a71ef0a25955cd6700`  
		Last Modified: Sat, 02 Dec 2023 05:06:36 GMT  
		Size: 589.3 MB (589325223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d04d868de389f9f4c2357cba5a6e3851ae8b7f1f9e2f2ce5e4b726c8c758f40b`  
		Last Modified: Sat, 02 Dec 2023 05:05:56 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d65e9b5f53b17f492cc0c17975c0c0f5abb573c04d2d1a9eca10eb3851e9199`  
		Last Modified: Sat, 02 Dec 2023 05:05:54 GMT  
		Size: 743.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb358361cfd86549547d4d83918ee5496ff49fab58d6e4e39cebe6f2ff790ab9`  
		Last Modified: Sat, 02 Dec 2023 05:05:54 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a422500587009860959352772257ee41bbf6c579719fa4bebb96fa9226e9ba6f`  
		Last Modified: Sat, 02 Dec 2023 05:05:54 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e275b220250392ba4d19e8c5ba806adf1d917ab83ef94bd033ea2bab49b951c2`  
		Last Modified: Sat, 02 Dec 2023 05:05:54 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c12f4e78b1fed2adcdcbd93ea49bf6532100691849a8230fd8ad3617cb0608d6`  
		Last Modified: Sat, 02 Dec 2023 05:05:54 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

## `couchbase:latest`

```console
$ docker pull couchbase@sha256:5e5cf0ff763af2cc3676b0f180004c69a8ebcb5a2a69cb350df18ad793bb6b04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchbase:latest` - linux; amd64

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

### `couchbase:latest` - linux; arm64 variant v8

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
